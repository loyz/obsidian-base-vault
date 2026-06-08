#FAIRagro #FAIRagroSummit26 

https://fairagro.net/community-summit-2026/#Programm
-----------------
**Keynote: The Key to Unlocking Community Potential and Innovation**
presenter: Matthias Lange

- Sustainable Infrastructure (slide)
- DataStewards buiding bridge between people and technologies / Institutional, General RD, Project Data Engineer.
- Incentives (KPIs: Publications, data publications, building up repositories/downloads, portals with visualisations etc., search)
Key (slide: green)

13:30
FAIRagro Search Hub
Julian and Atan
https://search-hub.fairagro.net
- Datasets
	- schema.org for general metadata
- Repositories (make interoperable)
	- scores for finability, acessibility, interoperability, 
	- re3data profile
	- even other NFDI repositories (RDAs)

**AI-based enrichment for Search Hub metadata – A case study ** 
_Abanoub Abdelmalak, FAIRagro_
- FAIRagro UC8: Model development and evaluation
- extract freetext metadata, enrich with URIs from AGROVOC API
- pass to Search Hub, crop and soil metadata enriched ca. 1.9 enrichments per dataset

**DWD Opendata: From Geonetwork to FAIRagro Repositories
_Rafael Posada, Deutscher Wetterdienst_

- OAI portal
- GDI (geoportal.de)
- GovData
data flow from top down
28 TB expected to qualify

**Data Management Plans for the agrosystem science – FAIRagros RDMO service and its templates**
_Antonia Leidel, FAIRagro_
- rdmo.fairagro.net
- Login via ORCID
- Link to Helpdesk

**DMP-Development and Experiences in a governmental environment**  
_Mirjam Prinz, StMELF_
from funders perspective RDM makes a lot of sense
funders should motivate for it
5 research institutions agriculture, wine, forestry, genetics ...?
Collaboration with BSA
DMP questionaire RDMO over FAIRagro
Antonia and Gabriel helped.
Still challenges: Only ORCID Login, but people without ORCID
When to reject a DMP? Needs to be simple to evaluate. There must be one responsible person, at least one data category, have to offer to Bavarian Archives, have talked to IT-department and IT-security, Cost information.
Helped a lot. Positive effects: raising consciousness and some institutes restructured to include RDM.
Culture change needs time.
from stone-age to digital age :)
Projects without RDMP and without having checked the boxes will be rejected.
Will the plan be checked later against results? at moment no. Later there should be data stewards in the institutions evaluating this.
Are researchers going back to RDMPs to optimise it? 
Talked to other funders about experience with introducing RDMOs? Not yet, but interested in exchange with them.

**FAIRagro DQ Services in the Data Life Cycle**
_Mahdi Hedayat Mahmoudi, FAIRagro_
- practical and modular tools to improve data quality across data lifecycle
- DQ4Agri quality analysis during data accquisition
- browser based
- Output: analyses
- BonaRES DQ-Kit: web app
- Trial Harvest-AI python pipeline for extraction of high quality standardised metadata
- FAIR Assessment Tool
- Standards Inventory: collection of vocabularies
- Publication Metadata Set: guidance on how to use schema.org
- Data Fitness Explorer (LLM powered) Interactive web app
- at moment only live demos (most of them)

SciWIn-Client and SciWIn-Studio: Simplifying FAIR Computational Workflows
_Jens Krumsieck_, FAIRagro

see full presentation on website

what is a workflow? input to output
different programming languages can be combined in pipeline
- workflows make transparent and reproducible
- why not used?
	- not aware
	- tool to learn
	- tool fragmentation
	- descriptions verbose
	- ...
- Common Workflow Language (CWL)
	- YAML based (easy parsable)
	- 3 types
		- Workflow
		- commandline tools
		- ..
- Shouldnt write CWL b y hand! => CyWIN Client
- s4n prefixing
- connect command to connect tools
- CyWIn Studio allows drag and drop creation of workflows.
what's the strategy to bridge the gap?
Is there a plan to combine it with publication strategy? Not yet, but considering.
Studio will be published end of this month.
Wrapping crappy scripts in CWL doesn't make it FAIR.
Teaching to code properly comes first. 
Reusability is improved but what about the other FAIR aspects? Not in our hands.

--------
Discussion panel:

SciWIn is only part. We need fair data. E.g. via the search hub. Clear connection between workflow and data.
Search Hub Middleware already available? Yes.
Bottom of Search Hub you find a survey.
Would DWD also use tools of FAIRagro for their data analyses? Some already use workflows etc. But good idea to use more useful tools.
re3data: what data selected? Feedback to re3data is given, etc. about repos not yet in re3data
AI enriched metadata first only in the seach hub to evaluate how community likes it. It could be fed to middleware so it can be re-used by others.
Incubator with TS4NFDI running next half year (Daniel) Glossary is a possible candidate.


Matthias: Tools at TRL 7-8 but tools have to brought to some kind of portfolio so that users can find and use them.

------------
--------------
Day 2
Timo Mühlhaus:
**Keynote:** Enabling Institutions and Community Members through the ARC Research Data Management Framework

Fair Diigita Objects to go from data to knowledge
E.g. in Plant science more than 600 digital technologies. Nobody can handle this and itt's not feasible to have data stewards doing all this

Immutable yet evolving
FAIR like unicorn. Nobody has seen it in full.
Platform like GitHub with quality badges
- works with collaborative workflows
- automatisation: build and validated. Whenever you sync a build process is triggered and is transformed to a FDO
- ARC is an RO-Crate
- RO-Crate is missing how data came to life. 
- data souvereignity. everything is a file and in your hands
- tools can be layered on top of this stack
- Tranining material 
Is it possible to retrofit objects to ARC?
- continous data
- catalog data
- asynchronous bach data -> ARC is well fitted here

Daniel Arend (IPK Gatersleben)
**Data Journey on the back of ARCs**
Generic ISA data to harmonise
ARC is metadata only. Files stay in original place. Cost effective for infrasrtructure.
RDI autonomy can stay as is.
UC13 connects two infrastructures
- ARC can harmonise datasets from RDIs and UseCases
- see publication
-> Middelware

**FAIR digital objects arriving in the user’s hands: ARC-based datasets in the Search Hub and SciWIn** 
_(Julian Schneider & Antonia Leidel, FAIRagro)_

How do ARCs and FAIRagro SearchHub interoperate?

What's advantage to Galaxy? Galaxy cannot run CWL workflows (yet)
Are workflows always running in container? no, but remotely it's better

**From Field Data to FDO: An ARC Quick Tour**  
_(Dominik Brilhaus, HHU)_

- ARCitect GUI for ARC
- potato drone infection demo
- downloads ARC (git clone)
	- to add drone photos: add new assay,
	- copy photos -> unstructured data, 
	- add tabular relation 
	- template for drone flight for metadata, fill out
	- git push
Antonia has a workflow to extract metadat from drone photos

**FAIR Standards Inventory**
_(Nils Reinosch, FAIRagro)_

- ontologies are fair
- AGROVOC
- link to OWL
- labels from AGROVOC in csv file for searching
- lowest level concept of a multilayered approach
- will integrate with terminology server

**From Papers to standardized metadata: AI-supported workflow for Extracting Knowledge on Agricultural Long Term Experiments**
_(Susanne Lachmuth, FAIRagro)_
 - LTE Overview Map to identify long term experiments
 - TrialHarvest-AI 
	 - python pipeline
		 - convert pdf to md
		 - prompt factory specific prompt to avoid hallucination
		 - Multi-LLM extraction per metadata category
		 - raw json output
		 - validation module with AGROVOC
		 - evaluation model to rate extraction
		 - ouput: validated reslults
	- mapping to predefined terms works for narrow concepts
	- prompt engineering is deterministic
	- has to be validated for ground truth
	- GDWG models

**Enabling high throughput crop growth simulation with SciWIn**
_(Joseph Gitahi, TUM)_
Crop models are data hungry
Using SciWIn
- different tools for image processing, pheonlogy etc.
- raster2sensor, phenocover, csm 
- python, and other langs
- commandline interfaces for tools are needed
- then dockerising the tools
- connected inputs and outputs
- CWL can be used with AI-assistance

**Quality Assessment of Agricultural Time-Series Data: A Demonstration of the DQ Tool** 
_(Sven Gedicke, FAIRagro)_

- quality problems become obvious later
- -> in-field quality controll to address issues early on
- lowering the barrier to uploading quality information
- light-weight algorithms needed
- sliding windows technique also applicable to spacial data
	- select column to analyse
	- immediate statistics
	- k-order, trucated k mean
	- Local Outlier Factor
	- download stats as XML
------------
Discussion:
Is there a timeline for putting all the tools together?
- something for the 2nd phase
- is ARC also for long-term accessibility
	- immutabilty comes from whenever you store : history freeses the underlying data, stored in Invenio and frozen. No tool is a lock in - so we think it's very future proof
	- process model under the hood. CWL process part fits this core process model. Focussing on the process model you do not need to know additional types. ISA
- RDM gap: how to reach out to researchers?
	- students love it
	- digital lietracy: chronological making notes
	- making data the first citizens: you have to order them, invest 5h to make your dataset long living
	- journal for ARC? talking to Metabolite, Nature uses ISA it is a subset. Considering issues etc. is still a long way.
------------
Bridging the gap between RDM support and research
**Keynote:** Bridging the gap between RDM support and Research.  
_(Shauna Ni Fhlaithearta, WUR)_

Talked to Harald von Waldow (Thünen) developing the SciWIn Workflow writing tool, about LTA

The Gap:

- Metadata standards
- privacy, data-integration, etc.  Integrated Compliance 
- Research IT Hardware and Capacity
- systematic causes:
	- WUR 4TU.ReserchData
	- rew3data
- carrot and stick: ?
- Embedded Data stewards
- for discussion:
	- How FAIR is FAIR enough?
	- Is FAIR RDEM a research field?
	- can we demand that cultural change starts at the top?
	- Clarify the role and responsibilities  of fiffernet flavours of data steward
	- Kill this idea: "build it and they will come"

**GreenRobust Cluster of Excellence**   
_(Karl Schmid, Uni Hohenheim)_

- nfdi, dataPLANT, Microbiota, FAIRagro, ...
- labNotebooks eLABFTW
- concentration on theory to discover new mechanisms for robustness
- using ARC
- create data across bilogical scales, Omic data
- machine learning and AI
- want to contribute to 2nd phase of FAIRagro


added value of links to different consortia?
using de.NBI infrastructure 
integrating multimodal data 

**LIA – A Digital Infrastructure for Field Trial Data**   
_(Nanina Tron, Julius Kühn-Institut)_

- handling of field trial data for all stages of RDM lifecycle
- from Excel fo DB often difficult
- POSTgres DB with Dashboard

**From Field to Formula: Making Agricultural Models FAIR with MathModDB**  
_(Marco Reidelbach, ZIB/ MaRDI)_

- MathModDB and MathAlgoDB
- come with a research question and be provided with a mathematical model
- how to add models to MaRDI KG
- MaRDMO client allows standardised documentation of the model -> published on the MaRDI KG 
- planning to have a first model by AI reading a uploaded research paper

**A practical guide for tending to repository metadata in re3data**   
_(Charlotte Neidiger)_

www.re3data.org
info@re3data.org
Mastodon: re3data@openbiblio.social
Bluesky

**From Planning to Practice: Research Data Management in the WetNetBB Project**   
_(Asim Khawaja, ATB Potsdam)_

- experiences as Research Data Manager
- What DMP is depends on how you treat it.
- Standard Operating Procedure
	- data audits
		- not punitive
		- reflective and collaborative
		- identify gaps
		- top down approach
		- talk to each individual
	- Governance needs an infrastructure
	- impacts: clear accountability, metadata consistency, legal compliance

Gespräch mit Timo Mühlhaus über ARC:
Eignung für LTA ist gegeben, da an keiner Stelle ein Lock in entsteht. Es gibt immer alles in input/output files die einem JSON-LD Graphen entspricht. ARC kann auch aus einem unvollständigen Grafen den Stand mit allen Files reproduzieren.
Man braucht weder die Infrastuktur noch den Graphen, um die Daten wiederzulesen. Sie sind zu jedem Zeitpunkt gut beschrieben und nach allgemeinen Standards gespeichert. 
Wenn etwas nicht von Beginn an in FAIR Format vorliegt, ist die Transformation der erste Schritt im Workflow.
Dirk von Suchodolez, Speaker of DATAplant is specialist.

	#ToDo Contact Dirk von Suchodolez
Good format with short presentations
Little time for poster session
Little talk of users, healing boards etc.

Good step forward. Many outputs.
Progress Report for 1st phase submitted end of February. Symposium on July 7th
Proposal for 2nd funding phase 
writing process: writing and review teams formed
new disciplines taken on boards: Animals and forestry
Consolidation: Biodata ... photo
Deadline not clear now Feb 27?
Sept. 2-4 Gatersleben

Biodata Community Conference
Feb/March 27 FAIRagro Plenary
Sept 2027 3rd CoRDI

Wissenschaftsratsbericht Recommendation to continue NFDI
some need discussion: ongoing 
- Safeguarding of domain expertise and community-driven infrastuctures : how much centralisation? Community branding; Good balance needed
- Sustainable Operating and funding model 
	- about people or flagship dataservices that have international visibility -> gap too large
- Clarifying governance structure

