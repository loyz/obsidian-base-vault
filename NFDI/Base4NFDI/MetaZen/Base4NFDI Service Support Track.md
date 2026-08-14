---
type: coding-project
tags:
  - Base4NFDI
  - basic-services
  - nfdi
  - KnowledgeGraph
  - Django
timestamp: "1783612718"
---


Setup with Cursor



prompt:
Ziel:
Entwicklung einer Web-App zur Verwaltung von Basisdienstkandidaten. Die App soll ein Self-Assessment Tool für Basisdienstkandidaten beinhalten und eine Dokumentation erstellen.

Funktionen der App:
1. Benutzeranmeldung:
   - Anmeldung über Identity and Access Management (IAM)
   - Erstellung eines Accounts mit folgenden Anforderungen:
     - Name
     - Institution
     - NFDI-Konsortien (ausgewählt durch Ontologie)
     - Rolle
       - Serviceteam
         - Admin
         - Mitglied
       - Basisteam
         - Admin
         - Mitglied
         - Rolle
           - SER
           - SLO
           - TA1-4

2. Erstellung des Serviceteams:
   - Hinzufügen von Teammitgliedern mit Rollenverwaltung
     - Admin kann Rollen im Team bessern, Basisteam-Admin kann alles bearbeiten
   - Eingaben für das Serviceteam:
     - Name des Services (inkl. Akronym, falls zutreffend)
     - Kurze Unterüberschrift zur Erklärung der Hauptfunktionen
     - Entsprechender NFDI-Bereich
     - Leitinstitution
     - Name des verantwortlichen wissenschaftlichen Mitarbeiters der Leitinstitution
     - Weitere beteiligte Institutionen (falls zutreffend)
     - Gewünschte Dauer des Projekts (max. 6 Monate)

3. Bewertung der Servicebereitschaft und Unterstützung:
   - Interaktives Fragebogensystem, das durch relevante Fragen führt
   - Verlinkung zu geeigneten Materialien für jeden Schritt (mit Checkbox “verstanden”)
   - Zusammensetzung von Checkboxes und Texteingabefeldern in einem Bericht:
     - Format: A4, 11 pt Arial, einzeilig
     - Maximal zwei Seiten, exklusive Anhang
     - Der Bericht dokumentiert:
       - Servicebereitschaft: Welche Module sind bereits abgeschlossen
       - Servicebedarf: Welche Anforderungen stellt der Service für diesen Vorschlag

4. Zusätzliche Funktionen:
   - Suchfunktion für Informationsmaterialien mit Anzeige der entsprechenden Papiere
   - Die Felder für Benutzer- und Teamkonten sowie die Klassifizierung der Papiere basieren auf der erweiterten NFDI-Core-Ontologie, unter Verwendung der TS4NFDI-Widgets (Dropdowns) wo möglich.

Workflow zur Entwicklung der SST-App:
1. Ontologie (SKOS ConceptScheme)
2. Klassifizierung/Vektorisierung von Zenodo-Dokumenten mit intelligenter Suchfunktion
3. Interaktives Fragebogensystem zur Selbsteinschätzung mit Berichtserstellung
4. Implementierung der Anmeldungs- und Kontoerstellung