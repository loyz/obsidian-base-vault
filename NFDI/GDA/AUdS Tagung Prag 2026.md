#Archiv #digitaleUnterlagen #LTA
18./19.März

BBAdW
Leitlinie 17
Forschungsdaten der Akademie
- Bewertung vs. Vollständigkeit
- wissenschaftlicher Wert
- auch Auswahlprozess
- Angusd Whyte, Andrew Wilson How toAppraise and Select Research Data for Curation
- Langfristige Ermöglichung von Interoperabilität und Wiederverwendbarkeit
- Archivierungsmatrix: Bewertung nach dem Geldbeutel?
	- verschiedene Herangehensweisen (Personenmonate)
	- Archivierungsstufe/Servicelevel -> foto
- wie mit Forschungsdaten und digitalen Services umgehen?
	- digitale Editionen
	- Metadatensysteme -> Aufwand zur Betreuung Komplexitätsgrad (Service Level)
- Digitalisate als Forschungsdaten
	- Langzeitsicherung nach Abschuss der Edition
	- Überlieferungsbildung vs. alles gebündelt aufbewahren (Proveninenzprinzip, institutionelle Zusändigkeiten)
		- sind bereits bei Herkunftsorganisationen bereits archiviert
		- Redundante Speicherung
		- andererseits: Erleichterung der Forschung
	- Beispiel aus Kant Opus postumum -> Strukturiertes Layout
		- Referenzen erfassen und kuratieren
		- kontinuierliche Kuratierung notwendig
**16 Jahre gemeinsame Software-kooperation und die Erfahrungen daraus (Claire Röthlingsberger-Jourdan)**
- KOST (Koordinationsstelle Schweitz und Liechtenstein)
	- Unterstützung bei der Archivierung digitaler Unterlagen
- Wann Software entwickelt wird
	- Ad-hoc Scripte (nicht publiziert und gepflegt)
	- Prototypen (PoC) 
		- z.B. csv to SIARD (wurden abgelöst durch bessere Tools oder kommerzielle Tools)
	- Daueraufgabe (zjBl Qualtitätssicherung)
- Warum?
	- Vermittlung von Fachwissen
	- lieber Code als lange Anweisungen (bessere Form von Fachwissen) Hilfe zur Selbsthilfe
- Wie?
	- Input kann von Archivar kommen. 
	- Konzept /Pflichtenheft/Kontrolle
	- Productowner und Entwickler haben gleich viel Arbeit
	- Anpassung bestehender Software -> durch Informatiker / hoher Aufwand
	- Komplette Eigenentwicklung
		- Software-/Applikationsentwickler
	- Initialkosten / Redesign
	- Weiterentwicklung (Architektur entfällt)
	- 0,6 FTE (eine Frau,  aber 1/3 der Geschäftsstelle)
	- Support eingeschränkt 
	- Nicht erwartete Gründe:
		- Technologischer Wandel (Security)
		- Erfolg
	- KOST-Tools
	- Ab April sollen PDF-Dateien auch reparieren können!

**Archiving by Design: wie gute Systeme gute Archive schaffen**
Vincent van HOOLT (Nationalarchiv der Niederlande)
Archivierung beim Entwurf
- Warum?
	- digitaler Wandel
	- digital soll für alle besser sein!
	- Legitimität / Organisation / Öffentlicher WErt
	- Welt arbeitet nicht in Akten
	- Integrierte Archivierung in Quellsystemen bzw. digitalen Systemen
	-
- Was?
	- Bei der Gestaltung oder Anpassung von Informationssystemen geeignete Maßnahmen treffen. Mit am Tisch sitzen.
	- Qualitätsmerkmale
		- auffindbar
		- aufrufbar
		- Lesbar (Archivierung von Windraddaten deren Format dem Archiv nicht bekannt ist)
		- Interpretierbar (=Metadaten)
		- Zuverlässig (Art und Weise der Überlieferung)
		- langlebig 
		- zugänglich
- Wann?
	- Organisation
		- Aufstellen von Informationsarchitekturen
		- Entwickeln von Massnahmen und Richtlinien
	- individuelle Projekte
		- Einkauf
		- Bau
		- Änderung und Anpassung
		- Migration
		- bei Projekten dabei sein
- Wie?
	- Whitepaper
	- AbD Scan
		- Anforderungen definieren
		- Qualitätsmerkmale
	- 10 Anforderungen für jedes System
		- Description
		- Objective
		- Implementation
		- Questions
	- DUTO scan Canvas
				- Benutzer
					^
					|
		- Prozess -> Information <- Systeme
	- Dialog mit Bürgern ist sinnvoll, denn die Systeme sind für die Bürger da

**Entwurf für einen nestor-Standard zur Aussonderung von archivwürdigen Informationender öffentlichen Verwaltung aus Dokumentenmanagementsystemen**
Julia KRÄMER-RIEDEL (Historisches Archiv mit Rheinischem Bildarchiv Köln)

- Idee, Genese, Ziele (Standardisierte Aussonderung aus DMS)
	- DMS Installationen haben unterrschiedliche Konfigurationen
	- Profgrammierung von individuellen Schnittstellen aufwendig
	- Inhalte vergleichbar
	- => klares Regelwerk möglich
- Rund mit Archivsparten und IT-Dienstleister aber nicht DMS Herstellerfirmen
- nach XDOMEA, wie sollen sie strukturiert sein, sinnvolle Verarbeitung durch Archivierungssysteme möglich
- Ziel: grundsätzliches Regelwerk für Archive, DMS Hersteller, Verwaltung
- Zusammenarbeit mit nestor AGs Archivstandards und AG xdomea

**Überlieferung von behördlichen Metadaten**
Uwe LEUENHAGEN (Landesarchiv Schleswig-Holstein)
- Archivische Metadaten -> AFIS
- Technische Metadaten (Medium, Dateifomate, Hahwerte) -> digitales Magazin
- Prozessuale Metadaten -> Verwaltung
- Behördliche Metadaten (Info aus Fachverfahren, Genehmigung, Nutzungsstatistik) -> Bestandteil des Archivobjektes
- Wie ins Archiv?
	- Als regulärer Teil der Abgabe
	- Als Inhalte in einem Transportstandard
		- Überführung in Datenmodell des Transportstandards (xdomea, xjustiz, ...)
	- Als zusätzliche Info
- Anzhl der Fachverfahren ist beliebig groß
- Originäre Feldnamen sollen erhalten werden wegen Interpretierbarkeit
- Generalisiertes XML Schema mit <entity> <dataset> und <field> wobei name genau der Bezeichnung im DMS entspricht.

**Langzeitarchivierung von Personaldaten und -dokumenten aus der Software SAP**
Claudia BRIELLMANN, Andres BUCHER, Stephanie WILLI (Hochschularchiv / Bibliothek der ETH Zürich)

**Von SIP (eCH-0160) zu DIMAG: Prozesse, Schnittstellen und Herausforderungen**
Béatrice GAUVAIN (Staatsarchiv Zürich)

- DIMAG kann nicht mit Schweizer Standard (eCH-0160)
- DIMAG Ingest Tool wird abgelöst
-  Backend Spring Boot -> Foto
- Felder mappen und erstellen
- Aus einem SIP mehrere oder AIPs bauen
- direkter Weg von eCH160 nach DIMAG

Barcamp 
**Brücken bauen: Die Schnittstelle des Tschechischen Nationalen Digitalarchivs mit Erschließungssystemen**

Fabian Näser

DIMAG-AFIS Connector
- Dokumentation
- Standardisierte Austauschmöglichkeiten (Ist xdomea ein Standard?)
- Kommunikation vereinfachen
- Systeminfrastruktur überall anders (Einzelinstallation, Verbundinstallationen)
- IT-Sicherheit und Kommunikationsstandards
- Fehlende Kommunikationsplattformen zwischen Beteiligten
-  (Vorbild EAD-AG)
- Kerndatensatz von Daten die aus dem AIP ins AFIS kommt?
	- nur noch eine ID als Verbindung geplant (Naumann)
		- aber beim INGEST über AFIS; dort werden dann Felder direkt ins AFIS gespeist
		- ID ist dauerhafte Schnittstelle/Verbindung
	- selbst mit RIC Ontologie wird es immer Abweichung geben (Näser)
	- Grundfrage: wie bekommen wir die Systeme überhaupt verbunden? (Eine Ebene höher) -> nestor AG Archivstandards? ()
	- Baden Würtemberg hat den Connector als erstes bestellt
	- Keine Massendaten verarbeitbar mit DIMAG Connector (Stadtarchiv Leipzig die DIMAG Connector gekauft haben) auch Landesarchiv Hessen und Niedersachsen.
	- Problem, dass DIMAG Kernmodul ganz verschieden installiert werden kann
	- Seit 1973 wird mit Bundesarchiv schon über digitale Archivierung gesprochen
		- Variante: Leute abholen wo sie sind. Heute 800 DIMAG Module im Einsatz
	- Andreas Becker (Regensburg): DIMAG ist Produkt in Entwicklung. Bewegte Vergangenheit. Kommunikationsbasis stärken. Auch funktioniert es nur mit einer VE. (Max VE = 1)
		- LAND hat Konkurrenzprodukt zu DIMAG: SORI
		- DIMAG ist vom Bund
		- Hessen nutzen eine einzige Mappingeinheit (statt wie ursprünglich gedacht ganz viele)
		- Wenn eAkten ins AFIS gebracht werden ist es nur eine Ersterschließung da z.B. die Laufzeiten differieren (Uwe Leuenhagen)
		- Christian Keitel (Landesarchiv Baden-Würtemberg): Leiter nestor AG Archivstandards und DIMAG
		- Zum Gesprächskreis lädt Herr Piskol aus Sachsen ein. (Info von Herrn Prof. Keitel)

**Spielerischer Workshop am Sächsischen Staatsarchiv – Fachverfahren: Von der Übernahme bis zur Nutzung**
Karsten HUTH (Sächsisches Staatsarchiv)

Schulung für die Übernahme von Fachverfahren mit Klemmbausteinen:
- Ein Objekt aus Lego wird der Gruppe intakt vorgestellt
- Nicht alles kann übernommen werden
- signifikante Eigenschaften müssen definiert werden
- Dokumentation erstellen. Schriftlich oder Zeichnung
- Einige Teile werden mit ins Archiv genommen
- Mit Anleitung und Teilen muss wieder zusammengebaut werden, wie das wieder in die Funktion gebracht werden kann. (2 Gruppen)
- Verständnis für wesentliche Eigenschaften entwickeln (Bei Reduktion)

**Analoge Prozesse digital adaptieren oder ganz neu denken? Konzept des StAGR zur Verarbeitung digitaler Ablieferungen von der Übernahme bis zur Erschliessung**
Flurina CAMENISCH, Georg Friedrich HEINZLE (Staatsarchiv Graubünden)
- Ingest:
	- als fertiges SIP (ideal) -> KOST-Val -> docu team feeder -> EAD ->CMI/AIS
	- Dateiablage etc. -> TreeSizePro
- Arbeitsschritte bei Erstellung eines SIPs (analog)
	- Kontrolle und Nachbewertung
	- Schlussbericht -> Abt. Erschließung
	- Ordnen
	- Konservatorische Maßnahmen
	- ...
- Digital:
	- Kontrolle und Nachbewertung
	- Ordnen gemäß Erschließungshandbuch
	- Schlkussbericht
	- finales SIP
	- Abt. Erschließung macht nur noch Kontrolle
	- Ingest
- Digitaler Prozess Neu:
	- mehr zurück zum analogen Prozess?
	- Vollständigkeitskontrolle und ggf. Nachbewertung
	- Nur automatisierte konservatorische Massnahmen
	- Schlussbericht und Dokumentation
	- Bilden eines Basis SIPs -> Abt. Erschliessung
	- dort: SIP nachbearbeiten, Daten für Erschliessung vorbereiten
	- Ordnen gemäß ERschliessungshandbuch, nochmalige Detailprüfung
-  =>Digital in der Abstraktion nicht so viel anders als Analog

**Digitale Barrierefreiheit als Voraussetzung für Teilhabe in der digitalen Archivierung**
Lukas HECK (Brandenburgisches Landeshauptarchiv)
- Alle Menschen haben das Recht auf Benutzung eines Archivs
- Website des VDAs Prof. Sr. Erdmuthe Meyer zu Bexten
- Digitale Bestände, Findmittel und Websites müssen für alle Menschen zugänglich sein
- Digitalisate -> angemessene Beschreibung,  Inhalt in einfacher Sprache
- PDF/UA Standard: Archivfähigkeit <- nicht automatisch -> Barrierefreiheit
	- PDF/A2, A3 -> PDF/UA-1
	- PDF/A4 -> PDF/UA-2
- Einfache Sprache
	- Verwendung von Sprachmodellen


**Kompetenzzentrum Geschäftsfallbearbeitung: ein Statusbericht aus dem Kanton Zürich**
Ayse KOCAKULAH (Staatsarchiv Zürich)

- Interoperable Schnittstellen SST
- Datensilos abbauen
- Fachapplikationen 1,2,3 -> DMS/ECM/Content Service 1,2 -> eCH160 -> Staatsarchiv Zürich 
- CMIS Standardschnittstelle/Hersteller Connectoren (sollen reduziert werden)
- CMIS nicht weit verbreitet wurde nicht von OASIS weiterentwickelt

**Einsatz von KI zur Verbesserung der Qualität der Nutzung und Verwertung von Datenbeständen im Historischen Archiv der Ungarischen Staatssicherheit**
Zoltán LUX (Historisches Archiv der ungarischen Staatssicherheitsdienste), Domonkos CZIFRA,
Peter KŐRÖSI-SZABÓ, Gábor KOVÁCS, Győző CSÓKA (Alfréd-Rényi-Institut für Mathematik)

- Archiv für Unterlagen aus Ungarischen Staatssicherheitsdiensten
- Entitätenerkennung
- Zusammenfassungen
- Interaktive Fragen
- -> Voraussetzung gut lesbare OCR Dokumente
- aber: oft schlechter Zustand der Dokumente
- KI Unterstützung bei OCR (Text Correction) und Named Entity Recognition
	- z.B Johann Schmidt -> welcher Record?
- Topic Recognition (zum Finden und Schwärzen Sensitiver Informationen)
- Schwer mit ABBY oder Tesseract
- RAG-Powered Chat
- high quality data is important
- Degraded Document Generator (for training)
	- Framweork pick language layout
	- Generate Dokument (tyewriter font)
	- Backgound Image 
	- Erosions Dilation
	- Gaussian blurring and noise
	- ... => complex examples
	- Millions of images to train
- Tasks:
	- Document Image Enhancement (DIE)
	- OCR
		- TrOCR
			- Line by line textdetection
			- Fast
			- Modular with different steps (clean detect text length, apply OCR)
		- LightOnOCR-2
			- Processing full pages
			- End-to-end
			- Slower
- AI Applications
	- Sensitive Data Removal
		- prompt: find sensitive parts and mark <Sensitive> and mask
	- RAG-Powered Chat
		- answer and source (highlightet)
- Fine-Tuning one day for language (multi-language models)

**Dezentrale Datenräume für ethische KI-gestützte Referenz und Zugriff in Kulturerbeeinrichtungen**
Victoria LEMIEUX (University of British Columbia), Matthias KAUN, Gerrit GRAGERT (Staatsbibliothek zu Berlin)

- Ki Bots scheren sich nicht um 
	- Datenschutz
	- Rechte
	- Datensouveränität
	- Kultureinrichtungen
- Bisher keine Antworten (Kgl. Bibliothek musste aus rechtlichen Gründen offline genommen werden)
- Neue Data Spaces!
	- Pontus-X
		- Datensouveränität\
			- Daten bleiben in Institution
			- Entscheidung über Datennutzung
		- Kein Vendor lock-in
		- Compute-to-Data
			- Verarbeitung dort wo Daten sind
		- Möglichkeiten der Monetarisierung
		- Gaia-X compliance -> Nachvollziehbarkeit der Datennutzung
		- Dezentral
		- Portal **CrossAsia**
			- lizensierte Quellen
			- Erlaubnis für Text- und Datamining
			- aber nicht für Download
		- Portal **Clio-X**
			- Web3 Data Space
			- decentral privacy first architecture 
			- e.g. Amazon S3 as storage
			- encryption: zero knowledge proof technology
			- data temporarily mirrored into the save data space
			- metamask wallet filled with tokens (for accounting) & blockchain logging
			- opportunity to share AI and use resources efficiently
			- data (and algorithm)remains with the archive (-> Foto)
			- Verfassungcharta (selfgoverning by archives and comunity)
			- 
**Graph-RAG und Regeln für vertrauenswürdigere LLMs**
Sven SCHLARB (Austrian Institute of Technology)

- LLM vs. Graph
	- neuro vs. symbolisch
- symbolisch: deterministische Wissensrepräsentation
	- explizit definiert (aufwendig)
	- Extrahiert (Rauschen, hoher Validierungsaufwand)
- Blackbox
	- auch chain of thought ist generiert, nachträglich
	- kleine Änderung im Prompt kann große im Ergebnis bedeuten
	- Halluzinationen: versteckte Falschinformationen, Verzerrrungen, Diskriminierung, Verachtiung, ... ; Guard rails dagegen
	- Maßnahmen: RAG, Quellennachweise; Human-in-the-loop
	- Chatbot Arena Leaderboard
	- Benchmark: e.g. Named Entity Recognition nur im Benchmark gut
- RAG Pipeline mit lokalen LLMs
	- Beispiel: Eoropäische Städte mit mehr als 2 Mio Einwohnern
	- SPARQL-Abfrage (muss auch korrekt sein)
	- Identifier: falsche QIDs (Wikidata) e.g. bei StartWars Figuren
	- LLM (agentic) ->  Funktionsaufrufe 
- Absicherung durch Regeln
	- Ausgabe von LLMs gegen Regeln mappen
	- => Nur Risikominimierung!
- Benutzung von Skills?
	- KIT Archiv (Klaus Lippert): User nehmen sich Digitalisate um eigene Modelle zu bauen

**Recherchemöglichkeiten von E-Mails mit der Software EMILiA**
 Elisabeth KLINDWORTH (Archiv der Max-Planck-Gesellschaft)

**A Work in Progress: Open-Source Digital Preservation Implementation for Research Data at the Deutsches Archäologisches Institut**
Juliane WATSON (Deutsches Archäologisches Institut), Katie PUNIA (Artefactual Systems)

- IANUS Project ab 2017 in NFDI4Objects
- Ziel: Nachhaltige Infrastruktur zur Langzeitarchivierung von Forschungsdaten
- aber keine Anschlussfinanzierung
- Ingest Szstem, Workflow basierte Validierung, OAIS compliant, PIDs
- WGs for GIS and 3D Data
- 