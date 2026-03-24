---
type: finding
status: documented
confidence: high
tags: [finding, high]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[Intercompany Transfer Tracker]]"
  - "[[GL Audit Trail Anomalies]]"
evidence-refs:
  - "[[Apollo QuickBooks LOGS 2022-2026]]"
  - "[[Apollo 2023 to dec 2024 General Ledger]]"
dollar-amount: 858000
estimated_impact: "$858K note"
direction: apollo-inflated
---

# Promissory Note Backdating

## Summary
An $858K promissory note ([[Apollo QuickBooks LOGS 2022-2026|QB Logs — batch timestamp analysis]]) attributed to Apollo was proven backdated by **174 days** via batch timestamp analysis. The note's purported execution date does not match the system timestamp of when the entry was actually created.

## Evidence Chain

### The Proof
- **Purported date:** The date shown on the promissory note document
- **Batch timestamp:** The system records when the entry was actually created in the accounting system
- **Delta:** 174 days — confirmed via [[DOC-QB-LOGS-2022-2026]] batch timestamp vs transaction date — the note was entered into the system nearly 6 months after its supposed execution date

### Why This Matters
A backdated promissory note of this size creates a retroactive liability on Apollo's books. It makes it appear Apollo owed this money for longer than it actually did, potentially justifying cash transfers from Apollo to ATI that would otherwise be unexplained.

## Directional Analysis
Creates liability on Apollo's books → justifies cash extraction from Apollo → consistent with the overall pattern.

## Counterarguments
- **"Administrative delay in recording"** — A 174-day delay in recording an $858K note is not a clerical oversight. Notes of this magnitude are recorded promptly.
- **"The note was genuinely executed on the earlier date but not entered until later"** — Possible but raises the question: why? And the batch-print pattern of all 12 monthly statements suggests systematic retrospective record creation, not isolated delay.

## Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — Entry creating promissory note (SHA: `d918f3c9...ef9a0a82`)
- [[Apollo 2023 to dec 2024 General Ledger]] — GL record
- [[Source Registry]] | [[Data Lineage]]

## Connected
- [[Rosanna Karim]] — Primary system user
- [[James Luhr Jr]] — Signatory
- [[GL Audit Trail Anomalies]]
- [[Master Timeline]]
