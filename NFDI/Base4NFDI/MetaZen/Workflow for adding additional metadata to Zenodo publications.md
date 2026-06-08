#zenodo #KnowledgeGraph
#NFDIcoreOntology

- Harvest from Zenodo and GoogleDocs
- Processing
- Storage and query
	- property graph (Neo4J)
	- triple store
- Output
	- JSON-LD sidecars
	- Queryable graph DB
import requests, json, time, pathlib

`COMMUNITY = "base4nfdi"`
`RAW_DIR = pathlib.Path("data/zenodo_raw"); RAW_DIR.mkdir(parents=True, exist_ok=True)`

`def harvest_zenodo(community, size=200, delay=0.2):`
    `page, all_hits = 1, []`
    `while True:`
        `r = requests.get("https://zenodo.org/api/records",`
                         `params={"q": f"communities:{community}", "size": size, "page": page},`
                         `timeout=30)`
        `r.raise_for_status()`
        `hits = r.json().get("hits", {}).get("hits", [])`
        `if not hits: break`
        `for rec in hits:`
            `(RAW_DIR / f"{rec['id']}.json").write_text(json.dumps(rec, indent=2, ensure_ascii=False))`
            `all_hits.append(rec)`
        `page += 1`
        `time.sleep(delay)`
    `return all_hits`

`records = harvest_zenodo(COMMUNITY)`
`len(records)`
Cell #2
--------------------------------------
`from datetime import datetime`

`CONTEXT = {`
  `"@vocab": "http://purl.org/dc/terms/",`
  `"dc": "http://purl.org/dc/elements/1.1/",`
  `"dcterms": "http://purl.org/dc/terms/",`
  `"foaf": "http://xmlns.com/foaf/0.1/",`
  `"skos": "http://www.w3.org/2004/02/skos/core#",`
  `"prov": "http://www.w3.org/ns/prov#",`
  `"schema": "http://schema.org/",`
  `"ndc": "https://w3id.org/nfdicore#",`
  `"ids": "https://example.org/ids#"`
`}`

`def classify_types(rec):`
    `md = rec.get("metadata", {})`
    `types = ["ndc:Document"]`
    `ut = (md.get("upload_type") or "").lower()`
    `if ut == "software":`
        `types.append("ndc:Software")`
    `if ut == "dataset":`
        `types.append("ndc:InformationContentEntity")`
    `return types`

`def z_to_jsonld(rec, base="https://example.org/nfdi/zenodo/"):`
    `md = rec.get("metadata", {})`
    `rid = rec["id"]`
    `base_uri = f"{base}{rid}"`
    `doi = md.get("doi") or rec.get("links", {}).get("doi")`
    `rec_url = rec.get("links", {}).get("html")`
    `date = md.get("publication_date") or md.get("date")`

    `# creators`
    `person_nodes, creator_refs, org_nodes = [], [], []`
    `for cr in md.get("creators", []) or []:`
        `pname = cr.get("name")`
        `pid = f"{base_uri}/person/{abs(hash(pname))}"`
        `p = {"@id": pid, "@type": "foaf:Person", "foaf:name": pname}`
        `if cr.get("orcid"):`
            `p["ids:orcid"] = f"https://orcid.org/{cr['orcid'].strip()}"`
        `aff = cr.get("affiliation")`
        `if aff:`
            `oid = f"{base_uri}/org/{abs(hash(aff))}"`
            `p["schema:affiliation"] = {"@id": oid}`
            `org_nodes.append({"@id": oid, "@type": "foaf:Organization", "foaf:name": aff})`
        `person_nodes.append(p)`
        `creator_refs.append({"@id": pid})`

    `# subjects`
    `kw = (md.get("keywords") or [])`
    `sub_refs, concept_nodes = [], []`
    `for term in kw:`
        `cid = f"{base_uri}/concept/{abs(hash(term.lower()))}"`
        `sub_refs.append({"@id": cid})`
        `concept_nodes.append({"@id": cid, "@type": "skos:Concept", "skos:prefLabel": term})`

    `doc = {`
      `"@id": base_uri,`
      `"@type": classify_types(rec),`
      `"dc:title": md.get("title"),`
      `"dc:description": md.get("description"),`
      `"dcterms:identifier": [x for x in [doi, rec_url] if x],`
      `"dcterms:date": date,`
      `"dcterms:license": (md.get("license") or {}).get("id") or (md.get("license") or {}).get("url"),`
      `"dc:creator": creator_refs or None,`
      `"dc:subject": sub_refs or None`
    `}`

    `graph = [{"@context": CONTEXT}, doc] + person_nodes + org_nodes + concept_nodes`
    `def clean(n):` 
        `return {k:v for k,v in n.items() if v not in (None, [], {})}`
    `return [clean(n) for n in graph]`

`OUT_JLD = pathlib.Path("data/jsonld"); OUT_JLD.mkdir(parents=True, exist_ok=True)`

`for rec in records:`
    `jld = z_to_jsonld(rec)`
    `(OUT_JLD / f"{rec['id']}.jsonld").write_text(json.dumps(jld, indent=2, ensure_ascii=False))`

