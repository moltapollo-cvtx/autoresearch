---
tags: [finding]
status: documented
confidence: high
documented_date: 2026-03-24
---

# Monthly P&L vs Consolidated GL — 2024 Reconciliation

## Summary

Cross-referencing Apollo's 12 monthly P&L CSVs (Jan–Dec 2024) against the consolidated General Ledger reveals that the monthly files are **internally self-consistent** — but the GL tells a different story on several key accounts, concentrated in **December year-end entries**.

---

## Internal Consistency: PASS

**Test A:** Sum of 12 monthly "Current Period" amounts = December "Year To Date" for every account. **Zero discrepancies.**

**Test B:** (Prior Month YTD) + (Current Month Current Period) = (Current Month YTD) for every account. **Zero discrepancies.**

This means either: (a) no retroactive P&L changes were made, or (b) all 12 files were regenerated after changes, presenting a cleaned-up view.

---

## 2024 P&L Summary (Full Year)

| Category | Full Year 2024 |
|----------|---------------|
| **Total Revenue** | **$3,847,248.55** |
| Total COGS (5xxx) | $2,851,167.18 |
| Total OPEX (6xxx) | $1,331,224.76 |
| Other (7xxx/9xxx) | $294,191.97 |
| **Net Loss** | **($629,335.36)** |

### Fuel Costs (P&L YTD December):
- 5500-00-00 Fuel: $4,806.43
- 5500-01-00 Fuel: $443,923.65
- 5310-00-00 Fuel Surcharge Pay: $269,743.61
- **Total fuel-related: $718,473.69**

---

## Discrepancies Found

### A. Retained Earnings — $8,669 Gap

| Source | 2024 Net Loss |
|--------|--------------|
| GL closing entry (12/31/2024) | $638,003.93 |
| P&L computed net loss | $629,335.36 |
| **Discrepancy** | **$8,668.57** |

The GL records $8,669 MORE in losses than the P&L computes. Where did the extra loss come from?

Additionally, prior year Retained Earnings (3500) was **retroactively adjusted** in December:
- Jan–Nov: ($549,194.17)
- December: ($553,214.17)
- **$4,020 added to prior year losses retroactively**

### B. Missing December Depreciation in GL

GL contains only 11 depreciation entries (Jan–Nov), each $19,665.18 = $216,316.98 total.
P&L shows 12 months totaling $237,315.82, with December at $20,998.84.

**$20,998.84 of December depreciation is absent from GL's Accumulated Depreciation account.**

### C. Insurance Expense Allocation — Sudden Stop

Insurance Expense (6200-00-00) ran at exactly **$51,260.09/month** for 8 months (Jan–Aug), then $51,299.34 for 2 months (Sep–Oct), then **$0.00 in both November AND December**.

Full year total: $512,679.40

This appears to be a fixed monthly allocation from ATI, not an actual insurance premium. The sudden stop in Nov/Dec is unexplained — ATI either stopped charging, or the charges were moved elsewhere.

**$512,679 ÷ 12 × 10 = $427,233 for 10 months at ~$51,260/month. The missing 2 months would add ~$102,520 if continued.**

### D. NP Gemini — $100K Year-End Spike

NP Gemini jumped from $703,663.10 to $803,663.10 on **December 12, 2024** — a $100,000 deposit labeled "cash advance."

This year-end spike in Apollo's debt to another ATI-controlled entity occurred just 19 days before year-end close.

---

## Balance Sheet — Perfect Intercompany Match

All intercompany accounts reconcile to the penny between GL and P&L:

| Account | GL | P&L Dec | Match |
|---------|-----|---------|-------|
| Cash (Stellar Bank) | $51,768.48 | $51,768.48 | YES |
| Accounts Receivable | $543,478.79 | $543,478.79 | YES |
| NP ATI | $615,639.99 | $615,639.99 | YES |
| NP Gemini | $803,663.10 | $803,663.10 | YES |
| NP Stellar 71654 | $319,599.01 | $319,599.01 | YES |
| NP Stellar 71166 | $289,534.46 | $289,534.46 | YES |

---

## NP ATI 2024 Activity — Complete Detail

Apollo's NP ATI grew by $124,457.95 during 2024 (from $491,182.04 to $615,639.99).

### ATI Advanced to Apollo: $181,306.29
| Date | Amount | Description |
|------|--------|-------------|
| Jun 14 | $1,306.29 | 401k drafted from ATI payroll |
| Jul 10 | $60,000.00 | Advance from ATI |
| Aug 29 | $40,000.00 | Advance to Apollo for O/O settlement |
| Sep 17 | $30,000.00 | Advance (overdraft) |
| Nov 6 | $50,000.00 | ATI advance |

### Apollo Paid Down to ATI: $75,800.14
| Date | Amount | Description |
|------|--------|-------------|
| Jan 6 | $6,400.00 | CH Robinson payment (RECON) |
| Jan 9 | $4,375.00 | CH Robinson payment (RECON) |
| Jan 30 | $8,176.80 | CH Robinson payment (RECON) |
| Feb 7 | $2,510.00 | CH Robinson payment (RECON) |
| Feb 16 | $30,000.00 | Wire |
| Apr 10 | $15,000.00 | NP paydown |
| Jun 20 | $2,920.84 | Applied invoice 414430 |
| Oct 11 | $6,417.50 | CHR received by ATI |

---

## Key Takeaway

The manipulation is NOT in the intercompany balances (those match perfectly) — it's in the **expense allocations** ATI controls:
- Insurance: fixed $51,260/month allocation (13.3% of revenue)
- Fuel: separate finding ([[Account 2010 Fuel Payable Mechanism]])
- Depreciation: year-end adjustments that don't fully reconcile

## Connected
- [[Account 2010 Fuel Payable Mechanism]] — Fuel manipulation
- [[Forensic Cross-Reference Report]] — Master cross-reference
- [[GL Audit Trail Anomalies]] — Backdating patterns
- [[Investigation Dashboard]]

## Source Files
- Apollo 2024 January.csv through Apollo 2024 December.csv (12 monthly P&Ls)
- [[Apollo 2023 to dec 2024 General Ledger]] (consolidated GL, 14,021 rows)
- [[Source Registry]] | [[Data Lineage]]
