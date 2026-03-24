---
tags: [finding]
status: documented
confidence: high
estimated_impact: "~$287K"
direction: both
---

# Fuel Cost Manipulation

## Summary
Apollo's ATI-prepared P&L reports fuel costs of approximately $720K. However, Apollo's own IFTA filing — a government-sworn document — reports approximately 145K gallons at a total cost of ~$433K, corroborated by EFS fuel card transaction records. The difference is approximately **$287K, a ~66% markup** with no documented basis. Simultaneously, ATI's own IFTA understates its fuel cost by ~$2M. Both discrepancies move money in the same direction: Apollo's expenses inflated, ATI's expenses deflated.

## Evidence Chain

### Independent / External Sources
1. **Apollo IFTA filing** — ~145K gallons, ~$433K total fuel cost. Government-sworn, filed with state authorities, cannot be retroactively altered by ATI.
2. **EFS fuel card records** — Corroborate the IFTA gallonage and spend figures. Third-party data held by EFS, not ATI.

### Internal Sources (ATI-controlled)
1. **ATI-prepared Apollo P&L** — Shows ~$720K in fuel costs for the same period.
2. **ATI's own IFTA** — Understates ATI's fuel cost by ~$2M (mirror image pattern).

### The Discrepancy
- **IFTA/EFS say:** ~$433K
- **ATI's books say:** ~$720K
- **Gap:** ~$287K (~66% markup)
- **Direction:** Apollo overstated, ATI understated — consistent across entities

## Directional Analysis
This is the single largest identified discrepancy. The overstatement appears on Apollo's expense line (reducing Apollo's apparent profitability), while ATI's books show the mirror — understating their own fuel costs. This is consistent with profits being siphoned from Apollo to ATI.

## Counterarguments
- **"Volume discounts or rebates could explain the gap"** — Possible but would need to be documented. We've requested volume discount agreements. Even so, discounts would reduce cost, not increase it. The gap goes the wrong direction for this explanation.
- **"Different accounting periods or accrual basis"** — IFTA covers a defined period. A ~66% markup cannot be explained by timing differences alone.
- **"ATI incurs fuel costs on Apollo's behalf not captured in IFTA"** — Possible in theory, but would need documentation and would need to show ~$287K in non-IFTA fuel purchases, which is implausible for the fleet size.

## Action Items
- [ ] Obtain unaltered EFS portal exports to confirm card-level detail
- [ ] Pull transaction reports for prioritized cards (see [[Fuel Card Overview]])
- [ ] Request documentation for any fuel charges beyond IFTA-reported volumes
- [ ] Cross-reference with [[Stellar Bank]] statements for actual cash outflows to fuel vendors


---

## NEW: 2023 GL Evidence — The Mechanism Exposed

The ATI GL Report for 2023 ([[ATI GL 2023 - Apollo N-R Analysis]]) reveals **exactly how** the fuel overstatement works:

ATI posts single-line journal entries labeled "fuel" directly to the "N/R Apollo Energy" account — no invoices, no supporting detail, no reference to specific EFS transactions. Six entries totaling **$234,683** were made between April and September 2023. These are general journal entries (not AP transactions), meaning they bypass the normal purchase/payment cycle entirely.

This is the direct link between "ATI controls the books" and "Apollo's fuel costs are inflated." The fuel charges aren't traceable to actual fuel purchases — they're arbitrary round-ish numbers posted as journal entries.

---

## QB Transaction Log Confirmation (Added 03/23/2026)

Source: [[DOC-QB-LOGS-2022-2026]]

The fuel-to-NP-ATI journal entries are **confirmed from Apollo's side**. The following GJ entries debit "Fuel Expense - Company" and credit "NP ATI" — simultaneously inflating Apollo's fuel cost and increasing Apollo's recorded debt to ATI:

| Trans# | Tx Date | Entered | By | Amount | Memo |
|---|---|---|---|---|---|
| 258 | 04/28/2023 | 09/18/2023 | Rosanna | $25,520.83 | fuel |
| 272 | 05/10/2023 | 09/19/2023 | Admin | $44,452.17 | fuel |
| 273 | 06/13/2023 | 09/19/2023 | Admin | $39,756.77 | fuel |
| 274 | 07/13/2023 | 09/19/2023 | Admin | $62,382.14 | fuel |
| 286 | 08/16/2023 | 09/22/2023 | Rosanna | $36,119.05 | fuel |
| **1169** | **09/20/2023** | **01/08/2025** | **Cordee** | **$26,451.77** | **co driver fuel** |
| **Total** | | | | **$234,682.73** | |

The sixth entry (Trans #1169) was entered **476 days** after its transaction date — the most extreme backdating in the entire dataset. All six entries were made as General Journal entries, bypassing the AP/AR cycle entirely.

**Total fuel charged to NP ATI via journal entries: $234,683 (2023) + potential additional amounts in 2024-2025 via different mechanism**

## Source Files
- [[Apollo IFTA Filing 2024]] — Government-sworn fuel data (independent)
- [[Apollo 2025 IFTA Filing]] — Government-sworn fuel data (independent)
- [[ATI IFTA 2024]] — ATI's IFTA filing (understates by ~$2M)
- [[ATI 2025 IFTA Filing]] — ATI's 2025 IFTA
- [[Apollo Fuel 2023 2025]] — EFS fuel card transaction data
- [[ATI Fuel 2023 2025]] — ATI fuel records
- [[ATI FUEL 2024]] — ATI 2024 fuel report
- [[Apollo QuickBooks LOGS 2022-2026]] — QB-side confirmation of 6 GJ entries
- [[ATI GeneralLedger Report 2023]] — ATI-side GL showing mechanism
- [[Apollo_Manual_Journal_Fuel_Targets]] — Suspicious: manual journal fuel targets
- [[Fuel_vs_Financials_Forensic_Report]] — Pre-existing forensic analysis
- [[Source Registry]] | [[Data Lineage]] | [[Duplicate Tracker]]
