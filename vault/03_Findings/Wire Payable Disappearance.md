---
type: finding
status: needs-investigation
confidence: medium
tags: [finding, medium]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Forensic Cross-Reference Report]]"
  - "[[Promissory Note Backdating]]"
  - "[[Intercompany Transfer Tracker]]"
evidence-refs:
  - "[[Apollo 2024 December]]"
  - "[[Apollo 2025 December]]"
  - "[[Apollo 2023 to dec 2024 General Ledger]]"
dollar-amount: 868535
direction: apollo-inflated
---

# Wire Payable Disappearance — Account 2011

## Summary

Apollo's Wire Payable account (2011) collapsed from **$869,941.75** (Dec 2024) to **$1,407.19** (Dec 2025) — a disappearance of **$868,535**. The most probable explanation is reclassification to the ATI Promissory account (2430), which appeared at $858,334.89 in 2025 with no prior balance. If confirmed, the $858K "backdated promissory note" was not new debt but a relabeling of existing Wire Payable — disguising the nature of the obligation.

## Evidence

- [[Apollo 2024 December]]: Wire Payable (2011) = $869,941.75
- [[Apollo 2025 December]]: Wire Payable (2011) = $1,407.19
- ATI Promissory (2430) went from $0.00 (Dec 2024) to $858,334.89 (Dec 2025)
- The timing of the Wire Payable collapse matches the promissory note appearance
- The dollar amounts are close: $868,535 disappeared, $858,335 appeared ($10,200 delta)

> [!MISSING-EVIDENCE]
> **To trace the reclassification:** Requires Apollo GL journal entry detail for account 2011 covering December 2024 through December 2025, showing all debit entries that reduced the Wire Payable balance. Cross-reference against account 2430 (ATI Promissory) credit entries in the same period.
> **From whom:** ATI ([[Rosanna Karim]]) — they control Apollo's QuickBooks system.
> **What it would prove:** If the Wire Payable was reclassified to ATI Promissory, the $858K note is not new debt — it's relabeled existing amounts, and the "backdating" becomes even more damning (retroactively creating a formal loan instrument for what was previously an informal clearing account).

> [!UNANALYZED-SOURCE]
> **[[Apollo 2023 to dec 2024 General Ledger]]** contains account 2011 entries that have not been specifically analyzed for the Wire Payable disappearance. A targeted review of all 2011 debits during 2024-2025 would likely reveal the reclassification trail.

## Connected

- [[Promissory Note Backdating]] — The $858K note that likely absorbed this balance
- [[Forensic Cross-Reference Report]] — Balance sheet analysis documenting the collapse
- [[Open Questions]] — Q2: Where did $868K Wire Payable go?
- [[Master Financial Reconciliation]] — E1/E2 double-counting warning
- [[Allegation Status Matrix]] — Allegation #15
