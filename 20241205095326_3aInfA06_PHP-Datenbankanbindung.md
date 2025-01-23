---
aliases: 
cssclasses: 
tags:
  - 3aAPC
date: 2024-12-05
deadline: 
hideFromQuery: false
link: 
info:
---

# PHP-Datenbankanbindung

---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: ITLxx/Informatik
- Datum: 2024-12-05

---
`ToDo: Create Table of Content && Remove this comment`

---
## Angabe
1. Analyse der aktuellen DB Verbindung mittels DatabaseFactory im Huge [Framework](https://www.eduvidual.at/mod/resource/view.php?id=6816895 "Framework").
2. Baue eine Funktion zB: `NoteModel::getNote()` auf mySqli um.

- Erkläre bei beiden den Ablauf und beschreibe welche Möglichkeit du bevorzugst. Begründe deine Entscheidung!
- Wie werden "prepared Statements" in den beiden Erweiterungen integriert?
- Erkläre den Unterschied zwischen "Parameter Binding" und "Prepare Statements".
- Wie werden "stored procedures" integriert?
- Wie werden die Daten einer Abfrage bei den beiden Erweiterungen abgerufen und ausgegeben?
- Wie werden die Verbindungen jeweils geschlossen?

---



|                               | PDO                  | MySQLi            |
| ----------------------------- | -------------------- | ----------------- |
| **Database support**          | 12 different drivers | MySQL only        |
| **API**                       | OOP                  | OOP + procedural  |
| **Connection**                | Easy                 | Easy              |
| **Named parameters**          | Yes                  | No                |
| **Prepared statements  <br>** | Yes                  | Yes               |
| **Performance**               | Fast                 | Fast              |
| **Stored procedures**         | Yes                  | Yes               |
| **Asynchrone Abfragen**       | No                   | Yes (only SELECT) |
