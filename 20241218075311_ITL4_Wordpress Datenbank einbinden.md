---
aliases: 
cssclasses: 
tags:
  - ToDo/Submit
  - ToDo/Finish
  - 3aAPC/ITL4
date: 2024-12-18
deadline: 
hideFromQuery: false
link: 
info:
---

# NameDesThemas
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: ITL4
- Datum: 2024-12-18

---
## Angabe
- Beschäftigen Sie sich mit Content Management System WordPress.
- Erstellen ein einfaches Kontaktformular mittels PlugIn (zum Vergleich)
- Erstellen Sie ein einfaches Formular, welches die Daten in eine zuvor erstellte SQL-Datenbank einfügt.
- Das Ziel ist es zuerst ein HTML Formular mittels normalem Editor (als HTML bearbeiten) eingefügt werden

![](attachment/567dd49ed1a5be25416b126531043edd.png)
- Der Submit ist in einer PHP Datei (des Themes) zu erkennen und danach der INSERT in die eigene Datenbank durchzuführen
![](attachment/bbfc40a6f881903391a608a6a438827a.png)
- Die Übung sollte aufbauend auf die Laborübung SQL-Ausgabe in Wordpress sein – verwenden Sie die gleiche Datenbank.
- Verwenden Sie die „mysqli“ oder „PDO“ Klasse, um eine Verbindung zur Datenbank herzustellen.
- Tipp: Versuchen Sie zuerst eine DB-Eingabe über eine einfache Internet-Seite, zB: „index.php“, herzustellen.
---

### ToDo
- [ ] ...
- [ ] Abgeben
## Lösung
### Kontaktformular erstellen
#### Plugin installieren
WPForms-Plugin installieren
![](attachment/f6eecf74f3f3070160163cc115d35b18.png)
#### Kontaktformular erstellen
![](attachment/0660972e5596a35fbb5a82368c32be13.png)
- Template Auswählen
Schritt für Schritt-Anleitung folgen
##### Versuch SMTP einzurichten für Bestätigungs-Mail

![](attachment/de298bdab3868b782c08907b0c319d3c.png)
- benötigt Google-Cloud, vorerst zu umständlich
	- Grundeinstellungen beibehalten
### Datenbank erstellen
- mittels phpmyadmin
```mysql
CREATE TABLE `kontaktformular`.`kontakte` (`ID` INT NOT NULL AUTO_INCREMENT , `Vorname` VARCHAR(50) NOT NULL , `Nachname` VARCHAR(50) NOT NULL , `email` VARCHAR(255) NOT NULL , `text` TEXT NOT NULL , `refnr` INT NOT NULL , PRIMARY KEY (`ID`), UNIQUE (`ID`)) ENGINE = InnoDB;
```
### Datenbank einbinden
>Ausgabe der Datenbank auf einer seite

#### Plugin installieren

php code schreiben
AnleitungQuelle: [PHP MySQL Select Data](https://www.w3schools.com/php/php_mysql_select.asp)



## Notizen aus dem Unterricht

## Quellen
- 
