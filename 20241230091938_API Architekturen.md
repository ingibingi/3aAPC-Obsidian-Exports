---
aliases: 
cssclasses: 
tags: 
date: 2024-12-30
deadline: 
hideFromQuery: false
info: 
link:
---
[Top 6 Most Popular API Architecture Styles](https://www.youtube.com/watch?v=4vLxWqE94l4)

> [!Def] API
> API... Application Programming Interface

# Beliebte Architekturen
## SOAP
- (ehemals) Simple Object Access Protocol
- W3C empfehlung
- OSI Level 4 (Transport) & Level 7 (Anwendung)
- XML-Basierend
- angeblich
	- verbos und komplex...
	- gut für sicherheitskritische Anwendungen
	- overkill für simple anwendungen
## RESTful
[RESTful APIs in 100 Seconds](https://www.youtube.com/watch?v=-MTSQjw5DrM)
"Representational State Transfer"
- Internet-"Backbone"
- Baut auf [HTTP-Methoden](20241223221351_HTTP.md#CRUD-Methoden) auf
- Einfach zu implementieren
- Für Arbeiten mit Echtzeitdaten ungeeignet
- Statless
	- Status wird nicht auf Server gespeichert
	- Jede Anfrage hat eigenen Token
	- 
## GraphQL
- Query Language
	- nur benötigte Daten werden übertragen
- flexibel und effizient
- steile Lernkurve
- von Facebook
## gRPC
- google Remote Procedure Call
- modern, performant
- verwendet standardmäßig Protocol Buffers
- beliebt für 
	- microservice-anwendungen
	- interservice kommunikation (z. B. bei Microsoft)
## WebSocket
- Low latency
- Für Echtzeitdaten
- oft overkill
- Aufrecht gehaltene, bidirektionale Verbindung zwischen Server u. Client
- 
## WebHook
- Event-gesteuert
- Asynchrone Kommunikation