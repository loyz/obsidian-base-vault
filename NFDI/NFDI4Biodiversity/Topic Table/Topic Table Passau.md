19.05.2026

Fragen HistOrniGraph / Austausch mit Tobias

bei Validierung

- unleserlich in {}? 
  - '[?]' for single letter
  - '[illegible]' for word
- font color z.B. <u><font color="#FF0000">Fringillidae</font></u> lassen? Bei Registerband 35 gibt es allerdings noch viel mehr unterschiedliche Tinten Austausch mit Tobias
- Belegexemplare in den SNSB
- GitHub HistOrnigraph 
  - mit run.py starten
  - input und output flags ändern etc.
  - NER bereits im repo
- Chandra 
  - über colab (Google): 'pip install -q candra-ocr vllm markdown'
  - method vllm ist besser
- Nächste Schritte 
  - Postprocessing 
    - regelmäßige Fehler bereinigen
    - Liste aller Vögel
    - Idee: eigener Prompt für Registerband (nur Vögel)
    - möglichst schnell Liste mit Arten
    - welche sachen sind irrtümlich unterstrichen?
    - Ansatz: alle unterstrichenen Token mit der Liste der Arten abgleichen?
  - Zenodo Literaturdatenbank
  - Ontologie festlegen
  - Vogelgesänge
  - Georeferenzierung (Geonames)
- Gespräch Ornithoportal
  - min. Auflösung 1 × 1 km
  - Vogelverhalten
  - Überflug
  - 

## Vorträge: Rethinking Historical Biodiversity Knowledge: Data, Methods, and Perspectives

Begrüßung durch Barbara Ebert

- historical data one of the identified topics of high interest
- topic table follow up for use cases Storyline: 1st data rescue for climate data

1. Atmospheric Circulation Reconstructions over the Earth (ACRE) - an overview of the international initiative (Rob Allen – ACRE)
   - https://www.met-acre.net/index.htm
   - www.met-acre.net
   - 3 elements 
     - recovery of international weather data (focus on before WW II)
     - dynamical 4D historical reanalyses (weather reconstruction), especially the 20CR, now back to 1806
     - climate services and application communities
   - data fed into internatioal repositories
   - umbrella for different projects
   - number of individual regional data rescue foci
   - ECA&D for Europe and Germany
   - early recordings: 
     - Mannheim Socieatas Meteorologida Paltina 1781-1792
     - Bayerische Ephemeriden 1781-1789
   - citizen science: weather detective
   - WInds, Waves and Storms for non-instrumental data
   - hand in datasets via EU Copernicus reach out
2. Transparency as a Method: How a Formal Workflow Makes Source Analysis Reproducable and Automated (Franck Schätz, Rüdiger Glaser – Universität Freiburg)
   - Transparenz ist die Methode selbst
   - 3 Quellengruppen 
     - gesellschaftsarchive
     - instrumentelle daten
     - natürliche Archvie
   - Gesellschaftliche Dimension: wie verletzlich sind Gesellschaften hinsichtlich Klimaereignissen
   - Historische Klimatologie 
     - spacial - temporal diagram (see photo)
     - aus Zeitung -?-> (Event, Time, Place, Event Intensity) / wie kommt man zu quantifizierbaren Ereignissen
     - Muster liegen in den Daten selbst
     - für Unwetter gibt es keine Referenzlinie
     - a text is a text / Nichtwissen ist bidirectional / wir wissen weder ob wir falsch liegen, noch ob wir richtig liegen
     - Issues in source analysis 
       - Finding sources
       - diverse source types with individual logic
       - language stage differ
       - transition from text to tupels
       - labor-intensive, expert-dependent
       - traceability and reproducibility are lacking in current practice
       - => Grenze des Wissens man weiß nicht ob zum Zeitpunkt x in y ein Gewitter war
     - Where we're going: 
       - Regeln werden zu Beginn (ex ante) aufgesetzt und nicht für jede Quelle individuell; bei Regeländerung wird wieder alles analysiert
       - Nachvollziehbarkeit
       - Wiederholbarkeit
       - Reihenfolge der Schritte ist entscheidend. Kann sich von Quellentyp, Sprachstufe unterscheiden
       - Zyklen vermeiden
       - formale Spezifikation der Arbeitsschritte
       - algorithmische Ausführung
       - alle Schritte werden zwischengespeichert
       - inter-annotator agreement Metrik (wichtige Metrik)
3. Historical-Ecological and Archaeological Perspectives: The case of Indigenous Forest Management in the Pacific Northwest (Chelsey Armstrong – Simon Fraser University, Kanada)
   - historical ecology 
     - eastern Europe, eg. Peter Zabo difference: 
       - Europe: history to learn about ecology / other parts of world: the other way round
     - importance of people in shaping the function and structure of the land. Only know that even land seemingly "wild" or "untouched" has been shaped by indigenous people / or has co-evolved
     - anthropologists have studied Pacific North West 
       - supposedly without agricultural land use
       - influencing laws etc.
       - but people acitively engineered their ecosystems
     - Documenting Forest Management: Biophysical Processes and Cultural Patterns 
       - look at the forst state and ask: how did it become this way?
       - do away the dichotomies cultural/natural
       - eg. ancient plant translocation, e.g. hazelnut (roots for blue dye) Paleobiolinguistic: 11 indigenous languages in BC => ancient hazelnut management resulted in genetic variation and distribution that can be found today
       - Forest Gardens in British Columbia
       - when cultivation of forest gardens stops conifers move in and wipe out diversity
       - pH 3.99 is a tipping point where soil can hold more nutrients
       - "sources" in historical archaeolgy - laetiicia Navarro