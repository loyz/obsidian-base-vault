Kilian Schwarz, Inga Lakomiec, Frank Förster (Gießen de.NBI Administrator), Sebastian Wozniewski (PUNCH, Arun Data), Alexander Sczyrba (Jülich, Uni Bielefeld, Microbiota FAIRagro Base, de.NBI Cloud Infrastruktur für Lebenswissenschaftliche NFDI Konsortien), Sebastian Jünemann (Jülich), Björn (später, mittags)
Arnulf Quadt (Gastgeber)
Göttingen hat NFDI Storage gewonnen, User werden noch gesucht. NHR soll als Resource mit in Antrag aufgenommen werden. 
Bereits 2x eingereicht. Mit Vorschlag der Verbindung von 2 unterschiedlichen Infrastrukturen. 
Soll auf breitere Basis gestellt werden. 
(DFG Storage: LMU, Aachen, Göttingen)
Liste vom TEC mit Konsortien die Cloud Infrastrukturen haben / Muss gecheckt werden.
Supercloud.png (in MC Base Antrag Ordner: 3 Jahre alt)
![[Supercloud.png]]

Governance sollte von OA kommen.
Nutzer beantragt Ressourcen und weiß nicht
Overlay Batch System, mit 5 Standorten, Open Stack, HPC, HTC
HTCondor Matchmaking. (Scheduling und Matchmaking, der User kann Requirements stellen und entsprechend wird es zugewiesen.)
Konzept von Services. (Z.B. jemand will Webserver auf VM betreiben)
Kubernetes an einem Standort, an einem Galaxy.
Bild ist alt. Über REANA kann man mit Interlink SLURM mit User Credentials verschieben.
=> Bild muss neu gemacht werden.
Mit dem OA Diagram beginnen.
MC bei Resource Federation bestehend aus HPC, Virtual Compute und Storage 
2-3 Standorte dazu, 

Ganze Bandbreite abdecken ist nicht möglich.
Aber größere Bandbreite von Skalen abdecken.
Übergänge von Posix und Nicht-Posix organisieren. 
Wenige Services, die alles abdecken. Tiefergehendes Stack.  
Wichtig ist nicht das Geld sonder das Mandat. (Kilian)
Lohnt es sich einen Antrag zu stellen. 
Sollten auck die kleinen Konsortien abholen.
Fertig zusammengeschaltete VMs, 2-3.
Wen adressieren? (Alex)
Reproduzierbarkeit (Harry)
Wenn VMs nur virtuelle Laptops sind, dann ist es nicht reproduzierbar.
Sollte weniger technisch sein, sondern UseCase und Motivation vermitteln. 
Gelber Bereich ist klar gesetzt. 
Plattform - reproducible environment - soweit schon gesetzt 
unten bereitstellen ()
Storage Call: von 9 die durchgegangen sind kommen 6 aus NHR
Galzxy, invenio, IAM sind im NFDI EOSC Knoten. Wird Service Provisioning der NFDI beeinflussen.
z.B. Caching, 

Use Cases:
Cloud auf mehreren HPC
Harry Reproduzierbarkeit
Philipp: S3 Storage Call
Data Analyze von CMS und Atlas reinschreiben 
Über Nextflow können Workflows auf NHR laufen.
NHR denkt mehr in global verteilten Dateisystemen, etc. 
Singularity, lokaler Speicher genügt aber nicht.
In verteiltem System verarbeiten und reproduzierbar wieder zurückbringen.
Nehmen wir da alle mit?
Erstmal Resourcen verbinden, dann reproduzierbar machen. 
In-kind muss klar reingebracht werden. 
Es gibt bereits Prototypen in unseren Communities.
Auch sehen was wir von EOSC aufnehmen können (Harry)
Cloud Richtung HPC, wenn Bedarf ist massiv skalieren in ein HPC System 
aber warum sollte HPC sich an MC beteiligen? Tier2 Anfragen, echte Dienste Webservice laufen zu lassen. (Weil sie kein Konzept haben wie sie Workflows auf HP)
Aachen, Göttingne haben eh schon ein breites Spektrum.
Anwendung in Containern haben und dann auf alles Zugriff haben (S3, Slurm)
Im BE über HPC? egal
Cloud bietet Kybernetes Cluster an? Nein nicht nur. 
SLURM gemanagedes Cluster 
Preprocessing auf S3 und VM und dann ..
User müssen sich heute in ganz viele Infrastrukturen einarbeiten.
Viele verbieten nach Außen gehen. 
Man bringt Daten auf S3 zu HPC 
Sebastian: Jetzt schon Verbindung zu PUNCH,  aber geht wegen Governance nicht 
TFGS, 
Idealfall: Workflow mit einer UserID laufen lassen auch wenn er verschiedene Ressourcen braucht.  (Braucht sauberes Scheduling)
Große Gruppe von AI Anwendern, die nicht wissen dass sie VM batch brauchen.
LifeScience ID muss als Community ID gemappt werden. 
Governance Themen 
Anforderungen an verschiedene NFDI AG:
IAM ist Zusammenfassung von vier IdentitiyProvidern. 
NHR ist auf große Volumen und lange Dauer angelegt. Für kurzfristige Speicheranfrage nicht geeignet.
Ganze Konsortien für de.NBI und NHR enablen. Der Nutzer ist im Pool. 
Welche Services wollen wir als MC zur Verfügung Stellen?
VMs, HPC Cores,
HEP data, public data
oder zutrittsbeschränkte Daten
Ist das nur ein UseCase: nur zu demonstrieren, dass das geht 
Nur ein Workflow t
Inkubator Konzept zur Integration von Services.
Komponenten müssen austauschbar sein.
Offensiver sagen, dass es nicht nach Beutegemeinschaft aussieht. 
April in Aachen auf OA Namen für WorkPackages vorstellen
Feedback einsammeln

Arbeitspakete
- Community Engagement

Mindestens einen zusätzlichen Use Case über Community Engagement
Nachhaltigkeit: Unterschiedliches Funding der Partner

Neu: Service Provisioning mit NHR verheiraten
HPC Resourcen so einfach benutzen wie 

CloWM läuft auf virtuellem SLURM, den durch einen reellen ersetzen. 
Dasselbe  mit PUNCH 2.0

Betonen, dass MC das für alle ausrollt:
Mehr Gewicht ggü NHR - dafür braucht es den Auftrag

API zur Cloud um Jobs zu schedulen
USP: Nur noch ein Ansprechpartner
noch nicht konsolidiert, was alles läuft, und kein Plan für die Zukunft
=> konsolidieren, Onboarding Procedure
Single Point of Contact
Governance für alle

Kilian schickt Google Drive Link rum 
Material um Service Deployer zu schulen : Ansible Schulung.  EKaCD und de.NBI (in-kind) 
