**A Semantically Integrated Framework for Robotic Data Acquisition inMechanical Testing**
Eric Breitbarth (DLR)
- self driving lab
- robot arm follwoing crack to detect freckle pattern with a microscope
- real positions are gathered
- data automatically stored in a KG
- algorithmic data evaluation
- Ontology based knowledge praphs represent required context explicitly
- one experiment: ca. 5x10^6 triples
- just one SPARQL query to reconstruct the experiment (photo)
- exponential instead of linear development with experiment automation
- Q&A:
	- what's the advantage of using a KG? -> every data point can be retrieved together with all relations

**Automated Metadata Acquisition in Energy Research using BPMN-driven Workflows at the Energy Lab at KIT**
Jan Martin Reckel (KIT)
- energy research
- BPMN Business Process Model and Notation
- easy process design stored in XML
- maybe tool for #FAIRagroUC6 

**A Semantic Laboratory Assistant for Metadata Acquisition in Electronic
Lab Notebooks**
 Tina Boroukhian (hereon)
 - metadata are essential for reproducibility
 - LabFriend = ELN-agnostic semantic assistant
 - makes data-driven suggestions
 - uses ontologies and knowledge graphs
 - supports terminolgy harmonisation and validation
 - transform data from Chemotion Repo into KG compatible representation
 - from unstructured free text Chemotion data to validated KG
 - using SHACL for validation
 - KGs aligned with BFO and related ontolgies to support interoperability
 - Use KG data in LabFriend suggestion software to increase the automation of annotation and validation
 - Q&A:
	 - DMP useable as context? -> KG constructed from historical data
	 - can ISA standard for lab assays be mapped? -> we use provenance model, ISA probably not 
	 - Chemotion is running on schema.org, issues when moving to sth. BFO-based?
**A Collaborative Approach to Metadata Interoperability: PID4NFDI, TS4NFDI, and RSpace**
Tilo Mathes (RSpace)
- challenge: capturing metadata from the beginning
- same meaning different vocabularies -> lineage breaks (photo)
- three bridges (photo)![[IMG_7440.jpeg]]
- Aligning ELN fields with DataCite vocabularies and PIDs
	- handle PID sub-elements correctly
- TSS widgets at point of capture, Cocoda at export
- RSpace ecosystem: downstream use is facilitated
- DataCite realtion types to linked objects in RSpace for imporved PID metadata
- future: crosswalks to schema.org, DCAT, PROV 
- reusable integration pattern
- Q&A
	- crosswalk to ISA? -> ISA not ready for multifunctional assays
	- language to describe mappings? -> mappings between entities (entity schemas). SSM (sesame) LinkML 

**The Agentic Automation Canvas: A Metadata Framework for Human-AI Task Delegation**
Sebastian Lobentanzer (Helmholtz Munich)
- Meta study on AI Speedup *(photo)*
- inversion of control loop
- Clinical scribes: no great effect of RCTs
- reasons for overshooting expectations
- Simpson's Paradox
- How to bridge the gap?
	- Agentic Automation Canvas
	- web app: aac.slolab.ai
	- validating entry as you go
	- collecting use cases
- more of a social tool
```embed
title: " - The BioCypher Ecosystem"
image: "https://biocypher.org/assets/images/social/index.png"
description: ""
url: "https://biocypher.org"
favicon: ""
aspectRatio: "52.5"
```


**AIMWORKS: Template-Driven, Agentic Framework for FAIR Knowledge Graph Construction in Hydrogen Technologies**
Mohammad J. Eslamibidgoli (FZJ)
- AIMWORKS System Architecture (photo)
- Validation and Quality Assurance (photo)
- Performance Evaluation of LLMs (photo)
	- PROV-O for provenance
	- 

