---
tags: [finding]
status: documented
confidence: medium-high
estimated_impact: TBD
direction: apollo-inflated
---

# ATI Monthly Billing Manipulation

## Summary
ATI's monthly intercompany charges to Apollo were initially entered at varying amounts (consistent with actual costs), then **modified upward to a fixed amount**. The modification converts variable, verifiable costs into a flat fee that is harder to challenge and consistently higher than the original entries.

## Evidence
- Initial entries showed varying monthly amounts
- Subsequent modification changed all amounts to a fixed figure
- Modification pattern visible in the journal entry history

## Directional Analysis
Every modification moved the number upward. A fixed billing amount that exceeds actual variable costs is a direct transfer mechanism from Apollo to ATI.

## Counterarguments
- **"Flat-rate billing is common in intercompany arrangements"** — True, but the transition from variable to fixed should be documented in a formal agreement. And the flat rate should approximate actual costs, not consistently exceed them.
- **"Rounding or simplification"** — The modifications are not minor rounding; they consistently increase the billed amount.

## Source Files
- [[ATI GeneralLedger Report 2023]] — Monthly billing entries visible
- [[ATI General Ledger 2022]] — Prior year comparison
- [[Apollo QuickBooks LOGS 2022-2026]] — Apollo-side view of billing
- [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] — ATI's claimed amounts
- [[ATI GL 2023 - Intercompany Billing]] — Billing pattern analysis
- [[Source Registry]] | [[Data Lineage]]

## Action Items
- [ ] Quantify total overcharge (sum of modifications across all months)
- [ ] Request formal intercompany billing agreement documentation
- [ ] Cross-reference with bank statements for actual cash transfers
