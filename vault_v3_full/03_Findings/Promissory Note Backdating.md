---
tags: [finding]
status: documented
confidence: high
estimated_impact: "$858K note"
direction: apollo-inflated
---

# Promissory Note Backdating

## Summary
An $858K promissory note attributed to Apollo was proven backdated by **174 days** via batch timestamp analysis. The note's purported execution date does not match the system timestamp of when the entry was actually created.

## Evidence Chain

### The Proof
- **Purported date:** The date shown on the promissory note document
- **Batch timestamp:** The system records when the entry was actually created in the accounting system
- **Delta:** 174 days — the note was entered into the system nearly 6 months after its supposed execution date

### Why This Matters
A backdated promissory note of this size creates a retroactive liability on Apollo's books. It makes it appear Apollo owed this money for longer than it actually did, potentially justifying cash transfers from Apollo to ATI that would otherwise be unexplained.

## Directional Analysis
Creates liability on Apollo's books → justifies cash extraction from Apollo → consistent with the overall pattern.

## Counterarguments
- **"Administrative delay in recording"** — A 174-day delay in recording an $858K note is not a clerical oversight. Notes of this magnitude are recorded promptly.
- **"The note was genuinely executed on the earlier date but not entered until later"** — Possible but raises the question: why? And the batch-print pattern of all 12 monthly statements suggests systematic retrospective record creation, not isolated delay.

## Connected
- [[Rosanna Karim]] — Primary system user
- [[James Luhr Jr]] — Signatory
- [[GL Audit Trail Anomalies]]
