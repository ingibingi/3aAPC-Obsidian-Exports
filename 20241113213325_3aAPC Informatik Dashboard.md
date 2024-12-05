---
aliases:
  - 3aAPC Informatik Dashboard
cssclasses:
  - \
tags:
  - 3aAPC/Inf
  - Dashboard
  - ToDo/Finish
  - ToDo/Submit
  - ToDo/Ask
date: 2024-11-13
hideFromQuery: true
---
---
```dataview
TABLE 
	contains(tag,ToDo) AS "To-Do",
	date, 
	deadline, 
	link
FROM 
	#3aAPC/Inf 
WHERE !hideFromQuery
SORT deadline ASC
```
---
# A1 Algorithmen
![](attachment/2b1ae8c840c0373ab1e59f3498a84206.md) 