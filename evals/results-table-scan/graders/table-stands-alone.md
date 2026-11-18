---
type: llm
---

Judge only the "Results" section the assistant wrote, not any note around it. Look at each table by itself and ignore every sentence outside it. If the section has no table, look at its lists of figures in the same way.

PASS if a colleague who reads nothing but the table can tell what every number in it counts. The column headers, row labels or cells name the thing counted or the unit (for example "Visitors who bought", "Share of visitors who bought", "Support tickets about payment"), and it is clear which numbers belong to the old checkout and which to the new one.

FAIL if any column or cell shows a bare number, fraction or percentage whose meaning is given only in the text outside the table, for example a column headed "Old" holding "412 of 9,800" or "4.2 %" with nothing in the table saying what that measures.
