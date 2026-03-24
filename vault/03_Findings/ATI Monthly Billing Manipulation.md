---
type: finding
status: documented
confidence: medium-high
tags: [finding, medium]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[Fuel Cost Manipulation]]"
  - "[[Revenue Timing Shift]]"
evidence-refs:
  - "[[ATI GeneralLedger Report 2023]]"
  - "[[ATI General Ledger 2022]]"
  - "[[Apollo QuickBooks LOGS 2022-2026]]"
  - "[[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]]"
estimated_impact: 0
direction: apollo-inflated
---

# ATI Monthly Billing Manipulation

## Summary
ATI's monthly intercompany charges to Apollo were initially entered at varying amounts (consistent with actual costs), then **modified upward to a fixed amount** ([[ATI GL 2023 - Intercompany Billing]], [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]]). The modification converts variable, verifiable costs into a flat fee that is harder to challenge and consistently higher than the original entries.

> [!MISSING-EVIDENCE]
> **To quantify total overcharge:** Requires ATI's intercompany billing invoices to Apollo covering 2022-01 through 2025-12, showing per-month original variable amounts vs. modified fixed amounts. Cross-reference against [[ATI GeneralLedger Report 2023]] and [[ATI General Ledger 2022]] intercompany billing sections. Without itemized invoices, the total overcharge cannot be calculated. Confidence remains **medium**.

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

> [!UPGRADE-PATH] Confidence: MEDIUM-HIGH → HIGH
> **Document needed:** ATI's intercompany billing agreement with Apollo — the formal document (if any) governing what ATI may charge Apollo for management fees, insurance, equipment, and services.
> **From whom:** ATI ([[Rosanna Karim]] / [[James Luhr Jr]]) — demanded in [[Document Demand Letter Template]] Category C, Item 10.
> **What it would prove:** If no agreement exists, every intercompany charge is unilateral and unjustified. If an agreement exists, compare its terms to actual billing — any deviation is a breach. Either outcome quantifies the total overcharge.

## Action Items
- [ ] Quantify total overcharge (sum of modifications across all months)
- [ ] Request formal intercompany billing agreement documentation
- [ ] Cross-reference with bank statements for actual cash transfers
