---
aliases: 
cssclasses: 
tags:
  - 3aAPC
  - ToDo/Submit
  - ToDo/Finish
date: 2024-12-17
deadline: 
hideFromQuery: false
link: 
info:
---

# Netzwerksicherheit & Neztzwerktechnik
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: DTSM
- Datum: 2024-12-17

---
## Angabe

1. Grundlagen Netzwerktechnik
	- Übersicht zu Grundfunktionen einer Firewall erstellen
	- 3 Schutzmechanismen für Netzwerke aufzählen
	- Hacking: Mögliche Angriffspunkte nennen und beschreiben
	- Datenabflusspunkte im Kontext Internetnutzung wiedergeben können
	- Protokoll zur Synchronisierung nennen  
	- Zeitsynchronisierung in Serversystemen beschreiben und begründen
2. Fragen Netzwerksicherheit
	- Welche prinzipielle Aufgabe hat eine Firewall?
	- Welche 2 prinzipiellen Funktionsweisen einer Firewall kennen Sie? – kurze Erklärung!
	- Was ist und welche Aufgabe hat eine „DMZ“ im Kontext Netzwerksicherheit?
	- Was versteht man unter einem „IDS“ im Kontext Netzwerksicherheit?
	- Was versteht man unter einem „IPS“ im Kontext Netzwerksicherheit?
	- Was sind die aktuell 3 häufigsten Bedrohungen der Netzwerksicherheit?
	- Was versteht man unter Malware?
	- Was versteht man unter „ Advanced Persistent Threats (APT)”?
	- Was versteht man unter “DDoS-Angriffe (Distributed Denial of Service)“?
	- Was versteht man unter einem „Angriffsvektor“ im Kontext Netzwerksicherheit?
	- Was versteht man unter „Ransomware“ – im Kontext Malware -  Erklärung anhand Beispiel?!
	- Was versteht man unter „Phishing“ – im Kontext Malware -  Erklärung anhand Beispiel?!
	- Was versteht man unter der „Zero-Day-Lücke“? – mit welchen Fristen wird in diesem Zusammenhang üblicherweise gerechnet?
	- Zu welchem Zeitpunkt spricht man von einer „N-Day-Schwachstelle“ im Kontext Zero-Day-Lücke?
	- Welche Maßnahmen können ergriffen werden um „Zero-Day-Exploits“ zu verhindern?
	- Was versteht man unter einem „White-, Grey-, Black-Hat“ – Hacker?
	- Nennen Sie 5 Methoden von Hackern und erklären Sie diese kurz!
	- Wie können Angriffe seitens IDS/IPS erkannt werden?
	- Was ist die Grundlage einer Authentifizierung?
	- Was versteht man unter einer Zweifaktor-Authentifizierung (2FA)?
	- Was versteht man unter einer Multifaktor-Authentifizierung (MFA)?
	- Welche Aufgabe hat Kerberos bzw. welches Ziel wurde bei der Entwicklung von Kerberos verfolgt?
	- Welche Eigenschaften weist Kerberos auf – kurze Erklärung?!
	- Wie läuft die Kerberos-Authentifizierung prinzipiell ab?
	- Welche 2 Vorteile werden durch Kerberos erreicht?
	- Wie werden Replay-Angriffe verhindert?
	- Warum ist es wichtig das in einem Netzwerk alle Systeme die gleiche Uhrzeit haben?
	- Was versteht man unter einem Token bzw. Token-Karten im Kontext Authentifizierung?
	- Welchen Vorteil bieten Tokensysteme gegenüber einer Smart-Card-Lösung?
	- Welchen Vorteil bietet ein Hardware-Token?
---
## Lösung
### Netzwerktechnik allgemein
#### Übersicht zu Grundfunktionen einer Firewall erstellen
#### 3 Schutzmechanismen für Netzwerke aufzählen
#### Hacking: Mögliche Angriffspunkte nennen und beschreiben
#### Datenabflusspunkte im Kontext Internetnutzung wiedergeben können
#### Protokoll zur Synchronisierung nennen  
#### Zeitsynchronisierung in Serversystemen beschreiben und begründen
### Netzwerksicherheit Fragen
#### Welche prinzipielle Aufgabe hat eine Firewall?
- Ein Netzwerk vor ungewünschtem Traffic schützen
- Sprich: schützt vor ungewünschten Zugriff
#### Welche 2 prinzipiellen Funktionsweisen einer Firewall kennen Sie? – kurze Erklärung!
- External Firewall
	- Grenzt das eigene (sichere) Netz von außen (unsicher) ab.
	- Lässt nur "sicheren" Traffic durch
	- Netzwerke lassen sich in unterschiedlich "sichere" Bereiche abgrenzen
- Personal Firewall
	- überprüft den Traffic an einem Endgerät
- Generell
	- Firewall beobachtet 
		- Header (IP-Adresse)
		- Inhalt (Packet)
#### Was ist und welche Aufgabe hat eine „DMZ“ im Kontext Netzwerksicherheit?
- DMZ... DeMilitarised Zone
- "Sicherer" Bereich eines Netzwerks
- Kommunikation nach Außen ist eingeschränkt
	- z. B. durch Firewall
- DMZ beinhaltet oft Inhalte, die öffentlich zugänglich gemacht werden müssen
- Empfehlung Abschottung sowohl nach Innen und nach außen
  ![](../../Other%20Files/Images/Pasted%20image%2020241218152039.png)
#### Was versteht man unter einem „IDS“ im Kontext Netzwerksicherheit?
- IDS...Instrusion Detection System
- Wichtiges Element für eine DMZ
- Erkennt falls diese kompromittiert wurde
- Wie gut ist die Erkennung?
	- False Positive
	- False Negative
#### Was versteht man unter einem „IPS“ im Kontext Netzwerksicherheit?
- IPS... Instrusion Prevention System
- Reagiert bei komprommitierung der DMZ
	- z. B. Sperrt den Traffic zu/von einer "verdächtigen" IP-Adresse
#### Was sind die aktuell 3 häufigsten Bedrohungen der Netzwerksicherheit?
>lt. https://www.computerweekly.com/de/tipp/Netzwerksicherheit-Die-3-groessten-Gefahren-und-ihre-Abwehr
- Malware
- Advanced Persistent Threats (APT)
- Distributed Denial of Services (DDoS)
#### Was versteht man unter Malware?
- Unerwünschte Software die gewöhnlicherweise Schaden verursacht
	- Viren
		- Programmcode
		- infiziert andere Dateien
		- vervielfältigt sich selbständig
	- Würmer
		- Programm
		- vervielfältigt sich selbständig
	- Trojanische Pferde
		- Programm
		- KEINE selbständige Vervielfältigung
#### Was versteht man unter „ Advanced Persistent Threats (APT)”?
- Koordinierte Angriffe auf ein Ziel
#### Was versteht man unter “DDoS-Angriffe (Distributed Denial of Service)“?
- DoS-Angriffe, die koordiniert von mehreren Positionen ausgeführt werden.
#### Was versteht man unter einem „Angriffsvektor“ im Kontext Netzwerksicherheit?
- Methode um eine Sicherheitslücke auszunutzen
#### Was versteht man unter „Ransomware“ – im Kontext Malware -  Erklärung anhand Beispiel?!
- Angreifer erhält Zugriff auf wichtige Daten
- Angreifer verschlüsselt die Daten
- Angreifer fordert Lösegeld für den Zugriff auf die eigenen Daten
#### Was versteht man unter „Phishing“ – im Kontext Malware -  Erklärung anhand Beispiel?!
- "Enkeltrick"
- Website, E-Mail, Werbebanner, Anruf etc.
- Ausgabe als das Original, um z. B. Passwörter zu erschleichen
#### Was versteht man unter der „Zero-Day-Lücke“? – mit welchen Fristen wird in diesem Zusammenhang üblicherweise gerechnet?
- Neue (bisher unbekannte) Lücke
- Lücke noch nicht länger als 24h bekannt
- Noch kaum Gelegenheit sich gegen Angriffe zu verteidigen
#### Zu welchem Zeitpunkt spricht man von einer „N-Day-Schwachstelle“ im Kontext Zero-Day-Lücke?
- Bereits länger bekannte Lücke
#### Welche Maßnahmen können ergriffen werden um „Zero-Day-Exploits“ zu verhindern?
- Sicherheitsstandards einhalten
- Pen-Tester engagieren
- schnell patchen

---
- Was versteht man unter einem „White-, Grey-, Black-Hat“ – Hacker?
- Nennen Sie 5 Methoden von Hackern und erklären Sie diese kurz!
- Wie können Angriffe seitens IDS/IPS erkannt werden?
- Was ist die Grundlage einer Authentifizierung?
- Was versteht man unter einer Zweifaktor-Authentifizierung (2FA)?
- Was versteht man unter einer Multifaktor-Authentifizierung (MFA)?
- Welche Aufgabe hat Kerberos bzw. welches Ziel wurde bei der Entwicklung von Kerberos verfolgt?
- Welche Eigenschaften weist Kerberos auf – kurze Erklärung?!
- Wie läuft die Kerberos-Authentifizierung prinzipiell ab?
- Welche 2 Vorteile werden durch Kerberos erreicht?
- Wie werden Replay-Angriffe verhindert?
- Warum ist es wichtig das in einem Netzwerk alle Systeme die gleiche Uhrzeit haben?
- Was versteht man unter einem Token bzw. Token-Karten im Kontext Authentifizierung?
- Welchen Vorteil bieten Tokensysteme gegenüber einer Smart-Card-Lösung?
- Welchen Vorteil bietet ein Hardware-Token?

## Notizen aus dem Unterricht

## Quellen
- 
