---
type: permanent
tags: [rag, failure-modes]
---

# RAG failures often look like confident nonsense

When retrieval fails or returns irrelevant chunks, models tend to:
- answer anyway
- blend memories and guesses
- sound persuasive while being wrong

Mitigation:
- require “insufficient data” fallback
- force tool/retrieval before answering certain questions
- add tests for missing/contradictory data
