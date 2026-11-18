---
type: llm
---

Judge only the interface strings, not any note the assistant wrote around them.

PASS if the error text for an oversized image says that the image is larger than 15 MB (or that the limit is 15 MB) and tells the user what to do next, such as choosing a smaller image.

FAIL if the limit or the next step is missing, or if the text only says that something went wrong.
