---
type: concept
title: Knowledge4Base
description: A RAG knowledge base for Base4NFDI
tags:
  - "#KnowledgeGraph"
  - "#Base4NFDI"
timestamp: "1783523422"
---
See also:
[[Workflow for adding additional metadata to Zenodo publications]]

Prompt for Monica (Sonnet 5):

- knowledge base for project Base4NFDI
- two document sources: Zenodo with pdfs or slides
- Google Docs on MyDrive from different owners
- A excel document with several tables that classify a (relevant) subset of the documents is attached
- some json_ld files (attached) derived from classifying a zenodo dump
- want to build a graph using NFDI core ontology as basis
- enable search eg. via a natural language interface for documents by:
	- author
	- topic
	- keyword
	- date
	- phase in research data lifecycle
	- target user group
	- phase in Base funding scheme
	- belonging/coming from/to task area
	- relevant for task area
	- relevant for basic service
	- mentioning consortium x
	- relevant for NFDI body x
- the DB should only store metadata to the documents and links to them
- the Google and Zenodo docs should be processed by an llm (via Anthropic API) to be tagged/classified
- script for json_ld
  
  Output
- # Ziel

Implementierungsguide für eine Wissensbasis (Knowledge Graph) für das Projekt Base4NFDI,

umsetzbar als Docker-Repo mit Jupyter Notebook, entwickelt mit Cursor.

  

## 1. Datenquellen

- Zenodo: [API/Dump-Quelle angeben] – Metadaten + [Volltext: ja/nein, Methode?]

- Google Docs (MyDrive, mehrere Owner): [google-api-python-client]

- Excel-Klassifikation: Rolle = [beides]

- JSON-LD (bereits generiert via Skript X)

  

## 2. Zielarchitektur

- Graph-Store: [Triplestore (Fuseki/GraphDB) | Neo4j] – Begründung: ...

- Docker-Setup: [docker-compose mit Services: ...]

- Jupyter-Rolle: [Prototyping | produktive NL-Suche | beides]

- Persistenz: [Volume-basiert | ephemer]

  

## 3. Ontologie

- Basis: NFDIcore [[V 3.0.5](https://ise-fizkarlsruhe.github.io/nfdicore/)]

- Erweiterung nötig für: Phase, Task Area, Zielgruppe, Konsortium, NFDI-Gremium

- Modellierung als: [SKOS ConceptScheme ]

- Ggf. Abstimmung mit TS4NFDI: [nein]

  

## 4. LLM-Klassifikation (Anthropic API)

- Zu taggende Facetten: Autor, Topic, Keyword, Datum, Phase (Lifecycle),

Zielgruppe, Phase (Base-Förderschema), Task Area (von/relevant für),

Basisdienst-Relevanz, erwähnte Konsortien, relevante NFDI-Gremien

- Prompt-Design: [iefern]

- Provenienz-Tracking: [ja, via prov:]

  

## 5. Suchinterface

- Methode: [ Hybrid]

- UI: [Chat-Widget & später Web-API]

  

## 6. Scope

- Dokumentenanzahl (ca.): 600

- Import-Modus: [ inkrementell]

- MVP-Umfang: [inkl. Suche]

  

## 7. Repo/Cursor-Kontext

- Bestehendes Repo/Template: [nein]

- Erwartete Cursor-Nutzung: [Schrittweise Prompts ]

PAT for Zenodo
'''fZJDXbhocmzqJSRBDQZiJhBsWkD2sJxSPLkSsqao0GEJreVInB8ZVT63TZpX'''
-----------------------------
