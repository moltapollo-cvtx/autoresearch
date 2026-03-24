---
type: finding
status: partially-documented
confidence: medium-high
tags: [finding, medium]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[ATI Monthly Billing Manipulation]]"
evidence-refs:
  - "[[APL GL work]]"
  - "[[Apollo ADJ Trail Balance 2024]]"
  - "[[Apollo ADJ Trial Balance 2023]]"
  - "[[Apollo ADJ Trial Balance 2025-QB]]"
dollar-amount: 145000
estimated_impact: "~$145K understated FY2024"
direction: apollo-inflated
---

# Revenue Timing Shift

## Summary
ATI-prepared monthly data for Apollo shows a systematic **one-month forward shift** in 2024 revenue recognition. Revenue that was earned and should have been recognized in a given month appears in the following month instead. The cumulative effect is approximately **$145K in revenue understated** (derived from [[Apollo ADJ Trail Balance 2024]], [[Apollo ADJ Trial Balance 2023]], [[Apollo ADJ Trial Balance 2025-QB]]) **in FY2024**, with corresponding overstatement in FY2025.

## Evidence
The comparison workbook (APL_GL_Comparison_Report.xlsx) was being built to document this pattern when the session was interrupted.

## Status
- [ ] **Complete the APL_GL_Comparison_Report.xlsx** with corrected P&L built from raw transaction dates
- [ ] Verify the shift pattern holds across all 12 months
- [ ] Quantify the exact impact on each period

## Directional Analysis
Understating FY2024 revenue makes Apollo appear less profitable in the completed fiscal year. This could justify lower distributions to Apollo's owner or support a narrative that Apollo needs continued ATI financial support.

## Source Files
- [[Apollo ADJ Trail Balance 2024]] — Adjusted balances (note typo: "Trail" not "Trial")
- [[Apollo ADJ Trial Balance 2023]] — Prior year comparison
- [[Apollo ADJ Trial Balance 2025-QB]] — Following year comparison
- [[Apollo Trial Balance]] — Unadjusted baseline
- [[APL GL work]] — Working analysis file
- [[Source Registry]] | [[Data Lineage]]

> [!UPGRADE-PATH] Confidence: MEDIUM-HIGH → HIGH
> **Document needed:** Completed APL_GL_Comparison_Report.xlsx — monthly revenue comparison across all 12 months of 2024, showing transaction-date revenue vs. book-date revenue for each month.
> **From whom:** Investigation team (analysis in progress, was interrupted).
> **What it would prove:** If the one-month forward shift holds across all 12 months, this becomes a systematic pattern that cannot be explained by isolated accrual timing. Upgrades from "pattern identified in partial data" to "systematic manipulation confirmed across full year."

## Counterarguments
- **"Accrual timing differences"** — Possible for individual months, but a systematic one-month shift across the year is a pattern, not a timing difference.
- **"Revenue recognition policy"** — Would need to be documented and consistently applied. A policy that systematically shifts revenue forward is unusual.
