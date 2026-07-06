# NFDI: [[Aruna]] vs. [[ILDG 2.0]]

## [[Aruna]] Object Storage (AOS)
### Architektur
- Verteiltes [[Multi-Cloud]]-Objektspeichersystem
- Cloud-native, zentralisiert
- [[S3-kompatible Schnittstelle]]
### Zielgruppe
- Disziplinübergreifend
- Domänenagnostisch
### Einsatz
- [[NFDI4Microbiota]] (RDM-Preserve)
- [[Langzeitarchivierung]]

## [[ILDG 2.0]] (Lattice QCD)
### Architektur
- [[Föderation]] autonomer regionaler Grids
  - [[CSSM]] Australien
  - [[JLDG]] Japan
  - [[LDG]] Europa
  - [[UKLFT]] UK
  - [[USQCD]] USA
### Core Services pro Grid
- [[Metadata Catalogue]] (MDC)
- [[File Catalogue]] (FC)
- [[Storage Elements]] (SE)
### Governance
- [[ILDG Board]]
- [[Metadata Working Group]] (MDWG)
- [[Middleware Working Group]] (MWWG)
### Metadaten-Standard
- [[XML-XSD]] Format
- [[QCDmlConfig]] Schema
- [[QCDmlEnsemble]] Schema
- Neue Felder
  - [[ORCID]] Unterstützung
  - [[Lizenz]] mit Embargo
  - [[Funding Reference]] (DataCite-Style)
  - Erweiterte Eichgruppen (SU N, SO N, SP N, U N)
### Authentifizierung ILDG 2.0
- Migration von VOMS-Zertifikaten
- [[INDIGO IAM]] (INFN-CNAF)
- [[OAuth2-OIDC]] Token-basiert
- [[eduGAIN]] Föderation
### Storage-Zugriff
- [[WLCG-Profil]]
- Capability-based Autorisierung
- [[dCache]]/[[StoRM]] Middleware
### Dateiformat
- [[LIME Format]] Version 1.2
- Multiple Gauge-Konfigurationen
- QCD+QED Support

## Gemeinsamkeiten
- [[NFDI]]/[[PUNCH4NFDI]] Förderung
- [[FAIR-Prinzipien]]
  - Findability
  - Accessibility
  - Interoperability
  - Reusability
- Herausforderung große Datenmengen

## Unterschiede
### Architekturphilosophie
- [[Aruna]]: zentralisiert
- [[ILDG 2.0]]: föderiert/dezentral
### Spezialisierung
- [[Aruna]]: generisch
- [[ILDG 2.0]]: hochspezialisiert (Lattice-Physik)
### Historie
- [[Aruna]]: neu entwickelt
- [[ILDG 2.0]]: 20 Jahre gewachsen

## Konvergenz-Trends
- [[Token-basierte Authentifizierung]]
- [[Cloud-native Sicherheitsstandards]]
- Mögliche Erweiterung: non-Lattice Domains
- Zukünftige Integration [[generische NFDI-Dienste]]
