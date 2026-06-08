
Hier sind drei unterschiedlich fokussierte Vorschlagsversionen für den NFDI4Biodiversity Flexfund 2026. Jede Version betont einen anderen strategischen Schwerpunkt — von technischer Infrastruktur über kollaborative Transkription bis hin zur wissenschaftlichen Erkenntnisgewinnung.

---

# 🗂️ Proposal 1: Fokus auf Interoperabilität & Knowledge Graph

## Abstract *(ca. 200 Wörter)*

Historical phenological records represent an irreplaceable window into pre-industrial ecosystem dynamics — yet they remain largely inaccessible to modern biodiversity research due to fragmented storage, non-standardised vocabularies, and the absence of machine-readable formats. This project builds upon an existing phenological mapping tool developed in collaboration with German state archives, which has already enabled the transcription and analysis of approximately 8,000 observations from 30 species across 13 developmental stages in Upper Palatinate (1855/56). We now propose to transform this tool into a fully interoperable research infrastructure by embedding transcribed data into a structured **knowledge graph** compliant with established biodiversity standards (Darwin Core, OWL, RDF). A publicly accessible **SPARQL endpoint** will allow researchers across disciplines to query, compare, and reuse historical phenological data alongside modern datasets. Historic species names will be systematically aligned with current taxonomic nomenclature using controlled vocabularies. The resulting infrastructure will serve as a model for mobilising archival biodiversity data at scale, directly supporting the FAIR principles championed by NFDI4Biodiversity. By connecting historical Bavarian forestry records (1869–1871) with contemporary phenological observations, the project will demonstrate the scientific and infrastructural value of semantically enriched archival data for climate-sensitive biodiversity research. [2] [4]

---

## Status quo *(ca. 150 Wörter)*

A prototype phenological mapping tool has been developed within the NFDI4Earth Incubator programme, enabling the digitisation and structured analysis of historical phenological records from German state archives [1]. To date, approximately 8,000 observations covering 30 species and 13 developmental stages from Upper Palatinate (1855/56) have been transcribed. Additional records from Bavarian forestries (1869–1871) have been identified in the Bavarian State Archives and await processing. However, the current tool lacks semantic interoperability: data are not yet stored in a machine-readable linked-data format, historic species names are not systematically mapped to accepted taxonomic nomenclature, and no standardised export or query interface exists. This severely limits the reusability and discoverability of the data. The absence of a SPARQL endpoint or knowledge graph structure prevents integration with modern biodiversity databases and inhibits cross-institutional data sharing — a core requirement of the NFDI ecosystem. [3] [2]

---

## Aim *(ca. 150 Wörter)*

This project aims to transform the existing phenological mapping tool into a semantically interoperable research infrastructure. The core objective is the construction of a **RDF-based knowledge graph** that encodes transcribed phenological observations using established ontologies and biodiversity standards (Darwin Core, TDWG vocabularies). A **public SPARQL endpoint** will enable flexible, cross-dataset querying by researchers worldwide. Historic species names will be reconciled with current taxonomic nomenclature through automated matching against authoritative name registries. Data will be downloadable in interoperable formats (CSV, JSON-LD, RDF/Turtle). The project will demonstrate the infrastructure's value by integrating the newly transcribed Bavarian forestry records (1869–1871) and enabling their direct comparison with modern phenological datasets. This will serve as a replicable blueprint for mobilising further archival biodiversity data across German state archives, in direct alignment with NFDI4Biodiversity's mission to improve the availability and usability of research data according to FAIR principles. [2] [4] [3]

---
---

# 🤝 Proposal 2: Fokus auf KI-gestützte kollaborative Transkriptionsplattform

## Abstract *(ca. 200 Wörter)*

Millions of historical biodiversity observations lie dormant in European archives, locked in handwritten records that resist automated processing without human validation. This project proposes the development of a **collaborative, AI-assisted transcription platform** for historical phenological records, building on an existing tool developed within the NFDI4Earth Incubator programme. The platform will employ machine learning models to pre-process and pre-annotate scanned archival documents, generating transcription suggestions that registered users — researchers, students, and citizen scientists — can review, correct, and validate. Crucially, all validated corrections will feed back into the training pipeline, enabling continuous improvement of transcription accuracy through **active learning**. The platform will incorporate standardised vocabularies to resolve historic species names into current taxonomic nomenclature and will support structured data entry aligned with Darwin Core standards. Starting with approximately 8,000 already-transcribed observations from Upper Palatinate (1855/56) as a validated training corpus, the platform will be applied to newly discovered Bavarian forestry records (1869–1871). The project directly addresses the bottleneck between archival richness and scientific accessibility, creating a scalable, community-driven infrastructure for biodiversity data mobilisation that aligns with NFDI4Biodiversity's FAIR data objectives. [3] [1] [2]

---

## Status quo *(ca. 150 Wörter)*

The phenological mapping tool developed in the NFDI4Earth Incubator has demonstrated the feasibility of digitising and structuring historical phenological records from German state archives [1]. Around 8,000 observations from Upper Palatinate (1855/56) have been manually transcribed, covering 30 species and 13 developmental stages. While this corpus proves the scientific potential of archival phenological data, the current transcription workflow is entirely manual — time-consuming, error-prone, and not scalable to the volume of records identified in Bavarian state archives. No AI-assisted pre-annotation or collaborative validation workflow currently exists within the tool. User contributions are not systematically captured as training data. Furthermore, the platform does not yet support community participation beyond the immediate project team, limiting the speed and scale at which new archival material can be mobilised. This represents a critical bottleneck given the volume of unprocessed records from Bavarian forestries covering 1869–1871. [3] [2]

---

## Aim *(ca. 150 Wörter)*

The central aim is to develop a **scalable, AI-assisted collaborative transcription platform** that lowers the barrier to mobilising historical phenological records. An integrated machine learning pipeline will generate pre-filled transcription suggestions from scanned archival documents; human users will validate and correct these suggestions through an intuitive web interface. All validated inputs will be recycled as labelled training data, enabling the model to improve iteratively with each transcription cycle. The platform will enforce standardised data entry (Darwin Core, controlled species vocabularies) to ensure immediate interoperability of all transcribed records. Gamification elements and structured onboarding will encourage participation from citizen scientists and students alongside professional researchers. The existing Upper Palatinate corpus (1855/56) will serve as the initial training dataset, and the platform will be deployed on the Bavarian forestry records (1869–1871) as a first real-world application. Workshops will introduce the platform to the broader NFDI4Biodiversity community. [2] [3] [4]

---
---

# 🔬 Proposal 3: Fokus auf wissenschaftlichen Output & Datenlücken in Bayern

## Abstract *(ca. 200 Wörter)*

Long-term phenological datasets are among the most powerful tools available for detecting and quantifying the biological impacts of climate change — yet the 19th century, a period of critical baseline significance, remains severely underrepresented in digitised biodiversity records for Bavaria and much of Central Europe. This project will close a concrete temporal and geographic gap by transcribing, standardising, and scientifically evaluating historical phenological records from Bavarian state archives, covering the years 1855/56 (Upper Palatinate) and 1869–1871 (Bavarian forestries). Building on an existing transcription tool developed within the NFDI4Earth Incubator, the project will produce a **scientifically validated, FAIR-compliant phenological dataset** spanning multiple Bavarian regions and decades. In collaboration with the Chair of Eco-Climatology at TU Munich (Letter of Commitment pending), the dataset will be used to address a focused research question on phenological shifts in tree species across the 19th century and their relationship to climate variability. Results will be published in a peer-reviewed journal, demonstrating the scientific value of archival phenological data for climate-sensitive biodiversity research and for training phenological prediction models. [3] [2] [4]

---

## Status quo *(ca. 150 Wörter)*

Phenological observations from the 19th century are of exceptional scientific value as pre-industrial baselines for climate impact research, yet they are rarely available in digitised, standardised form [3]. Within the NFDI4Earth Incubator, a phenological mapping tool was developed that enabled the transcription of approximately 8,000 observations from Upper Palatinate (1855/56), covering 30 species and 13 developmental stages [1]. Additionally, previously unknown phenological records from Bavarian forestries (1869–1871) have been identified in the Bavarian State Archives. However, these datasets have not yet been scientifically evaluated: historic species names remain unresolved against current nomenclature, records do not conform to modern data standards, and no domain-expert collaboration has been formalised. The data are therefore not yet suitable for publication or integration into comparative phenological analyses. A collaboration with the Chair of Eco-Climatology at TU Munich is being pursued to provide the necessary scientific expertise. [2] [3]

---

## Aim *(ca. 150 Wörter)*

This project aims to produce a **peer-reviewed scientific publication** based on newly transcribed and standardised Bavarian phenological records from the 19th century, demonstrating the value of archival data for climate-sensitive biodiversity research. The specific research question — to be refined following an Elicit literature review — will focus on detectable phenological shifts in Bavarian tree and plant species between 1855 and 1871 and their correlation with documented climate variability of the period. All records will be standardised against Darwin Core and current taxonomic nomenclature, and published as an open, FAIR-compliant dataset. The transcription tool will be enhanced to support this workflow, including automated name matching and structured export. Domain expertise will be contributed by the Chair of Eco-Climatology at TU Munich (LoC in preparation). The resulting dataset will serve as a replicable model for filling 19th-century phenological data gaps across Bavaria and beyond. [2] [3] [4]

---

## 📚 Quellen

| ID | Quelle |
|----|--------|
| [1] | NFDI4Earth Incubator – Phenological Mapping Tool (2024): [nfdi4earth.de](https://nfdi4earth.de/images/20241030_nfdi4earth_incubator_phenomapping.pdf) |
| [2] | NFDI4Biodiversity – Flexfunds Call 2025: [nfdi4biodiversity.org](https://www.nfdi4biodiversity.org/en/news/flexfunds-call-2025/) |
| [3] | PMC – *The written history of plant phenology: shaping primary data* (2023): [pmc.ncbi.nlm.nih.gov](https://pmc.ncbi.nlm.nih.gov/articles/PMC10326116/) |
| [4] | ResearchGate – *iKNOW: A platform for knowledge graph construction for biodiversity* (2022): [researchgate.net](https://www.researchgate.net/publication/362877185_iKNOW_A_platform_for_knowledge_graph_construction_for_biodiversity) |

---

**Nächster Schritt:** Für Proposal 3 empfehle ich folgende Elicit-Suchanfrage, die du direkt einspeisen kannst:

> *"What is the scientific value of 19th-century phenological records for detecting climate-driven shifts in plant and tree phenology in Central Europe, and how have such records been used to train or validate phenological prediction models?"*

