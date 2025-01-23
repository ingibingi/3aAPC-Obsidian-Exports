---
aliases:
  - Datenstuktur
cssclasses:
  - pageBreak
tags:
  - 3aAPC/Inf
date: 2024-11-14
deadline: 2024-11-14
hideFromQuery: false
link:
  - https://www.eduvidual.at/mod/assign/view.php?id=6816852
info: Java Framework & Hashtables noch nicht verstanden -> besser ausarbeiten
---
# Datenstrukturen 
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: Informatik
- Datum: 2024-11-14
---
Inhaltsverzeichnis

1. [Angabe](#angabespan-classpagenumberspan)
	1. [ToDo](#todo)
2. [Was ist eine Datenstruktur?](#was-ist-eine-datenstrukturspan-classpagenumberspan)
3. [Daten-Typen](#daten-typenspan-classpagenumberspan)
4. [Gängige Struktur-Typen](#g%C3%A4ngige-struktur-typenspan-classpagenumberspan)
	1. [Datensatz (Tupel/Record)](#Datensatz%20(Tupel/Record))
	2. [Array](#Array)
	3. [Linked List](#Linked%20List)
	4. [Queue](#Queue)
	5. [Stack](#Stack)
	6. [Heap](#Heap)
	7. [Graph](#Graph)
	8. [Baum](#Baum)
	9. [Hashtable](#Hashtable)
5. [Java Collections Framework](#java-collections-frameworkspan-classpagenumberspan)
	1. [Datentypen](#datentypen)
6. [Notizen aus dem Unterricht(#notizen-aus-dem-unterrichtspan-classpagenumberspan)
7. [Fazit](#fazitspan-classpagenumberspan)
1. [Quellen](#quellenspan-classpagenumberspan)
---
## Angabe

> [!NOTE]
> Erstellen Sie eine [Übersicht](https://www.eduvidual.at/mod/page/view.php?id=6816898 "Übersicht") über Grundlegende [Datenstrukturen](https://www.eduvidual.at/mod/page/view.php?id=4528025 "Datenstrukturen"). 
> 
> - Was versteht man unter Datenstruktur?
> - Welche Grunddatentypen gibt es? (mit Speicherbedarf)  
>     
> - Wer übernimmt die Verwaltung der Daten im Speicher/auf der Festplatte?  
>     
> - Erstellen Sie eine [Übersicht](https://www.eduvidual.at/mod/page/view.php?id=6816898 "Übersicht") gängiger Datenstrukturen inkl. kurzer Beschreibung derer Eigenschaften (Array, Queue, Stack, Heap, Graph, Baum, Hashtable)
> - Geben Sie die jeweiligen Java Klassen aus dem **Java Collections [Framework](https://www.eduvidual.at/mod/resource/view.php?id=6816895 "Framework")** an. Die wichtigsten Methoden inkl. kurzer Beschreibung sollten auch nicht fehlen.
> 
> Quelle:   [https://de.wikipedia.org/wiki/Datenstruktur](https://de.wikipedia.org/wiki/Datenstruktur)

### ToDo
- [x] Erklärung Datenstruktur
- [x] Übersicht Grunddatentypen (mit Speicherbedarf)
- [x] Verwaltung der Daten im Speicher/auf Festplatte
- [ ] Übersicht Datenstrukturen (Java Collections Framework)
	- [ ] Beschreibung d. Eigenschaften
	- [ ] wichtigste Methoden
---
<span class="pageBreak"></span>
## Was ist eine Datenstruktur?
> [!NOTE] Def.: Datenstruktur
> - Die Struktur, mit der Daten angeordnet und verknüpft werden.
> - Unterschiedliche Datenstrukturen
> 	- haben Einfluss auf die Effizienz mit der die Daten gefunden, gelesen, geschrieben werden können
> 	- unterscheiden sich in den möglichen Operatoren für die einzelnen Datensätze
> 	- haben unterschiedlichen Speicherbedarf
- [Grafik Pyramide Datenstruktur](https://www.eduvidual.at/pluginfile.php/7765572/course/section/3377753/1532026350.png)
	![](attachment/a02b0419efd9cd10602c3580835a3d67.png)
	
---
<span class="pageBreak"></span>
## Daten-Typen
nicht verwechseln mit Daten-Strukturen
Details sind abhängig von Umgebung
- True/False
	- Boolean
- Speicheradresse
	- Pointer
- Ganzzahlen
	- Integer 
- Gleitkommazahlen
	- Float
- Symbol
	- Char
- Text
	- String
## Gängige Struktur-Typen
### Datensatz (Tupel/Record)
- Einfachste Datenstrukturen
- Folge von Werten
- z. B. Zeile einer Tabelle
### Array
- Menge von Werten
	- alle haben den selben Datentypen
- Kann Gut:
	- auf Elemente Zugreifen
- Kann NICHT Gut:
	- Elemente Hinzufügen
	- Elemente Entfernen
- Anzahl der Werte oft NICHT änderbar
	- Der Wert selbst ist schon veränderbar
- Alle Daten des Datensatzes in einem Block
- Lineare Datenstruktur
### Linked List
- Menge von Werten
	- können unterschiedliche Datentypen besitzen
- Kann Gut:
	- Element hinzufügen
	- Element löschen
- Kann NICHT Gut:
	- auf Elemente zugreifen
- Singly Linked List
	- An Ende von Datensatz ist der Link (pointer) zu nächstem Datensatz hinterlegt
		- Quasi eine Schlange A->B->C->D->...
- Doubly Linked List
	- Element hat zusätzlich auch link zu vorherigem Element
		- Mehr Speicherbedarf
		- Rückwärtige Suche möglich
- Lineare Datenstruktur

### Queue
![](attachment/e4641012d808638f370869add6beb8ce.png)
- Sonderform der Liste
	- Kann als Array oder Linked List umgesetzt werden
- "Elemente stellen sich in einer Reihe (Queue) an"
- FIFO
	- First In
	- First Out
	- der älteste Datensatz wird zuerst abgegriffen
- Befehle
	- Enqueue
		- Neues Element an Ende hinzufügen
	- Dequeque
		- Ältestes Element von Anfang entfernen
		- evtl. auch ausgeben
	- Peek
		- Ältestes Element von Anfang ausgeben
### Stack
- Sonderform der Liste
	- Kann als Array oder Linked List umgesetzt werden
- "Elemente werden aufeinander gestapelt (stacked)"
- LIFO
	- Last In
	- First Out
	- immer das neueste Element ausgeben
- Befehle
	- Push
		- Neues Element auf Stack oben ==drauflegen==
	- Pop
		- Neuestes (==oberstes==) Element von Stack ==entfernen==
		- evtl. auch ausgeben
	- Top
		- Neuestes (==oberstes==) Element von Stack ==ausgeben==
	- IsFull
		- returns true if full
	- IsEmpty
		- returns true if empty
- Vorteile
	- Oben gelistete Befehle haben O(1)
	- Gut geeignet für Rekursive Funktionen
	- Offer
		- Neues Element am Ende vom Stack hinzufügen
		- Unten Reinlegen
	- Poll
		- Letztes Element 
	![](attachment/bbdd86afe2f10d49bebd16bd3ca6759b.png)

### Heap
![](attachment/062cb520f70f60f4cc52bb0f6b15a21d.png)
- Baum-Struktur mit Priorisierung 
	- Höherer Index -> Höhere Priorität
- Knotenpunkte stehen in Parent/Child Beziehung zueinander
	- 1 Parent (P) hat 
	- 0-n Children (C)
- Verhältnis der Indexwerte zw. Parent und Child
	- Index(P) > Index(C)
- MaxHeap / MinHeap
	- Beschreibungen gelten für MaxHeap
	- MinHeap: 
		- Pirorisierung von kleinerem Index
		- Index(P) < Index(C)
- Kann Suche Beschleunigen
### Graph
![](attachment/f1503ea4e7b9332d60f72a509ac34b61.png)
- Die Verbindung selbst ist (teil) der Information
- Knotenpunkte können Verbindungen zu mehreren anderen Knotenpunkten haben
### Baum
![](attachment/83d0f027f7f2e62a379c5b530f9c59a1.png)
- Knotenpunkte stehen in Parent/Child Beziehung zueinander
	- 1 Parent (P) hat 
	- 0-n Children (C)
### Hashtable
- ein "Dictionary"-Array wird erstellt
- dieses wird als "Index" verwendet
- Damit lassen sich Inhalte schneller suchen
- Wird für große Datenmengen verwendet
- Die Adresse des Objekts wird über den Such-Key generiert
- Probleme durch Überlappungen/Kollisionen werden mit open/closed adressing-Methoden minimiert
	- open adressing
		- linear probing... der nächste Freie Platz wird genommen
	- closed adressing
		- Bei berechneter adresse wird eine linked list erstellt. das 1. Element wird der head, jedes weitere wird angehängt
- Load Factor
	- Ist die Größe des Arrays größer als die Anzahl der Elemente, so kommt es weniger oft zu kollisionen
	- $\text{Load Factor}=\frac{\text{Besetzte Elemente}}{\text{Verfügbare Elemente}}$
- Typische Umsetzung
	- Daten: Linked Liste mit den eigentlichen Elementen
	- Hashtable: Array mit Such-Keyword und Pointer zu Element in Linked Liste
- ![Hash Tables and Hash Functions - YouTube](https://www.youtube.com/watch?v=KyUTuwz_b7Q)
## Java Collections Framework


- ![](attachment/e1dcf968d167db2d9cc1b29f11ce586a.png)
### java.uitl.Collections
- [java.util.Set](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html)
	- Menge
		- jeweiliges Element kommt max 1x vor
- [java.util.SortedSet](https://docs.oracle.com/javase/8/docs/api/java/util/SortedSet.html
	- Extends Set
	- Elemente sind geordnet
- [java.util.NavigableSet](https://docs.oracle.com/javase/8/docs/api/java/util/NavigableSet.html)
	- Extends SortedSet
	- Elemente sind vergleichbar
	- Methoden:  floor, ceiling, lower, higher
- [java.util.Queue](https://docs.oracle.com/javase/8/docs/api/java/util/Queue.html)
	- Extends Collection
	- Sammlung von Elementen
	- Selbes Element kann mehrfach vorkommen
	- Elemente sind geordnet
	- Methoden:	
		- offer(e)
			- Element e hinzufügen
		- poll()
			- Element entfernen
		- peek()
			- Element lesen
- [java.util.concurrent.BlockingQueue](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/BlockingQueue.html)
	- Extends Queue
- [java.util.concurrent.TransferQueue](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/TransferQueue.html)
	- Extends BlockingQueue
- [java.util.Deque](https://docs.oracle.com/javase/8/docs/api/java/util/Deque.html)
	- Extends Queue
- [java.util.concurrent.BlockingDeque](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/BlockingDeque.html)
	- Extends Dequeue
### java.util.Map
- [java.util.SortedMap](https://docs.oracle.com/javase/8/docs/api/java/util/SortedMap.html) 
	- Extends Map
		- Map: Dictionary (aber als Interface)
	- Elemente sind geordnet
- [java.util.NavigableMap](https://docs.oracle.com/javase/8/docs/api/java/util/NavigableMap.html)
	- Extdends SortedMap
	- Methoden
		- lowerEntry, floorEntry, ceilingEntry, higherEntry
- [java.util.concurrent.ConcurrentMap](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/ConcurrentMap.html)
	- Extends Map
- [java.util.concurrent.ConcurrentNavigableMap](https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/ConcurrentNavigableMap.html)
	- Extends ConcurrentMap
## Notizen aus dem Unterricht
- Wer übernimmt die Speicherung der Datenstruktur auf der Festplatte/im Arbeitsspeicher
	- Für die Festplatte: Das Dateisystem (FAT32, ext3, ext4, Btrfs, NTFS, etc.)
	- Für den Arbeitsspeicher: Das Betriebssystem
## Fazit
- Listen ist der Überbegriff für
	- Arrays
	- Linked Lists
- Spezielle Listen sind
	- Stacks (LIFO)
	- Queues (FIFO)

## Quellen
- [Datenstruktur – Wikipedia](https://de.wikipedia.org/wiki/Datenstruktur)
- [Arrays vs Linked Lists - Computerphile](https://www.youtube.com/watch?v=DyG9S9nAlUM)
- [Collection Framework](https://www.javatpoint.com/collections-in-java)