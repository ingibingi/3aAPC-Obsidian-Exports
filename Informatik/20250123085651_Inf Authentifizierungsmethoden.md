---
aliases: 
cssclasses: 
tags:
  - 3aAPC
  - ToDo/Submit
  - ToDo/Finish
date: 2025-01-23
deadline: 
hideFromQuery: false
link: 
info:
---

# Authentifizierungsmethoden
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: ITLxx/Informatik
- Datum: 2025-01-23

---
## Fido2
- FIDO... Fast IDentity Online
- Alternative zu Passwort
- Authentifizierung mit Hardware-Sicherheits-Key (Dongle)
- Basiert auf
	- Webauthn
	- CTAP
- Hebelt weitere Gefahren (großteils) aus
	- Replay-Attacks
	- Phishing
- Generelle Funktionsweise
	- Kommunikation mittels Private/Public Key-Verschlüsselung
	- Verschlüsselung erfolgt mittels Sicherheits-Key
	- Client 
		- sendet Anfrage
			- mit Private Key verschlüsselt
		- Beweis Client ist Client
	- Server
		- entschlüsselt Anfrage
			- mit Public Key
		- erstellt Aufgabe
			- Simple Operation, die jeder Computer lösen kann
		- verschlüsselt Aufgabe
				- mit Public Key[^1]
		- sendet Aufgabe an Client
	- Client  
		- entschlüsselt Aufgabe
		- löst Aufgabe
		- verschlüsselt Lösung
			- mit Private Key
		- sendet Lösung an Server
	- Server
		- entschlüsselt Lösung
		- überprüft Lösung
		- 

![FIDO Promises a Life Without Passwords - YouTube](https://www.youtube.com/watch?v=lRFeuSH9t44)
### Passkey
- Benutzerfreundliche Erweiterung von Passkey
	- damit einhergehend ein geringer Verlust an Sicherheit
- Authentikator über Software-Lösungen (z. B. über Smartphone)
- Von Apple/Google/Microsoft beworben
	- u. A. aus wirtschaftlichen Gründen

[^1]: Sowohl Private Key, als auch Public Key können jeweils verschlüsseln und entschlüsseln. Aber NUR der jeweils Andere Key kann die Verschlüsselung des Einen lösen. 
