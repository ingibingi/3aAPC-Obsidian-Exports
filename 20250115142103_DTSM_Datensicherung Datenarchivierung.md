---
aliases: 
cssclasses: 
tags:
  - 3aAPC
  - ToDo/Submit
  - ToDo/Finish
date: 2025-01-15
deadline: 
hideFromQuery: false
link: 
info:
---
# Datensicherung und Datenarchivierung
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: ITLxx/Informatik
- Datum: 2025-01-15
---
## Notizen aus dem Unterricht
- Datensicherung
	- aka.: Backup
	- Kurz- bis Mittelfristig
	- Um Datenverlust zu vermeiden
- Datenarchivierung
	- Langfristige Speicherung von Daten
	- Jahre bis Jahrzehnte
- Restore
	- Wiederherstellung von Daten
- Probleme bei Archivierung
	- Hardware-Medium/Software ändern sich
		- Verfügbarkeit Lese-Gerät nicht mehr verfügbar

### Notizen aus Lehrgang 2
```
### Halbleiter
- Flash-Speicher
	- USB-Stick
	- SSD
	- SD-Karte
### Optische Datenträger
- CD
	- ca. 1980
	- ~500 MB
- DVD
	- ca. 1995
	- ~5 GB
- Blu-ray
	- ca. 2005
	- ~25 GB
### Magnetische Datenträger
- Kernspeicher
	- ca. 1950
	- "Moby Memory"
		- 1.2 MiByte
		- 175x127x64 cm
		- MIT ~1960
		- 380000 USD (über 3 Millionen USD in 2024)
- Magnetband
	- ca. 1940
	- IBM 726 "7-Track"
		- ca. 1950
		- ca. 3 MByte
	- IBM 2400 "9-Track"
		- ca. 1960
		- ca. 20 MByte
	- IBM 3400
		- ca. 1970
		- ca. 100 MByte
	- IBM 3480
		- ca. 1985
		- ca. 400 MByte
	- Datasette
		- Mobiler Datenträger
		- ca. 1980
		- 1 MByte
	- LTO
		- ca. 2000
		- 100 GB
- Diskette (Floppy-Disk)
	- Mobiler Datenträger
	- 8 Zoll
		- ca. 1970
		- 80 KByte
	- 3,5 Zoll
		- ca. 1980
		- 360 KByte
	- 3,5 Zoll ED
		- ca. 1990
		- 3 MByte
- HDD-Festplatte
	- ca. 1990
	- 1997: GB-Festplatten
	- 2008: Terrabyte-Festplatten
```

| Speichermedium             | Kapazität                                                                                         | Verwendung                  | Problem                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------------- | --------------------------- | --------------------------------------------------------- |
| 3.5" Floppy                | 360 KByte (1980)<br>3 MByte (1990)<br>1.44 MB                                                     | Mobiler Datenträger         | Empfindlich auf Magneten                                  |
| HDD-Festplatte             | x GB (1997)<br>x TB (2008)                                                                        | PCs                         | Empfindlich auf Erschütterung                             |
| Kernspeicher (Moby Memory) | 1.2 MiByte (1950)                                                                                 | Supercomputer               | Groß, Sehr(!) teuer                                       |
| SSD                        | 8 TB (2024)                                                                                       | PCs                         | Begrenzte Schreibzyklen                                   |
| Magnetband                 | 3 MB (1950)<br>20 MB (1960)<br>100 MB (1970)<br>400 MB<br>(1985)<br>100 GB (2000)<br>18 TB (2020) | Langzeitspeicherung         | Teure Schreib/Lese Hardware                               |
| Datasette                  | 1 MB (1980)                                                                                       | Mobiler Datenträger         |                                                           |
| USB-Stick                  | MB-GB                                                                                             | Mobiler Datenträger         | Wird immer falsch herum reingesteckt (vor USB-C Standard) |
| SDHC-Karte                 | bis 2TB                                                                                           | Aufnahme von Bildern/Videos |                                                           |
| CD                         | ~0.50 GB                                                                                          | Archivierung                | Begrenzte Lebensdauer                                     |
| DVD                        | ~5 GB                                                                                             | Archivierung                | Begrenzte Lebensdauer                                     |
| Blu-Ray                    | ~50 GB                                                                                            | Archivierung                | Begrenzte Lebensdauer                                     |
## Sicherungskonzepte
### Komplettsicherung
- auch Vollsicherung genannt
- Vorteile
	- vollständiger Datensatz
	- leicht wiederherstellbar
- Nachteile
	- Zeitaufwändig
	- Hoher Speicherbedarf
### Differentielle Sicherung
- Änderungen relativ zur letzten Vollsicherung werden gesichert
- Jede neue Sicherung beinhaltet jede Änderung bis zur letzten Vollsicherung
- Mittlerer Speicherbedarf
### Inkrementielle Sicherung
- Änderungen relativ zur letzten Inkrementellen Sicherung werden gesichert
- Wiederherstellung verglichsweise aufwändiger
- Geringster Speicherbedarf
### 3-2-1 Regel
- 3 Datenkopien
- 2 Medien (z. B. Festplatte & DVD)
- 1 Kopie an anderem Ort (z. B. Privete / Public Cloud)
### Hybrid Cloud
- Mischform Private und Public Cloud
### Großvater-Vater-Sohn
#### Beispiel
zusätzlich "Großvater" für Archivierung
- 4 Sohn-Festplatten (Tag)
	- S1...Montag
	- S2...Dienstag
	- S3...Mittwoch
	- S4...Donnerstag
- 4 Vater-Festplatten (Woche)
	- V1...1. Freitag im Monat
	- V2...2. Freitag im Monat
	- V3...3. Freitag im Monat
	- V4...4. Freitag im Monat
- 12 Großvater-Festplatten (Monat)
	- G1...1. Jänner
	- G2...1. Februar
	- G3...1. März
	- ...
	- G12...1. Dezember
- ? Urgroßvater-Festplatten (Jahr)
  evtl. nicht überschreiben, um Archivierung zu erhalten
	- U1...01.01.2021
	- U2...01.01.2022
	- U3...01.01.2023
	- ...
- neues Backup einer Generation überschreiben die älteren
	- das neueste jeweils das älteste des jeweiligen Levels
- -> Man hat:
	- Tägliche Backups der letzten (4+1=) 5 Tage
	- Wöchentliche Backups des letzten Monats
	- Monatliche Backups des letzten Jahres
	- Jährliche Backups zur Archivierung
### Türme von Hanoi
- Unterschiedliche Medien
- Älteste Sicherung vor $2^{n-1}$ Tagen
	- n... Anzahl Speichermedien


| Tag | A   | B   | C   | D   | E   |
| --- | --- | --- | --- | --- | --- |
| 1   | x   |     |     |     |     |
| 2   |     | x   |     |     |     |
| 3   | x   |     |     |     |     |
| 4   |     |     | x   |     |     |
| 5   | x   |     |     |     |     |
| 6   |     | x   |     |     |     |
| 7   | x   |     |     |     |     |
| 8   |     |     |     | x   |     |
| 9   | x   |     |     |     |     |
| 10  |     | x   |     |     |     |
| 11  | x   |     |     |     |     |
| 12  |     |     | x   |     |     |
| 13  | x   |     |     |     |     |
| 14  |     | x   |     |     |     |
| 15  | x   |     |     |     |     |
| 16  |     |     |     |     | x   |
| 17  | x   |     |     |     |     |
# Datenschutz
- Datensparsamkeit
	- nur zwingend benötigte Daten verwenden
- Vertraulichkeit
	- Daten nur an Befugte.
	- Kein Zugriff durch Unbefugte
- Datenintegrität
	- Keine Manipulation/kein Löschen der Daten
	- auch nicht durch technische Störungen
- Verfügbarkeit
	- Daten müssen abrufbar sein, wenn der Benutzer es will
	
## Anonymisierung
- Daten werden so verändert, dass die Zuordnung auf eine Person nicht (oder nur mit unzumutbarem Aufwand) möglich ist
## Datenschutzfreundliche Software
- Quelloffene (Open Source) Software sind oft (nicht immer) eher datenschutzfreundlich
## Teststoff
- Netzwerksicherheit 19-23
- Unterschied Backup/Sicherung
- Backup-Strategie - Generationenprinzip
- Speichermedien (siehe Präsentation)
	- Kapazitäten
- 3-2-1 Backup Strategie Regel
- Vorteile/Nachteile Cloud Backup
- Was ist eine Hybrid Cloud
