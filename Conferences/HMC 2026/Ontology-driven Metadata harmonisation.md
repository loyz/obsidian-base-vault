**Local SDemantics with Global meaning**
- how should i choose the right ontology when in a domain without clear policies
- step by step approach: start with local ontologies; first create a simple local ontology and gradually develop a global ontolgy
	- upload to url
	- discoveries: EXPO, Dublin Core, ORCID ...
	- link your local ontolgy to standard terms
- Key to adoption is not a new technology but about what to tell humans
- RDF/OWL/SPARQL already provides the tools needed
**Interoperable Metadata for describing Health Studies**
- target data
	- individual health data from unselected patients & healthy subjects
	- from studies
	- from disease registries
- data uniqueness
- Data holding organisations (DHOs)
- recommendation how to make study data FAIR (see photo)
- ART-DECOR to model the metadata scheme
- Simplifier/HL7 publisher 
- Mapping to other Metadata Schemes:
	- Clinical trial registries
	- GHGA
	- ecrin
	- DataCite
	- ERDRI
- NFDI4Health Local Data Hub (LDH)
- nfdi4health.de/en/service/metadata-schema.html
**Integrating Domain Ontologies and Workflow Metadata for Interoperable
Computational Experiments**
- MaRDIbnTA2 /NFDI4Cat
- MaRDIflow lightweight workflow framework for the abstraction of FAIR CSE workfolws
- metadata documentation is enforced
- still prototype
```embed
title: "MaRDIFlow: A Workflow Framework for Documentation and Integration of FAIR Computational Experiments"
image: "https://zenodo.org/api/communities/e75094a1-a5cf-40a0-8668-108f1e88acbf/logo"
description: "MaRDIFlow, a cse workflow framework that abstracts the multi-layered components from FAIR computational experiments. This work is a part of Measure 4 (M4) in the Task Area 2 (TA2) of  the MaRDI (https://www.mardi4nfdi.de/about/mission) consortium. The design specification as well as the working prototype of our RDM tool is presented through different use cases. In the present version, MaRDIFlow acts a command-line tool such that it enables users to handle the workflow components as abstract objects described by input to output behavior. mardiflow_v1.0.0.tar.gz is a latest working prototype appended along a submitted manuscript, includes two use-cases as working examples.       "
url: "https://zenodo.org/records/10608764"
favicon: ""
aspectRatio: "100"
```

```embed
title: "MaRDIFlow: A CSE workflow framework for abstracting meta-data from FAIR computational experiments"
image: "https://arxiv.org/static/browse/0.3.4/images/arxiv-logo-fb.png"
description: "Numerical algorithms and computational tools are instrumental in navigating and addressing complex simulation and data processing tasks. The exponential growth of metadata and parameter-driven simulations has led to an increasing demand for automated workflows that can replicate computational experiments across platforms. In general, a computational workflow is defined as a sequential description for accomplishing a scientific objective, often described by tasks and their associated data dependencies. If characterized through input-output relation, workflow components can be structured to allow interchangeable utilization of individual tasks and their accompanying metadata. In the present work, we develop a novel computational framework, namely, MaRDIFlow, that focuses on the automation of abstracting meta-data embedded in an ontology of mathematical objects. This framework also effectively addresses the inherent execution and environmental dependencies by incorporating them into multi-layered descriptions. Additionally, we demonstrate a working prototype with example use cases and methodically integrate them into our workflow tool and data provenance framework. Furthermore, we show how to best apply the FAIR principles to computational workflows, such that abstracted components are Findable, Accessible, Interoperable, and Reusable in nature."
url: "https://arxiv.org/abs/2405.00028"
favicon: ""
aspectRatio: "58.333333333333336"
```
**MOLSIM: An Interoperable Ontology for Representing BiomolecularSimulation**
- Nature paper on implementation of FAIR in biomolecular simulations
- agnostic labeling 
- see photos
- development considerations
	- foundational taxonomy
	- subjective process that relies on sustained community consensus and efforts
	- LLM drafts definitions for expert validation and refinement

**Toward FAIR and Reproducible Data Quality Control: A Use Case–Driven
Data-Quality Processing Metadata Schema for Time Series Data**
- time-series data
	- NetCDF or CSV files
	- SensorThings API (STA) endpoints
- supporting
	- automated QC workflows
	- manual instpection steps
	- flagging schemas
	- reproducibility
- TERENO (Terrestrial Environmental Observations) &
- ACTRIS (Aerosol Clouds and Trace Gases Reserch Infrastructure)
	- Large scale
	- high quality data policies
	- How to represent QC information in the metadata?
	- data stream with obserations from OGC Sensor Things
- ```embed
title: "A General Schema for Time Series Data Quality Guided by Real-World Use Cases and Based on International Standards"
image: "https://zenodo.org/api/communities/436eab22-8269-4832-93d7-965884e34e67/logo"
description: "The World Wide Web Consortium (W3C) provides general best practices for including data quality information in data shared over the web. However, their implementation in practice often requires mapping or interpreting W3C concepts to the application domain. We report on a concrete approach to implementing the W3C Data Quality recommendations into time series data, thereby applying them to a wide range of scientific processes.  To that end, we propose a general schema for modeling data quality control information for time series data. The schema is guided by prominent use cases from the Earth and environmental sciences. It incorporates data quality flags, as well as processing information from automated quality control procedures and data inspections by domain experts. We provide a concrete implementation of the schema in the SensorThings API data model. Additionally, we demonstrate how file-based time series data can be annotated using the proposed schema in RO-Crates and the NetCDF format. By deeply integrating the W3C standard, we obtain a practice-oriented, semantically sound schema. We demonstrate the schema’s implementation for its initial use cases and provide additional relevant examples.    The proposed schema realizes quality control in the SensorThings API data model and for file-based time series data. Our approach preserves the original domain-specific structures while ensuring compliance with the W3C recommendations. Thus, we offer a straightforward plan to improve the readability and machine actionability of existing data quality information and corresponding workflows across domains. We even enable their interoperability on an international level."
url: "https://zenodo.org/records/19693929"
favicon: ""
aspectRatio: "38.734177215189874"
```
=> #FAIRagro #FAIRagroUC6 
