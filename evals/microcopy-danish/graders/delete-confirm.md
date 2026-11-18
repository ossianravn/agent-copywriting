---
type: llm
---

Judge only the interface strings, not any note the assistant wrote around them.

PASS if the confirmation for deleting a case states that the case's images and notes are deleted too and that this cannot be undone, and if the confirming button names the action with its verb (for example "Slet sag").

FAIL if a consequence is missing, or if the confirming button is a bare "OK", "Ja" or "Bekræft".
