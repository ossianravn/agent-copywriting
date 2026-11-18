---
max_turns: 25
timeout_seconds: 900
allowed_tools: [Read, Glob, Grep, Skill, Agent]
---

Vi bygger en app til håndværkere, hvor de uploader billeder af færdigt arbejde til en sag. Jeg mangler tekster til tre steder:

1. Fejlen, når et billede er for stort. Grænsen er 15 MB.
2. Den tomme tilstand på siden "Billeder" på en sag, før der er uploadet noget.
3. Bekræftelsesdialogen, når man sletter en sag. Sagens billeder og noter slettes også, og det kan ikke fortrydes.

Vi siger "du" til brugeren. Knappen til upload hedder allerede "Tilføj billeder".
