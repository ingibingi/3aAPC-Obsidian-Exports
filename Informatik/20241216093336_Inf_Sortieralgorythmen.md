---
aliases: 
cssclasses: 
tags:
  - 3aAPC
date: 2024-12-16
deadline: 
hideFromQuery: false
link: 
info:
---

# Sortieralgorithmen
---
- Autor: Ingo Schlapschy
- Schuljahr: 2024/25
- Lehrgang: 2
- Klasse: 3aAPC
- Gruppe: C
- Fach: ITLxx/Informatik
- Datum: 2024-12-16

---
`ToDo: Create Table of Content && Remove this comment`

---
## Bubble Sort
- Liste Durchgehen
	- Vergleich Von Element mit Nächstem Element
		- Wenn unsortiert -> vertauschen
		- weiter zu nächstem Element
## Insertion Sort
- Liste Durchgehen
	- Kleinstes Element merken
- Kleinestes Element an 1. Stelle
- Bei 2. Stelle wiederholen
## Selection Sort
- Aufteilen in 2 Teile
	- Unsortierter Part
	- Sortierter Part
- Nächstes Element 
## Merge Sort
- Element 1 und 2 Vergleichen
	- Sortiert als Array "A" hinterlegen
- Element 3 und 4 vergleichen
	- Sortiert Als Array "B" hinterlegen
- ...restliche Liste derart durchgehen
- Element 1 aus "A" mit Element 3 aus "B" vergleichen
	- kleinstes Element in Array A_2 hinterlegen
	- nächstgrößeres Element mit vormals größerem Element vergleichen
	- kleinstes Element in Array A_2 hinterlegen

# Vergleich

| Sortierverfahren | Big O(n)  | ist stabil | ist in Place |
| ---------------- | --------- | ---------- | ------------ |
| Bubble           | n^2       | möglich    | ja           |
| Insertion        | n^2       | möglich    | ja           |
| Selection        | n^2       | möglich    | ja           |
| Merge            | n\*log(n) | möglich    | nein         |
| Quicksort        | n\*log(n) | nein       | ja           |
