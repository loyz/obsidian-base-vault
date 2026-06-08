**Data Quality Assessment (DQA)**
- data quality requirements must be explicit
- Input clinical data (fever temp), input metadata enrich before Output and CDSS
- Rules behind it, sometimes embedded in code
	- probability of a certain response
	- starting from formal data quality framework, rules expresse in a non techical manner
	- DQ Grading: if it's a problem is context sensitive
		- seperate expectations, requirements, .. from coding
	- Data quality is really difficult notion
		- foundational = how good are measurements?
		- intrinsic 
		- question specific
		- integrate DQ concept, indicator rules, Gradning rules, DQ results
		- DQ is only partially maesurable
		- there is no standard; it's total chaos
		- Data quality vocabulary? can show quality through different quality concepts
**Self-assessment for FAIR data publication**

- Curation @KU Leuven
- autochecks but still manual is necessary
- issues often surface only during curation
- check my datset tool
- check if tool can be integrated into Dataverse pipeline
- is it necessary to archive all the data? no, think what is reasonable
**Ontology/Driven FAIR Sensor Maintenance Metadata**
- maintenance is essential context for sensor data quality 
- how can it be made FAIR by design?
- collect in semantically annotated way
- Reused ontologies: SOSA, SSN; PROV-O; P-PLAN; => MOIN ontology => MOIN4BokisEck, Moin4Tesperhude (for specific use cases)
- Ontolgy-driven forms with SHACL
- closing the interoperability loop:
	- Herbie queried via SPARQL
	- ...
	- publishing to O2A registry
- MOIN4Herbie makes sensor maintenance metadata FAIR
- ```embed
title: "MOIN4Herbie / MOIN4Herbie public access · GitLab"
image: "https://codebase.helmholtz.cloud/assets/twitter_card-570ddb06edf56a2312253c5872489847a0f385112ddbcd71ccfa1570febab5d2.jpg"
description: "Helmholtz Codebase - GitLab"
url: "https://codebase.helmholtz.cloud/moin4herbie/moin4herbie-public"
favicon: ""
aspectRatio: "100"
```

**FAIR AIMS bringing rich metadata for phzsical samples into the digital world**
- Open samples in ESS, hybrid, granular; solution for the long tail
- How to connect samples with research data and publications?
- IGSN 
- FAIR WISH project (for Helmholtz association)
- registered 15k IGSNs with workflow
- FAIR AIMS: Automated IGSN Management System not only for ESS but also matter domain
- IGSN Metadata levels
- aligned with DataCite Schema, but developed in different directions
- => IGSN Metadata Schema 2.0; many DataCite elements can be included in IGSN Schema
	- IGSN  Core Schema (DataCite plus common kernel)
	- IGSN Supplementary Schemata for different sample classes
**From Siloed Experiments to ...**
- datin AI infrastructure for R&D
- Glossaries
-  construct KG
- FAIR Data Foundation (FAIR is requirement)
- KG is far more efficient for searching
- prerequisite for automated manifacturing
- public release in some month expected
**Open Data, Open Access, THOTH Open Metadata**
- journals -> <JATS> <TEI>
- https://thoth.pub
- https://zenodo.org/records/18173982
- github.com/thoth-pub/
- put your book in and generate all metadata for all platforms: MARC, ONIX, KBART, Crossref XML
- showcase of open data workflows in the context of OA book publishing: https://zenodo.org/records/17340814
- small publishers can excel on Springer Press etc.
- support initiative via OpenBookCollective




