---
abstract: 'This report examines how governmental data can be made more accessible

  and usable for research in Earth System Science (ESS) by applying the

  FAIR principles --- Findable, Accessible, Interoperable, and Reusable.

  Using High-Value Datasets (HVD) defined under Implementing Regulation

  (EU) 2023/138 (DVO-HVD) as a pilot case, it analyses workflows,

  standards, and infrastructures that support discoverability and

  reporting.


  HVD---such as national-scale climate, hydrology, and land-use

  datasets---must be published as Open Data, tagged in metadata, and

  reported at the Member State level. Their stringent requirements expose

  gaps in metadata quality, harvesting consistency, and cataloguing,

  making them ideal for testing improvements.


  The report focuses on three key questions: how agencies can improve the

  way, they publish datasets; how ESS scientists can effectively find and

  access them; and what is needed for a sustainable, end-to-end data

  pipeline. It reviews the legal context (PSI Directive, DVO-HVD, DNG,

  GeoZG) and infrastructures including GDI-DE, GovData, umwelt.info, and

  NFDI4Earth (OneStop4All/KnowledgeHub). Findings highlight the need for

  harmonised metadata, semantic search, stronger feedback channels, and

  richer documentation.


  Without claiming to propose complete technical solutions, the report

  provides a roadmap for strengthening data infrastructures to serve both

  governmental agencies and the scientific community. It shows how HVD can

  act as a catalyst for broader, FAIR-aligned improvements.

  '
author:
- email: astrid.ziemann@tu-dresden.de
  name: Astrid Ziemann
  orcid: 0000-0002-6686-3736
- name: Alois Georg Wieshuber
  orcid: 0009-0001-7010-7968
- name: Tim Schürmann
  orcid: 0009-0009-4778-5902
- name: Stefan Krämer
- name: Maximilian Berthold
  orcid: 0000-0003-1985-6426
- name: Frank Kratzenstein
date: 2025-09
doi: 10.5281/zenodo.17553005
figPrefix: Fig.
identifier: D2.3.1
include-before: '\section*{Call for review}

  This document is intended to be updated regularly. We invite you to actively contribute
  by providing feedback, particularly on missing data or information relevant to researchers
  in the OneStop4All portal of NFDI4Earth. Your input will help improve this report
  and ensure it meets the needs of the research community. Please send your comments
  to the NFDI4Earth [User Support Network contact form](<http://onestop4all.nfdi4earth.de/?support>):
  <https://onestop4all.nfdi4earth.de/>.

  \newpage

  \section*{Abbreviations}

  Accessibility / Accessible (FAIR): In the context of FAIR, the property that (meta)data can be retrieved by humans and machines via standardised protocols, with clear access conditions (including authentication/authorisation).

  Aggregator / metadata aggregator: A service that collects metadata from multiple providers. Often it includes harmonisationn and quality-assessment. Collected data are usually made available via APIs for redistribution to downstream portals and catalogues and for harvesting.

  API: Application Programming Interface.

  ATOM Feed: Refers to the Atom Syndication Format (ASF), an XML standard used for web feeds. In ESS this IETF registered standard is also used for structured download of geodata tiles.

  BGR (Bundesanstalt für Geologie und Rohstoffe): Federal Institute for Geology and Natural Resources

  BSH (Bundesamt für Seeschifffahrt und Hydrographie): Federal Maritime and Hydrographic Agency

  BKG (Bundesamt für Kartographie und Geodäsie): Federal Agency for Cartography and Geodesy

  BDSG (Bundesdatenschutzgesetz): Federal Data Protection Act

  CSW: Catalogue Service for the Web

  Catalog / catalogue (metadata catalogue): Structured collection of metadata records describing datasets and services, usually searchable via a web interface and/or an API.

  CKAN (Comprehensive Knowledge Archive Network): Software used by the GovData catalogue and by other national and regional government organisations in the EU.

  Controlled vocabulary: A curated set of standardised terms (often with identifiers) used in metadata to ensure consistent tagging. This in turn makes targeted search more efficient.

  CSW (Catalogue Service for the Web): OGC standard for publishing and querying geospatial metadata catalogues; a CSW  interface is commonly used for harvesting ISO-based metadata.

  DCAT: Data Catalog Vocabulary. A W3C vocabulary (RDF-based) for describing datasets and data services in catalogues.

  DCAT-AP: Data Catalog Vocabulary Application Profile. It specifies required fields and conventions for interoperable metadata exchange. There is a german derivative (DCAT-AP.de) of the European standard (see below).

  DCAT-AP.de: German derivative of the DCAT application profile, that is used by the GovData portal for the exchange of adminatrarive open data. It is curated by the FITKO.

  Destatis (Statistisches Bundesamt): Federal Statistical Office

  DNG (Datennutzungsgesetz): Data Use Act

  DSGVO: Datenschutzgrundverordnung -> GDPR

  DVO-HVD (Durchführungsverordnung High-Value Datasets): EU implementing regulation defining High-Value Dataset categories and publication/reporting requirements.

  DWD (Deutscher Wetterdienst): German Weather Service

  ESS: Earth System Science

  EU: European Union

  EU-HVD: European High-Value Dataset Act

  FAIR principles (Findable, Accessible, Interoperable, Reusable): Guiding principles designed to improve (meta)data management and stewardship, making data more fit for its scientific purpose. First formulated in a 2016 *Scientific Data* article, the principles have given rise to the GoFAIR initiative and have since been adopted by numerous other RDA initiatives around the world, including the NFDI.

  Findable (FAIR): FAIR property that data and metadata can be discovered via searchable metadata, stable identifiers, and indexing.

  FITKO (Föderale IT-Kooperation):  The IT Planning Council´s Federal IT Cooperation is an organisation that coordinates the targeted digitalisation of the German public administration (federal, state and local government).

  GDI (Geodateninfrastruktur): Geodata Infrastructure. A coordinated framework of standards, services, and organisations enabling interoperable discovery and access to geospatial data (used e.g., for GDI-DE and state-level SDIs).

  GDI-DE: Geodateninfrastrukur Deutschland / German Spatial Data Infrastructure. See the report for a detailed description.

  GDPR: General Data Protection Regulation

  Geodata / geospatial data: Data with explicit spatial reference.

  GeoZG (Geodatenzugangsgesetz): Geodata Access Act

  gov-agencies: governmental agencies

  gov-data: governmental data

  Harvesting: Automated retrieval of meta(data) from source catalogues/endpoints into an aggregator or portal, typically scheduled and repeated.

  HVD: High-Value Datasets

  INSPIRE (Infrastructure for Spatial Information in the European Community): EU framework (Directive) and associated technical rules for harmonised spatial data and metadata; referenced as ISO 191\*-based XML metadata implemented in Germany through GDI-DE.

  Interoperable / interoperability (FAIR): FAIR property that (meta)data can be integrated across systems and domains, typically via shared standards, formats, and semantics (including controlled vocabularies).

  ISO: International Organization for Standardization

  ISO 191\* suite: Suite of standards for geospacial data with ISO 19115-1 as its core. ISO 19139 defines a XML schema for gegraphic metadata derived from ISO 19115.

  IWG: Informationsweiterverwendungsgesetz

  JSON (JavaScript Object Notation): Format for file and data exchange. Specivically suited for exchanging metadata.

  JSON-LD (JavaScript Object Notation for Linked Data): A JSON serialisation for linked data, derived from recommendations of the W3C´s recommendations for embedding data in the globally linked RDF model in a lightweight JSON format.

  Keyword (metadata keyword): A term used in metadata for search and filtering; the report highlights problems when keywords are inconsistent (e.g., case sensitivity) or not linked to controlled vocabularies.

  Landes-GDI (Landesgeodateninfrastrukturgesetze): Spatial data infrastructure and geospatial regulations in Germany.

  LDSG (Landesdatenschutzgesetze): State Data Protection Acts

  Machine-readable: A form and access method that software can process automatically (structured formats, standardised interfaces), required for HVD publication and FAIR-aligned workflows.

  Metadata: Data about data. In our context: Structured descriptive information about datasets/services (e.g., title, abstract, licence, spatial/temporal coverage, access links) enabling discovery and assessment for use.

  Metadata quality: The degree to which metadata are complete, correct, consistent, standard-conformant, and sufficiently rich for reliable discovery and reuse.

  Monitoring: Systematic checking and metrics on metadata availability and conformance (e.g., within the GDI-DE Monitor) to support quality assurance and reporting.

  NFDI (Nationale Forschungsdateninfrastruktur): National Research Data Infrastructure. A German initiative founded in 2020 to improve the national research data infrastructure, financed by a Bund-Länder agreement.

  NGO: Non-Governmental Organization

  OGC: Open Geospatial Consortium

  OGC standards: Standards from the Open Geospatial Consortium referenced for interoperable geodata services and catalogues (e.g., CSW, WFS).

  Open Data: Data made available for reuse with minimal legal and technical restrictions in accordance with the Open Definition [https://opendefinition.org/]. Open Government Data refers to all data wich is produced and paid for by public bodies and made freely available for any purpose.

  Open.NRW (Open Government in Nordrhein-Westfalen): Information and open data portal of the state government of North Rhine-Westphalia.

  Portal: A user-facing service that supports search and access to metadata and links to datasets (e.g., GovData, Geoportal, OneStop4All, umwelt.info).

  PSI Directive (EU) 2019/1024 / Open Data Directive: EU directive that is the legal basis for reuse of public sector information; the HVD regulation is a focused extension of this directive for especially valuable datasets.

  RDF: Resource Description Framework

  SDI: Spatial data infrastructure

  Semantic search: An advanced search and retrieval method enhanced by semantics. Rather than relying on literal keyword matching semantic methods aid in understanding user intent and context by making use of synonyms, controlled vocabularies, ontologies and mappings between vocaburlaries. Semantics reduce keyword-dependency in discovery.

  SPARQL query / SPARQL endpoint: SPARQL is a recursive acronym, that stands for `SPARQL Protocol and RDF Query language´. It is a semantic, SQL-like query language used to retrieve, manipulate and analyse RDF data. It enables complex queries to be performed across diverse linked datasets. A SPARQL endpoint is a web-based service interface for RDF data that accepts SPARQL queries via HTTP. Endpoints can be used either programmatically or via a graphical user interface.

  Thesaurus: A referenced controlled vocabulary source for keywords.

  Turtle: Terse RDF Triple Language (Syntax und Datenformat für RDF)

  UBA (Umweltbundesamt): Federal Environment Agency

  URI: Uniform Resource Identifier. A (unique) string of characters used to unambiguously reference resources and concepts on the internet.


  W3C: World Wide Web Consortium

  WFS: Web Feature Service. An OGC standard for accessing vector geospatial features via web services.

  '
include-preamble: '\interfootnotelinepenalty=10000 \clubpenalty=1000 \widowpenalty=1000 '
keywords:
- NFDI
- NFDI4Earth
- NFDI4Earth Deliverable
- HVD
- GovData
- GDI-DE
- metadata
lang: en-GB
link-citations: 'true'
lof: 'true'
lot: 'true'
subtitle: Availability of Government Data for Research Purposes
tblPrefix: Tab.
title: Report on data made available for research by governmental authorities
toc: 'true'
version: '1.0'
---

# Introduction

This report, titled **"Report on Data Made Available for Research by
Governmental Authorities,"** aims to improve access to governmental
data (gov-data) in alignment with the FAIR principles[^1] --- Findable,
Accessible, Interoperable, and Reusable. It is targeted at scientists
and data-providing authorities in the field of Earth System Science
(ESS) and outlines a process-oriented approach to enhance the
discoverability and usability of gov-data.

To support this goal, we focus on High-Value Datasets (HVD), using a
defined and delimitable dataset as a practical entry point. HVD
represent standardised, high-quality inputs (e.g., climate, hydrology,
land use data) that underpin Earth system models and analyses; improving
their discoverability directly benefits the ESS community. Under
Implementing Regulation (EU) 2023/138 ("DVO-HVD")[^2], HVD are
public-sector geospatial datasets that:

- Are listed in the Annex to the DVO-HVD (six thematic categories):

  - Geospatial

  - Earth observation and environment

  - Meteorological

  - Statistics

  - Mobility

  - Company and business registers

- Are provided in machine-readable form at all generalization levels
    down to 1:5 000, and

- Collectively cover the entire territory of an EU Member State.

In Germany, meteorological HVD (e.g., station observations, validated
climate series) are provided by the Deutscher Wetterdienst (DWD), while
other authorities may contribute additional datasets.

HVD must be published as **Open Data**, marked in metadata, and included
in national reporting. Their demanding scope exposes shortcomings in
harvesting, metadata quality, and cataloguing---making them ideal pilots
for pipeline improvement.

The report addresses three guiding questions:

- How can governmental agencies make their datasets discoverable for
    the scientific community?

- How can ESS scientists effectively locate and access these datasets?

- What steps are needed for a sustainable, end-to-end data pipeline?

In examining these questions, the report references established
standards and frameworks. Relevant metadata frameworks include:

- **INSPIRE**[^3] -- ISO 191\*-based XML metadata for geospatial data,
    implemented in Germany by GDI-DE.

- **G8 Open Data Charter**[^4] -- DCAT AP (JSON) metadata, implemented
    nationwide by GovData.

- **EU-HVD**[^5] -- DCAT AP-based publication of HVD, with GDI-DE
    supplying records and GovData providing metadata.

To enable comprehensive data discovery, the report also considers
existing infrastructures such as the **Geodateninfrastruktur Deutschland
(GDI-DE**[^6]**)**, **GovData**[^7]---the German national data
portal---and **UBA** **umwelt.info**[^8]. All three platforms already
apply DCAT-based metadata and represent key components in the evolving
HVD ecosystem. Furthermore, the report incorporates perspectives from
the **NFDI4Earth**[^9] initiative, particularly its
**KnowledgeHub**[^10] and the **OneStop4All portal**[^11], which aim to
streamline metadata aggregation and improve data discoverability.

However, simply listing datasets in catalogs is insufficient; effective
discovery requires both metadata and datasets to be jointly accessible
and contextually relevant. The report therefore considers semantic
filters and other enhancements informed by EU HVD guidelines to enable
structured, interoperable searches.

Rather than prescribing fully developed technical solutions, the report
proposes a pathway toward more robust, FAIR-aligned data infrastructures
for ESS, identifying requirements, open issues, and promising strategies
for sustained improvement.

# Legal and Infrastructural Foundations for Governmental and HVD Metadata

## Legal framework for governmental data

In June 2024, the EU High-Value Dataset (HVD) Implementing Regulation
entered into force. This regulation (EU) 2023/138[^12] defines a list of
categories of high-value datasets that must be made available for free
re-use by governmental authorities across all EU member states. As
stated in the regulation, its goal is "to ensure that public data of
highest socio-economic potential are made available for re-use with
minimal legal and technical restrictions and free of charge."[^13]

In Germany, the INSPIRE Directive is primarily implemented through the
Geodata Access Act (GeoZG[^14]), which establishes national regulations
for geospatial interoperability and access. At state level,
complementary spatial data infrastructure and geospatial regulations
(Landes-GDI) refine responsibilities and technical specifications,
ensuring INSPIRE standards are operationalised across state
administrations.

Already in 2007, the EU launched the INSPIRE initiative to support "the
purposes of Community environmental policies and policies or activities
which may have an impact on the environment"[^15] This initiative aimed
to build a common EU-wide infrastructure for geospatial data, setting
essential standards for data interoperability and accessibility. INSPIRE
laid the groundwork for harmonizing environmental and geospatial data
across Europe.

Over time, research and practical experience demonstrated that public
sector data serves citizens, researchers, and businesses best when it is
openly accessible. This realisation led to the EU\'s Open Data
Initiative and the adoption of the PSI Directive (EU) 2019/1024[^16],
which sought to make public sector information more widely usable by
science and the economy. However, to sharpen the focus on datasets with
the highest potential societal benefits, the HVD regulation was
introduced.

The HVD regulation builds on the principles of the PSI Directive (EU)
2019/1024, specifying categories like geospatial, meteorological, and
environmental data as high-value datasets. These datasets are seen as
key drivers for innovation, economic growth, and societal progress. They
may be expanded in future to reflect scientific and technological
progress. In Germany, the regulation was first implemented through
updates to the Informationsweiterverwendungsgesetz (IWG)[^17] which
adopted the earlier EU directive 2003/98/EG[^18]. When this directive
became substituted by 2019/1024 the IWG became an update and was
replaced by the new Datennutzungsgesetz (DNG)[^19] in 2021, ensuring
compliance with EU requirements. The DNG expanded data categories,
emphasized FAIR principles, and reduced restrictions. The development
reflects growing awareness of data\'s socio-economic value and the need
for harmonized, accessible, and innovation-driven data policies in the
digital age.

In parallel with the regulations on open data and high-value datasets,
the General Data Protection Regulation (GDPR/DSGVO[^20]) is implemented
in Germany through the Federal Data Protection Act (BDSG), which is
supplemented by State Data Protection Acts (LDSG). Similarly,
state-level Freedom of Information and Open Data laws implement and
extend the obligations and reuse measures introduced by the
Datennutzungsgesetz (DNG) for subnational public bodies.

The GDI-DE plays a central role in coordinating the provision and
accessibility of these datasets. The structured provision pathway
outlined in the regulatory framework involves federal, state and local
authorities consolidating and standardising data sets in accordance with
their obligations under the BDSG/LDSG (data protection),
GeoZG/Landes-GDI (geodata) and DNG (open data), before forwarding them
to the GDI-DE. This multi-layered compliance and technical consolidation
enable the scientific community at large to reuse the data.

Looking ahead, the EU plans to expand the list of high-value datasets
and further improve interoperability standards. In Germany, efforts will
likely focus on increasing the usability of these datasets for research
and industry while integrating them with emerging technologies like
artificial intelligence. Strengthening collaborations between public
authorities, academia, and private enterprises is expected to maximize
the societal and economic benefits of open data.

Future expansions to the list of high-value datasets will likely require
coordinated adjustments to federal (DNG, GeoZG and BDSG) and state
(Landes-GDI and LDSG) frameworks. This will ensure consistent
interpretations for operational agencies, enabling datasets to reach
infrastructures such as GDI-DE with both legal conformity and technical
interoperability.

NFDI4Earth is committed to improving the availability, accessibility,
findability, and quality of high-value datasets by leveraging the NFDI
infrastructure and adhering to FAIR principles (Findable, Accessible,
Interoperable, Reusable). Its mission is to ensure that Earth system
data is open, standardized, and efficiently reusable, thereby supporting
the EU\'s goals for high-value datasets and fostering innovation across
science and society.

![Connection between legal requirements for governmental data
and responsible authorities](./figure1.png){width="6.270833333333333in"
height="3.657985564304462in" #fig:connection-legal-requirements}

## Governmental metadata host -- aggregator

A **metadata aggregator** is a service provider that collects,
harmonizes, manages, preserves, and redistributes metadata from multiple
sources. Aggregators serve as organisational and technical
intermediaries between data-providing institutions (data providers) and
downstream systems such as portals or APIs.

Typical responsibilities of an aggregator include:

- Harvesting metadata from various source systems on a regular basis,

- Transforming and standardizing metadata according to overarching
    frameworks (e.g., DCAT-AP),

- Managing persistent access points, interfaces, and data quality
    assurance mechanisms,

- Forwarding harmonized metadata to central or supranational data
    portals

A prominent example is **GovData**[^21], which harvests metadata from
sources such as **GDI-DE**[^22] (Germany's Spatial Data Infrastructure)
and **Destatis**[^23] (the Federal Statistical Office). GDI-DE itself
acts as an aggregator by collecting metadata from institutions such as
the **German Weather Service (DWD)**, the **Federal Institute for
Geosciences and Natural Resources (BGR)**, and **federal state-level
geodata infrastructures**.

A **metadata host** is a service provider responsible for storing
digital objects and their associated metadata. The hosting function
includes:

- Capturing and maintaining metadata records,

- Presenting datasets and metadata through user-facing interfaces
    (e.g., web portals, map viewers),

- Providing machine-readable access via standardized APIs and
    protocols (e.g., CSW, WFS, SPARQL endpoints).

In addition to infrastructure, hosts often provide tools for metadata
creation, validation, and version management, thereby supporting
long-term usability and compliance with metadata standards.

The integration of aggregation and hosting capabilities within a single
entity can be highly beneficial for:

- Ensuring consistent data quality through harmonized metadata
    handling,

- Providing stable and reliable access paths to metadata and datasets,

- Simplifying communication channels with both data providers and
    downstream consumers (e.g., research platforms or public data
    portals).

For example, **GDI-DE** acts as both a metadata host and aggregator for
numerous federal agencies, whereas **GovData** mainly focuses on
centralized aggregation and metadata distribution. Similarly,
**umwelt.info** operates as a thematic host and aggregator within the
environmental data sector.
See the overview in [@tbl:overview].

\scriptsize

  **Aggregator**   **Metadata Providers**                                                             **Interface/Standard**
  ---------------- ---------------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------
  GDI-DE           DWD, BGR, BKG, federal state infrastructures                                       INSPIRE-compliant CSW, ATOM Feed
  GovData          GDI-DE, Destatis, etc.                                                             DCAT-AP-DE (JSON / RDF)
  umwelt.info      Authorities (federal, state, local) like BfG, BAW, BGR, GdWS, BSH, DESTATIS etc.   Several kinds of interfaces, a lot of sources INSPIRE-compliant, internal metadata schema and CKAN-based API

: Overview to focused Aggregators, Metadata providers (governmental authorities) and Interfaces/ tandards for governmental data in Germany {#tbl:overview}

\normalsize

Whether an aggregator, especially the GDI-DE, accepts and integrates
metadata from a given source depends on several key criteria (*please
note*, that none of these criteria is obligatory to be scraped or
harvested by umwelt.info):

- **Standard Compliance:** Metadata must conform to established
    schemas such as [DCAT-AP-DE](https://www.dcat-ap.de) or the [INSPIRE
    Metadata Regulation](https://inspire.ec.europa.eu/metadata).

- **Machine-Readable Access:** Metadata must be available through open
    and standardized interfaces (e.g., CSW, SPARQL, REST APIs, ATOM
    feeds).

- **Persistence and Availability:** The metadata service must be
    consistently available, version-controlled, and technically
    reliable.

- **Licensing and Openness:** Metadata must include clear licensing
    terms (e.g., Data License Germany) that permit reuse in open data
    contexts.

- **Relevance and Currency:** The harvested metadata should be updated
    regularly and refer to publicly accessible, relevant datasets.

A sustainable and scalable research data infrastructure relies on
**well-structured hosting and aggregation services**. Only through
professional metadata management can governmental data become truly
**FAIR** for the ESS community and the public alike.

Building on the overview of data aggregators presented in this chapter,
the following sub-sections provide a closer look at key
infrastructures---GDI-DE, GovData, and umwelt.info---as well as the
NFDI4Earth initiative. These platforms illustrate how metadata
aggregation and discoverability are implemented in practice.

*Please note*, that in the **HVD infrastructure**[^24], there is no
keyword "HVD" itself. Instead, **thematic designations** (e.g.,
"Meteorology") are used as **keywords from a controlled vocabulary**,
including the specification of the respective **thesaurus**. The
challenges and opportunities outlined below serve to raise awareness
within the research community, helping researchers understand why
certain data may not yet be discoverable and how these insights can
inform their own work on data and metadata. Researchers are invited to
actively contribute to the further development of this report and to
provide feedback via the **User Support Network**[^25] **of
NFDI4Earth**.

### GDI-DE

The Geodateninfrastruktur Deutschland (GDI-DE) is a joint initiative of
the Federal Government, the 16 federal states and municipal associations
to make their spatial data interoperable and easily accessible online.
It implements the EU INSPIRE Directive (2007/2/EC)[^26] by providing
central technical components---Geoportal.de[^27],
Geodatenkatalog.de[^28], Registry[^29], Testsuite[^30] and
Monitor[^31]---that allow users to search, view, download and interlink
geospatial datasets from all administrative levels.

GDI-DE's mission is to support science, administration, economy and the
public by ensuring that distributed geodata (topographic, thematic,
environmental, cadastral) conform to open OGC/ISO standards and FAIR
principles. It thereby fosters cross-border and cross-sectoral
collaboration in policy-making, research and applications.[^32]

The Coordination Office (Koordinierungsstelle) GDI-DE at the Federal
Agency for Cartography and Geodesy (BKG) in Frankfurt am Main acts as
Germany's National INSPIRE Point of Contact. It:

- Advises the Steering Committee (Lenkungsgremium GDI-DE) on INSPIRE
    implementation[^33]

- Represents Germany in EU INSPIRE Working Groups and liaises with the
    European Commission

- Develops GDI-DE concepts, guidelines and best practices for
    metadata, services and data harmonisation.

#### GDI-DE monitoring metrics

The GDI-DE Monitor is the national quality-assurance tool for checking
availability and conformance of all metadata in the GDI-DE. As of the
latest harvesting cycle (28.08.2025):

- 747 295 metadata records have been harvested into the Monitor

- 349 503 of these records are identified as INSPIRE-relevant
    ("inspireidentifiziert"), yielding a MDi1.1[^34] (The number of
    spatial data sets for which metadata exist) conformance rate of 72 %

- 3176 datasets carry the HVD keyword, of which 54 originate from BGR
    and 3 from DWD

  - Those numbers are extracted directly via the monitoring tool and
        are not available for outside access. Questions regarding more
        precise queries and exact numbers should be directed
        to: <support@gdi-de.org>

#### GDI-DE operational observations and challenges

Based on the current state of the Monitor and HVD-tagging workflow, the
following issues have been identified:

- **Inconsistent HVD thesaurus naming**: The HVD keyword is
    case-sensitive and not applied uniformly, making consolidation
    across records difficult

- **Downstream catalogs opaque**: Harvesting via Geodatenkatalog.de
    does not transparently identify secondary catalogs, hindering
    traceability of metadata origins

- **Outdated Monitor structure**: The existing Monitor UI and data
    model are antiquated; a redesign focused on metadata quality metrics
    is already underway

- **Mixed provider catalogs**: Multiple data-providing authorities
    (federal and Länder) share catalogs; since the "Bund" flag is
    assigned at catalog level, identifying the true origin of each
    dataset later is non-trivial

- **CSW performance limitations**: Current CSW queries are slow and
    were not designed for large-scale HVD searches

- **No CSW HVD thesaurus**: There is no dedicated HVD thesaurus for
    CSW, so HVD identification falls back on "any text" searches,
    resulting in imprecise tagging

Compiling these issues and challenges provides value to the research
community: it raises awareness among researchers, helping to explain why
certain data may not yet be discoverable. Additionally, these points can
inform researchers' own work on data and metadata. If further challenges
are identified, they should be added to the list and communicated to the
GDI-DE Monitor. In this way, the exercise also provides added value for
GDI-DE.

### GovData

**GovData**[^35] is the official open data portal of the German federal
government. It serves as a central metadata aggregator and publication
platform for administrative datasets originating from various levels of
government---federal, state, and municipal. As a metadata hub, GovData
enables structured, standardized, and FAIR-aligned access to public
data, supporting scientific, administrative, and civic reuse. It relies
primarily on the [DCAT-AP-DE](https://www.dcat-ap.de/)[^36] metadata
standard and provides interfaces for both manual access (via its web
portal) and machine-readable harvesting[^37] (via RDF, TURTLE and
JSON-LD APIs).

Several federal institutions provide metadata to GovData that is
relevant to the ESS domain. These include:

- **Federal Statistical Office (Destatis)** -- Socio-environmental
    indicators, land use, demography,

- **Federal Environment Agency (UBA)** -- Environmental monitoring
    data, air quality, water quality,

- **Federal Institute for Geosciences and Natural Resources (BGR)** --
    Geology, mineral resources, soil data,

- **German Meteorological Service (DWD)** -- Climate and weather data,

- **Federal Maritime and Hydrographic Agency (BSH)** -- Marine and
    coastal data,

- **Federal Agency for Cartography and Geodesy (BKG)** -- Base
    geospatial datasets, topography, reference systems.

These institutions typically expose their metadata through
INSPIRE-compliant or DCAT-based catalogs, which are harvested by GovData
on a regular basis.

GovData plays a central role in the implementation of the European
High-Value Dataset (EU-HVD) regulation. As Germany's official HVD focal
point, GovData is tasked with publishing metadata for all federally
maintained datasets falling under the six HVD categories (see HVD).

In addition to federal institutions, **state and municipal authorities**
also contribute metadata to GovData. Examples include:

- **Open.NRW** (North Rhine-Westphalia),

- **OpenData.Berlin**,

- and other regional platforms that syndicate their metadata through
    DCAT-AP-DE catalogs.

These non-federal contributors play a crucial role in publishing spatial
These non-federal contributors play a crucial role in publishing spatial
and administrative datasets, often complementary to those of federal
agencies. However, their metadata often lacks consistent HVD or thematic
annotations relevant to ESS, limiting semantic discoverability.

#### GovData monitoring metrics

The following results are based on our own survey conducted on the
GovData portal. For this purpose, the portal's search function and the
keyword *HVD* were used. This approach relates solely to the search and
retrieval process within the portal and does not imply that *HVD* is
used as a keyword in the underlying metadata.

As of August 13, 2025, the platform lists:

- 6,295 HVD-designated metadata records,

- of which 5,206 are INSPIRE-identified datasets
    ("inspireidentifiziert"),

- and 642 datasets are tagged with the keyword \"HVD\".

45 HVD datasets come directly from the BGR, 9 from the BKG and 34 from
DWD.

HVD metadata is not consistently annotated with thematic keywords from
controlled vocabularies, which restricts discoverability through
keyword-based filtering. This inconsistency points to the need for
improved metadata annotation practices, particularly with respect to the
application of controlled vocabularies and the classification of
datasets as HVD. Nonetheless, GovData has begun aligning its metadata
practices with EU implementation guidelines, including the systematic
use of controlled vocabularies and semantic tagging.

Germany's reporting on high-value datasets under Commission Implementing
Regulation (EU) 2023/138[^38] may reference its national open data
catalogue (GovData) for metadata, API and licence links (Art.
5(3)(a)--(c)). The EU framework monitors Member State compliance for the
following points:

- completeness and timeliness of HVD publication,

- interface availability,

- and accessibility of metadata and underlying datasets.

#### GovData operational observations and challenges

While GovData provides essential infrastructure for metadata
aggregation, several challenges have been observed. In particular, the
incomplete mapping of ISO 19139 to DCAT-AP-DE leads to a loss of
metadata at the aggregator site:

- **Inconsistent use of the \"HVD\" keyword** across datasets, making
    search and filtering unreliable,

- **Incomplete thesaurus integration**, limiting semantic
    interoperability and keyword harmonisation across data providers,

- **Redundant metadata entries** or catalog overlaps due to repeated
    harvesting from both federal and regional catalogs (e.g., the same
    dataset listed by both BKG and GDI-DE),

- **Lack of linkage** between metadata records and authoritative
    vocabularies (e.g., GEMET, INSPIRE themes),

- **Variation in metadata quality**, especially in descriptive fields
    such as abstract, temporal coverage, and licensing,

- **Sparse metadata for APIs or real-time data feeds**, which are
    increasingly important for research in Earth System Sciences.

GovData fulfills a vital role as Germany's central metadata aggregator,
especially in the context of EU-HVD implementation. While its coverage
and technical infrastructure are substantial, **metadata quality
assurance**, **keyword governance**, and **semantic annotation
practices** remain areas for improvement. Continued alignment with the
FAIR principles and EU metadata guidelines will be key to increasing the
value of GovData for scientific users, particularly in the Earth System
Sciences.

### UBA umwelt.info

**umwelt.info**[^39] is a search engine developed by the German
Umweltbundesamt (Federal Environment Agency, UBA) as a central access
point to publicly available environmental and nature conservation data
across Germany. It aims to make environmental information---such as
maps, measurements, research findings, educational materials, and
funding program descriptions---findable and comparable. The search
results are evaluated based on the fulfillment of the FAIR criteria. The
portal umwelt.info is hosted by the UBA (National Center for
Environmental and Nature Conservation Information).

The web portal complements the offerings of **GDI-DE** and **GovData**
with a thematic, user-oriented access point that focuses on
environmental topics and makes searching easier for both experts and
non-experts. For ESS researchers, umwelt.info provides an intuitive,
central entry point to locate relevant environmental datasets across
various institutions---ranging from federal agencies to civil society.
The portal's intelligent search functionality, combined with editorial
content and clearly displayed metadata, enhances data discovery and
lowers access barriers.

umwelt.info collects metadata and references to datasets. Harvesting
covers a broad range of providers---including federal agencies, research
institutions, regional authorities, NGOs, and even private individuals
or organizations. The engine harvests metadata via technical
interfaces---such as APIs---where available, and employs web harvesting
(crawling) and scraping to gather metadata from sources that lack
machine-readable interfaces[^40]. The internal metadata model is
influenced by DCAT-AP.de but remains flexible enough to accommodate
diverse, non-standard data sources.

The portal does not store full datasets, but integrates metadata---like
titles, descriptions, licenses, spatial and temporal extent, source
links, and resource links to datatsets if openly accessible---into its
search index. If metadata are missing or unstructured, umwelt.info
creates structured metadata (e.g., via scraping) to ensure consistency
and discoverability.

#### UBA monitoring metrics

There is no publicly displayed metric on umwelt.info about how many HVDs
are listed. While the portal may indeed capture metadata from HVD
sources, the number of HVDs, completeness, or timeliness is not reported
in its public interface or documentation.

#### UBA operational Observations and opportunities

While the portal's flexible metadata (and data) search capabilities
offer clear advantages, they also pose several challenges:

- **Heterogeneity of data sources**: Because umwelt.info harvests from
    very diverse systems, **metadata quality and format vary widely**---
    making stringent filtering necessary before applying the index for
    individual use cases.

- **Metadata standardization limits**: umwelt.info does not impose a
    strict metadata standard but uses an adaptive internal schema. This
    ensures wide coverage but can impact consistency[^41].﷟ Therefore
    umwelt.info offer a publicly accessible API based on CKAN-standard.

- **Completeness vs. feasibility**: Since not all data providers offer
    APIs or structured metadata, some sources must be scraped---raising
    concerns about completeness, freshness, and data integrity. At the
    same time, scraping enables the capture of additional, even
    unstructured, content, but this approach introduces specific
    challenges that need to be carefully addressed and resolved.

- **Scaling editorial support**: Presenting thematic, curated search
    results and editorial context (articles, infographics) requires
    ongoing coordination and resource allocation[^42].﷟ Currently, this
    is implemented through dedicated editorial workflows at umwelt.info,
    where experts curate and contextualise content for specific
    environmental and thematic domains.

- **Data provider engagement**: Encouraging agencies and institutions
    to expose structured metadata (e.g., via DCAT or APIs) remains
    crucial and challenging. The portal is open to advising
    organizations on best practices.

In the governmental domain, there are additional portals---beyond those
previously mentioned---that collect structured metadata to varying
degrees. However, as far as we can determine, all of this metadata is
harvested by one of the aggregators we have already discussed.

## GDI-DE Profile convention for metadata of High-Value Datasets

To ensure consistent identification, discovery, and harvesting of HVD,
the GDI-DE has issued a binding profile convention for ISO 19115/19139
metadata applicable to all datasets falling under the scope of the
DVO-HVD. This requirement supplements the general metadata conventions
described in Chapter 6 of GDI-DE "Konventionen zu Metadaten"[^43], which
govern all Open Data transfers to the national portal GovData.

A dataset is recognised as HVD within the GDI-DE ecosystem only if its
metadata explicitly carries the HVD tag as prescribed by the profile
convention. Such tagging ensures that the dataset is ingested into
GovData and is counted toward Germany's national DVO-HVD reporting
obligations.

Within each `gmd:descriptiveKeywords` element, one of the six EU HVD
category Uniform Resource Identifiers (URIs) must be embedded as a
`gmx:Anchor` value, for example:

In each `gmd:descriptiveKeywords` section, one of the six EU
HVD-category URIs must be inserted as a `gmx:Anchor`:

\scriptsize

+----------------------------------+----------------------------------+
| **HVD Category (German           | **URI**                          |
| categories)**                    |                                  |
+==================================+==================================+
| Geospatial (Georaum)             | <http:                           |
|                                  | //data.europa.eu/bna/c_ac64a52d> |
+----------------------------------+----------------------------------+
| Earth Observation and            | <http:                           |
| Environment (Erdbeobachtung und  | //data.europa.eu/bna/c_dd313021> |
| Umwelt)                          |                                  |
+----------------------------------+----------------------------------+
| Meteorology (Meteorologie)       | <http:                           |
|                                  | //data.europa.eu/bna/c_164e0bf5> |
+----------------------------------+----------------------------------+
| Statistics (Statistik)           | <http:                           |
|                                  | //data.europa.eu/bna/c_e1da4e07> |
+----------------------------------+----------------------------------+
| Business and Ownership           | <http:                           |
| Information (Unternehmen und     | //data.europa.eu/bna/c_a9135398> |
| Eigentümerschaft von             |                                  |
| Unternehmen)                     |                                  |
+----------------------------------+----------------------------------+
| Mobility (Mobilität)             | <http:                           |
|                                  | //data.europa.eu/bna/c_b79e35eb> |
+----------------------------------+----------------------------------+

\normalsize

The list provided by the Publications Office of the EU itself is
referenced as the associated source in the `thesaurusName` element as
follows:

- `title` element: `gmx:Anchor` pointing to
    "<http://data.europa.eu/bna/asd487ae75>"

- `date` element: "2023-09-27" with `dateType="publication"`

As an interim compatibility measure, metadata records may alternatively
include the German category name as free text while citing HVD
categories in the `gmd:thesaurusName` element.

The associated source is specified in the `thesaurusName` element as
follows:

- `title` element: "High-value dataset categories"

- `date` element: "2023-09-27"

- `dateType` element: "publication"

However, this approach is less robust for automated harvesting and is
therefore discouraged in favour of the URI-based method.

[@fig:workflow] summarizes the path from the original data provider through the
GDI-DE metadata catalogue to the GovData national portal and,
ultimately, to DVO-HVD reporting. HVD tagging according to the GDI-DE
profile convention is applied at the metadata ingestion stage.

![Workflow for High-Value Dataset metadata within the GDI-DE framework.](./figure2.png){#fig:workflow}

### Observed shortcomings and next steps

- National scope only[^44] -- The DVO-HVD requires coverage at Member
    State level; transboundary datasets of relevance to ESS are
    currently excluded.

- Metadata-only limitation[^45] -- HVD tagging addresses
    discoverability but does not guarantee underlying data quality,
    completeness, or interoperability.

- Pipeline reliability issues[^46] -- Variations in thesaurus naming
    (including case sensitivity) and the absence of a dedicated HVD
    thesaurus in the CSW endpoint reduce harvesting consistency.

These results are expected to be incorporated into the planned redesign
of the GDI-DE monitor and the HVD processing pipeline. The objective is
to implement more rigorous metadata quality controls, harmonised
thesaurus handling, and end-to-end traceability from the original data
provider to the national GovData reporting framework.

# Method for increasing gov-data

Ensuring that gov-data relevant to ESS is **findable, accessible, and
usable** requires more than simply publishing metadata. It depends on a
coordinated strategy for searching, aggregating, and validating metadata
across multiple portals, with consistent use of standards and
identifiers. In addition, robust quality controls for (meta)data and
semantic search options play a key role in improving the findability and
reuse of government data in research.

This chapter presents a workflow for improving gov-data visibility
through the *NFDI4Earth OneStop4All*[^47] (OneStop4All) portal as the primary
discovery interface for scientists with the
*NFDI4Earth KnowledgeHub*[^48] serving as its metadata backend. HVD are
used as a worked example, both because of their legal relevance under
*DVO-HVD* and because they present an excellent test case for end-to-end
data pipeline quality. For OneStop4All to function as a comprehensive
discovery service, it must integrate gov-data from national metadata
providers (e.g., GDI-DE, GovData). Within this framework, HVD can be
flagged or prioritized in the KnowledgeHub to highlight their importance
for ESS research.

## Search definition

The process begins with the definition of the search scope. This
includes:

- **Dataset scope** -- e.g., all HVD categories relevant to ESS:

  - Geospatial (land use, administrative boundaries)

  - Earth Observation & Environment (remote sensing products,
        habitat maps)

  - Meteorological (weather station data, climate series)

- **Target authorities** -- e.g.,

  - Deutscher Wetterdienst (DWD) for meteorological HVD,

  - Bundesanstalt für Geowissenschaften und Rohstoffe (BGR) for
        geological HVD.

- **Additional filters** -- e.g., "High-Value Dataset" tagging,
    spatial coverage (national), temporal coverage (past 30 years),
    formats (NetCDF, CSV, GeoPackage), licences (Open Data). In order to
    make search definitions more effective, it is essential to
    supplement them with **semantic search options** (e.g., synonyms,
    ontologies, controlled vocabularies), as these compensate for
    differences in terminology between portals and authorities.

**Example**: Define a search for Meteorological HVD provided by DWD,
with the keywords "climate time series" and "station observations",
restricted to datasets covering Germany in machine-readable form.

## Data availability search

The defined search is executed in parallel across three primary
platforms:

1. **GDI-DE** (national INSPIRE-based spatial data catalogue),

2. **GovData** (German national open data portal), and

3. **OneStop4All** (NFDI4Earth).

For each platform, the number of matching datasets is recorded. This
produces a 3 × 2 result matrix for the example of two authorities (three
platforms × two counts: HVD-tagged matches for DWD and BGR).

**Example**: In addition to GDI-DE (Chapter 2.2.1
produces a 3 × 2 result matrix for the example of two authorities (three
platforms × two counts: HVD-tagged matches for DWD and BGR).

**Example**: In addition to GDI-DE (Chapter 2.2.1) and GovData (Chapter
2.2.2), a targeted search was conducted in the KnowledgeHub via SPARQL
query[^49].

A manual search was also performed via the web portal OneStop4All. Here,
results vary significantly depending on the applied keyword. The example
of HVD data yields the results shown in {@tbl:comparison}.

\scriptsize

  Platform / Source                        Total HVD datasets   DWD   BGR
  ---------------------------------------- -------------------- ----- -----
  GDI-DE Monitor                           3176                 3     54
  GovData                                  6295                 34    45
  KnowledgeHub: keyword "HVD"              602
  KnowledgeHub: keyword "hvd"              1
  OneStop4All: keyword "HVD"               1144                 4     0
  OneStop4All: keyword "High-value data"   460                  0     20

: Comparison of HVD dataset availability across infrastructures {#tbl:comparison}

\normalsize

The search is a snapshot, so you can\'t expect everything to match up
perfectly. Still, there are some clear differences: The numbers vary
widely across platforms. OneStop4All shows strong **keyword
dependency**, with DWD and BGR datasets only discoverable under
different terms. These inconsistencies confirm that **metadata
harmonisation and thesaurus alignment** are necessary to improve
visibility and ensure reliable harvesting into OneStop4All. The highly
keyword-dependent hits in OneStop4All underscore the need for
**thesaurus-based and semantic search**, which standardizes different
spellings and synonyms.

## Coverage comparison

The counts are compared to detect coverage gaps:

- Are all HVD-tagged datasets present in OneStop4All?

- Do any exist in GDI-DE or GovData but are missing from OneStop4All?

- Are some HVD datasets missing an HVD tag in metadata?

Such deviations can be reduced through **systematic quality controls**
(e.g., validation of HVD tags, automated checks for gaps).

**Example analysis**: The DWD climate series appear in GDI-DE and
GovData, but two datasets are missing in OneStop4All due to absent HVD tags
in the harvested metadata. One additional dataset is missing entirely
because it is only published on the DWD website without portal
integration.

## Direct action and feedback channels

When gaps are detected, the following actions are initiated:

- **Portal-level contact** -- Use official feedback channels of GDI-DE
    and GovData to report missing records.

- **Authority-level contact** -- Directly approach the responsible
    agency (e.g., DWD, BGR) to address metadata publication or tagging
    issues.

- **NFDI4Earth support structures** -- Utilise the *Interest Group
    Metadata* and the NFDI4Earth Helpdesk to coordinate follow-up, track
    issues, and propose standardisation improvements.

**Example action**: For the missing DWD datasets, OneStop4All project staff
submit an issue to the IG Metadata mailing list, tagging it as "HVD gap
-- meteorology". The DWD data officer is contacted via GDI-DE feedback
form to update metadata records with the proper HVD URI.

## Identification of weak points and solution pathways

The process (see [@fig:gaps]) not only identifies missing datasets but also highlights
systemic weaknesses such as:

- Metadata inconsistencies (e.g., non-standard HVD category naming),

- Gaps in harvesting pipelines from source catalogues to OneStop4All,

- Lack of prioritisation or highlighting for HVD in search interfaces.

These findings feed into a *solution blueprint* (Anders et al.,
2024[^50]) to propose technical fixes such as:

- Establishment of automated quality control for (meta)data,

- Greater harmonisation of metadata with ontologies and controlled
    vocabularies,

- Integration of semantic search mechanisms into OneStop4All to take
    synonyms and multilingualism into account,

- Enforcing URI-based HVD tagging in metadata,

- Expanding KnowledgeHub harvesting endpoints,

- Implementing an "HVD priority" search filter in OneStop4All.

![Workflow for identifying and resolving gaps in the visibility
of governmental data.](./figure3.png){#fig:gaps}

# Recommendations

Building on the findings from Chapters 2 and 3 and informed by
stakeholder workshops, this chapter summarises actionable
recommendations to improve the discoverability, accessibility, and
usability of governmental data (gov-data) for Earth System Science
(ESS). The recommendations draw on lessons learnt from:

- **NFDI4Earth HVD Workshop** (Hamburg, November 2024), and

- **GDI-DE Workshop "High-Value Datasets from a User Perspective"**
    (March 2025).

The measures outlined here address technical, organisational, and
collaborative dimensions of the HVD pipeline and can also be applied to
gov-data more broadly.

## Strengthening feedback channels

**Observation:**

Both workshops highlighted the absence of a formalised feedback
mechanism for scientists to report missing datasets, metadata issues, or
usability problems back to governmental authorities and portal
operators.

**Recommendations:**

- **Establish a persistent feedback channel** -- potentially via the
    *User Support Network* (USN) of NFDI4Earth -- to collect, triage,
    and forward issues to data providers.

- **Leverage existing structures** -- integrate with GDI-DE's and
    GovData's support forms, while maintaining a central NFDI4Earth
    tracking system.

- **Pre-publication feedback loop** -- before releasing new HVD
    datasets, run a quick expert review (scientists) to verify metadata
    completeness, file usability, and documentation quality.

- To further ensure data quality, **automated checks for metadata
    completeness and HVD tag consistency** should complement the expert
    pre-publication review.

## Improving data preparation and documentation

**Observation:**

Several datasets suffer from insufficient guidance on access, format,
and structure. Examples from the workshops include:

- Lack of code snippets or download instructions.

- No documentation for file contents (e.g. time ranges, variable
    lists).

- Ambiguous or proprietary formats without explanation (e.g. .cap XML
    format).

- Deviations from standard formats not documented (e.g. SYNOP data
    exceptions).

**Recommendations:**

- **Provide minimal technical onboarding** for each dataset:

  - Short description of contents.

  - Information on spatial/temporal coverage.

  - Supported formats and conversion hints (e.g. Shapefile to
        GeoPackage).

  - Sample code (Python, R) for download and parsing.

- **Standardise file structures** where possible; where not possible,
    provide explicit exceptions documentation.

- **Ensure primary data access** for datasets that are currently only
    available in derived form (e.g. D-AERO).

- Additionally, consistent use of **controlled vocabularies and clear
    thesaurus references** will improve interoperability and enable
    semantic search across platforms.

## Metadata quality for scientific use

**Observation:**

Scientific workflows require richer metadata than is sometimes provided
under minimal Open Data obligations. The *White Paper: Recommendations
for Earth System Sciences Metadata Provision* offers a useful reference,
which could be aligned with gov-data conventions and HVD metadata
profiles.

**Recommendations:**

- **Adopt ESS-specific metadata extensions** for HVD in addition to
    mandatory DCAT/ISO elements (e.g., variable list, processing
    history, uncertainty estimates).

- **Automated quality control procedures** should be established to
    validate metadata formats, completeness, and adherence to controlled
    vocabularies.

- **Harmonise tagging practices** for HVD categories (URI-based,
    case-consistent).

- **Semantic search mechanisms**, including synonym resolution and
    multilingual support, should be integrated to enhance
    discoverability for diverse scientific workflows.

- **Promote registration of authorities in re3data**, ensuring
    institutional persistence and visibility in the research data
    ecosystem.

## Enhancing cross-sector collaboration

**Observation:**

Sustainable improvement of HVD quality and usability requires ongoing
interaction between data providers and the scientific community.

**Recommendations:**

- **Create regular exchange formats** -- e.g., thematic workshops,
    joint metadata hackathons, or an online forum moderated by
    NFDI4Earth.

- **Document and share use cases** where scientist--authority
    collaboration improved data quality, serving as blueprints for other
    domains.

- **Highlight mutual benefits** -- better usability increases
    scientific uptake, while positive exposure strengthens the mandate
    for open data provision.

- **Collaboration** should also support the **continuous monitoring
    and versioning of harvesting pipelines** between source portals
    (GDI-DE, GovData) and the OneStop4All / KnowledgeHub to ensure data
    consistency and reliability over time.

## Contact points to science

**Observation:**

Authorities often lack established communication channels to the
research community, leading to one-way data publication without
iterative improvement.

**Recommendations:**

- **Map existing contact networks** -- identify existing liaison
    roles, committees, or domain-specific working groups that could
    bridge science--authority communication.

- **Integrate these channels into NFDI4Earth** -- ensuring they are
    discoverable via the OneStop4All KnowledgeHub.

- **Develop a rapid-response mechanism** -- enabling timely feedback
    and resolution without multi-month delays.

These measures collectively address the key questions outlined at the
beginning of this report: enabling authorities to publish and annotate
data effectively, improving scientists' ability to find and access data,
and ensuring a sustainable, high-quality data pipeline.

**Overall priority actions:**

1. Set up a coordinated feedback and tracking mechanism via NFDI4Earth.

2. Enrich HVD metadata and documentation for scientific workflows.

3. Establish sustainable collaboration formats between authorities and
    scientists.

4. Ensure consistent metadata tagging and authority registration in
    research data registries.

\scriptsize

+----------------+----------------+--------------+----------------+
| **Re           | **Respons      | **Priority** | **Expected     |
| commendation** |        ible**  |              | Impact**       |
+================+================+==============+================+
| Establish      | NFDI4Earth,    | High         | Continuous     |
| persistent     | GDI-DE,        |              | improvement of |
| feedback       | GovData        |              | data quality   |
| channel (via   |                |              | and            |
| NFDI4Earth     |                |              | completeness   |
| USN)           |                |              | through direct |
|                |                |              | issue          |
|                |                |              | reporting.     |
+----------------+----------------+--------------+----------------+
| Implement      | Data-providing | Medium       | Early          |
| p              | authorities,   |              | correction of  |
| re-publication | NFDI4Earth     |              | meta           |
| feedback loop  | experts        |              | data/usability |
| for HVD        |                |              | issues before  |
|                |                |              | public         |
|                |                |              | release.       |
+----------------+----------------+--------------+----------------+
| Provide        | Data providers | High         | Reduced entry  |
| minimal        | (e.g., DWD,    |              | barriers for   |
| technical      | BGR)           |              | ESS            |
| onboarding     |                |              | scientists,    |
| (docs + code   |                |              | faster dataset |
| snippets) for  |                |              | integration in |
| each dataset   |                |              | workflows.     |
+----------------+----------------+--------------+----------------+
| Standardise    | Data providers | Medium       | Increased      |
| file           |                |              | in             |
| structures or  |                |              | teroperability |
| document       |                |              | and reduced    |
| deviations     |                |              | processing     |
|                |                |              | time for end   |
|                |                |              | users.         |
+----------------+----------------+--------------+----------------+
| Ensure primary | Data providers | High         | Enables        |
| data access    |                |              | r              |
| where only     |                |              | eproducibility |
| derived data   |                |              | and advanced   |
| is provided    |                |              | scientific     |
|                |                |              | analyses.      |
+----------------+----------------+--------------+----------------+
| Adopt          | Data           | Medium       | Improved       |
| ESS-specific   | providers,     |              | scientific     |
| metadata       | NFDI4Earth IG  |              | relevance and  |
| extensions for | Metadata       |              | d              |
| HVD            |                |              | iscoverability |
|                |                |              | of datasets.   |
+----------------+----------------+--------------+----------------+
| Harmonise      | Data           | Medium       | Consistent     |
| tagging        | providers,     |              | search results |
| practices for  | metadata       |              | and reduced    |
| HVD categories | catalog        |              | false          |
|                | operators      |              | negatives in   |
|                |                |              | dataset        |
|                |                |              | discovery.     |
+----------------+----------------+--------------+----------------+
| Register       | Data           | Low          | Increased      |
| authorities in | providers,     |              | international  |
| re3data        | institutional  |              | visibility and |
|                | data managers  |              | integration in |
|                |                |              | research data  |
|                |                |              | in             |
|                |                |              | frastructures. |
+----------------+----------------+--------------+----------------+
| Create regular | NFDI4Earth,    | Medium       | Strengthened   |
| exchange       | authorities,   |              | trust and      |
| formats        | ESS community  |              | shared         |
| (forums,       |                |              | understanding  |
| workshops,     |                |              | between data   |
| hackathons)    |                |              | providers and  |
|                |                |              | scientists.    |
+----------------+----------------+--------------+----------------+
| Map and        | NFDI4Earth,    | High         | Direct and     |
| integrate      | authorities    |              | efficient      |
| existing       |                |              | communication  |
| science        |                |              | between        |
| contact        |                |              | stakeholders,  |
| networks       |                |              | enabling rapid |
|                |                |              | feedback       |
|                |                |              | cycles.        |
+----------------+----------------+--------------+----------------+
| Develop a      | Authorities,   | High         | Timely         |
| rapid-response | NFDI4Earth USN |              | corrections    |
| mechanism for  |                |              | and            |
| feedback       |                |              | improvements   |
| resolution     |                |              | without long   |
|                |                |              | delays,        |
|                |                |              | ensuring       |
|                |                |              | up-to-date     |
|                |                |              | data           |
|                |                |              | availability.  |
+----------------+----------------+--------------+----------------+

: Compilation of recommendations with responsibilities, prioritization, and expected impact {#tbl:recommendations}

\normalsize

# Outlook

The present report constitutes an initial step toward enhancing the
discoverability and usability of governmental data (gov-data) for the
Earth System Science (ESS) community. A follow-up version --- planned as
**Deliverable D2.3.2** --- will incorporate direct feedback from ESS
researchers to refine both the methodological approach and the technical
recommendations.

To ensure that the updated report reflects the practical needs of its
users, feedback channels will be actively promoted and maintained.
Options include:

- **User Support Network (USN)**[^51] and its ticketing system,
    enabling structured and trackable issue reporting.

- **Direct author contact** for case-specific inputs.

The choice of feedback mechanism will depend on the required immediacy,
the complexity of the feedback, and the need for follow-up discussions.
Engagement will be further supported by targeted calls for contributions
via ESS mailing lists, NFDI4Earth communication channels, and relevant
community forums.

The continued development of workflows and conventions for metadata and
data publication will be aligned with ongoing work in **standardization
bodies (e.g., DIN)** and relevant European and international
initiatives. This will ensure that national practices remain
interoperable with broader frameworks and benefit from community-driven
best practices.

Future efforts must not focus solely on the discovery of datasets, but
also on their transformation into value-added products and services:

1. **From Data → to Data Products** -- ensuring validation,
    standardization, and rich metadata to guarantee scientific
    reusability.

2. **From Data Products → to Data Services** -- offering static and
    dynamic portals or APIs for visualization, analysis, editing,
    downloading, and generating actionable insights.

This progression will support a fully FAIR-aligned ecosystem, where
datasets are not only findable but also directly usable in applied and
research contexts.

The next phase of work will be guided by four interlinked goals:

1. **Finding the Data** -- integrating services and metadata search
    engines for comprehensive discovery across domains and
    infrastructures.

2. **Using the Data** -- providing clear access and enabling effective
    FAIR-compliant utilization.

3. **Interoperable Data** -- ensuring compatibility across disciplines,
    applications, and regions.

4. **Reusable Data** -- facilitating adaptation and application of
    datasets for new use cases.

Through this framework, the future work will progressively close
existing gaps, improve collaboration between public authorities and ESS
scientists, and strengthen the overall infrastructure for open and
interoperable gov-data.

# Acknowledgements {#acknowledgements .unnumbered}

We thank Eric Habiryayo (Bundesanstalt für Geowissenschaften und
Rohstoffe) for his valuable discussions within Measure 2.3, which
contributed indirectly to the conceptual framing of this report.
Furthermore, we thank Jonas Grieb (Senckenberg Gesellschaft für
Naturforschung) and Anna Brauer (TU Dresden) from the KnowledgeHub Team
of NFDI4Earth for supporting us with SPARQL requests.

This work has been partly funded by the German Research Foundation (DFG)
through the project NFDI4Earth (DFG project no. 460036893,
<https://www.nfdi4earth.de/>) within the German National Research Data
Infrastructure (NFDI, <https://www.nfdi.de/>).

[^1]: Wilkinson, M. D., et al. (2016). The FAIR Guiding Principles for scientific data management and stewardship. Scientific Data, 3, Article number: 160018. <https://doi.org/10.1038/sdata.2016.18>

[^2]: <https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32023R0138>

[^3]: <https://eur-lex.europa.eu/eli/dir/2007/2/2019-06-26>

[^4]: <https://www.gov.uk/government/publications/open-data-charter/g8-open-data-charter-and-technical-annex>

[^5]: <https://eur-lex.europa.eu/legal-content/EN/ALL/?uri=CELEX%3A32023R0138>

[^6]: <https://www.gdi-de.org>

[^7]: <https://www.govdata.de>

[^8]: <https://umwelt.info>

[^9]: <https://www.nfdi4earth.de>

[^10]: <https://knowledgehub.nfdi4earth.de>

[^11]: <https://onestop4all.nfdi4earth.de>

[^12]: <https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj/eng>

[^13]: Chapter (2): <https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj/eng>

[^14]: <https://www.gesetze-im-internet.de/geozg>

[^15]: Article 1: <https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32007L0002&qid=1752146988381>

[^16]: <https://eur-lex.europa.eu/eli/dir/2019/1024/oj?eliuri=eli%3Adir%3A2019%3A1024%3Aoj&locale=en>

[^17]: <https://www.bmwk.de/Redaktion/DE/Gesetze/Technologie-Innovation/iwg.html>

[^18]: <https://eur-lex.europa.eu/legal-content/EN/ALL/?uri=CELEX%3A32003L0098>

[^19]: <https://www.gesetze-im-internet.de/dng/index.html#BJNR294200021BJNE00070000>

[^20]: <https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:02016R0679-20160504>

[^21]: <https://www.govdata.de>

[^22]: <https://www.gdi-de.org>

[^23]: <https://www.destatis.de/EN/Home/_node.html>

[^24]: <https://dataeuropa.gitlab.io/data-provider-manual/hvd/annotation_in_geometadata>

[^25]: <https://onestop4all.nfdi4earth.de/>

[^26]: <https://eur-lex.europa.eu/eli/dir/2007/2/2024-11-26/eng>

[^27]: <https://geoportal.de>

[^28]: <https://geodatenkatalog.de/gdi-de/srv/ger/catalog.search#/home>

[^29]: <https://registry.gdi-de.org>

[^30]: <https://www.gdi-de.org/en/SDI/components/GDI-DE%20Testsuite>

[^31]: <https://www.gdi-de.org/en/SDI/components/GDI-DE%20Monitor>

[^32]: <https://www.gdi-de.org/>

[^33]: <https://ggim.un.org/UN-IGIF/documents/Aktionsplan-IGIF-german.pdf>

[^34]: <https://wiki.gdi-de.org/download/attachments/1334739009/DOC6_MIG10_IndicatorsGuide_v2019-07-19.pdf?api=v2>

[^35]: <https://www.govdata.de>

[^36]: <https://www.dcat-ap.de>

[^37]: <https://www.govdata.de/suche/daten/govdata-metadatenkatalog>

[^38]: <https://eur-lex.europa.eu/eli/reg_impl/2023/138/oj/eng>

[^39]: <https://umwelt.info>

[^40]: <https://umwelt.info/de/artikel/ueber-den-metadatenexport>

[^41]: <https://www.umweltbundesamt.de/umweltinfo-faq>

[^42]: <https://www.umweltbundesamt.de/umweltinfo-start-tab>

[^43]: <https://www.gdi-de.org/download/AK_Metadaten_Konventionen_zu_Metadaten.pdf>

[^44]: <https://dataeuropa.gitlab.io/data-provider-manual/hvd/Reporting_guidelines_for_HVDs>

[^45]: <https://dataeuropa.gitlab.io/data-provider-manual/hvd/Reporting_guidelines_for_HVDs>

[^46]: <https://www.loc.gov/catworkshop/lcsh/PDF%20scripts/1-2-WhyCV.pdf>

[^47]: <https://onestop4all.nfdi4earth.de>

[^48]: <https://knowledgehub.nfdi4earth.de>

[^49]: [https://sparql.knowledgehub.nfdi4earth.de/](https://sparql.knowledgehub.nfdi4earth.de/?default-graph-uri=&qtxt=%23%20Count%20all%20subjects%20(e.g.%20datasets%2C%20data-services)%20where%20the%20keyword%20%22HVD%22%20is%20used%0APREFIX%20dcat%3A%20%3chttp%3A%2F%2Fwww.w3.org%2Fns%2Fdcat%23%3e%0A%0ASELECT%20(count(distinct%20%3Fsubject)%20as%20%3Fcount)%0AWHERE%20%7B%0A%20%20%3Fsubject%20dcat%3Akeyword%20%3Fk%20.%0A%20%20%23%20Need%20to%20use%20the%20filter%20with%20string%20casting%20because%20literals%20in%20the%20database%20are%20sometimes%20as%20%22HVD%22%40en%20or%20%22HVD%22%40de%20%0A%20%20FILTER(STR(%3Fk)%3D%22HVD%22)%0A%7D%0A%0A%0A&format=text%2Fhtml) (follow link for full query)

[^50]: Anders, I., Kaspar, F., Kratzenstein, F., Schupfner, M., & Thiemann, H. (2024). Standardisation and making public authority data available for research. Zenodo. <https://doi.org/10.5281/zenodo.10948876>

[^51]: <https://onestop4all.nfdi4earth.de/>
