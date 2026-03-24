---
type: chain-of-custody
status: active
confidence: high
tags: [chain-of-custody]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Source Registry]]"
  - "[[Duplicate Tracker]]"
  - "[[Document Registry]]"
evidence-refs: []
---

# Data Lineage

> Traces the path from raw data files through analysis to findings and deliverables. Every finding must have an unbroken chain back to source files.

## Lineage Map

### Finding 1: Fuel Cost Manipulation (~$287K)
```
RAW DATA (Independent):
  [[Apollo IFTA Filing 2024]] → ~145K gal, ~$433K fuel
  [[Apollo 2025 IFTA Filing]] → IFTA fuel figures
  [[ATI IFTA 2024]] → ATI understates fuel by ~$2M
  [[ATI 2025 IFTA Filing]] → ATI IFTA figures
  [[Apollo Fuel 2023 2025]] → EFS fuel card data
  [[ATI Fuel 2023 2025]] → ATI fuel records

RAW DATA (ATI-controlled):
  [[ATI GeneralLedger Report 2023]] → 6 GJ entries = $234,683 "fuel"
  [[Apollo QuickBooks LOGS 2022-2026]] → Confirms same 6 entries from Apollo side
  [[Apollo_Manual_Journal_Fuel_Targets]] → Suspicious: manual journal targets for fuel

ANALYSIS:
  → [[Fuel Card Overview]] (card-level detail)
  → [[Fuel Spend Reconciliation]] (IFTA vs P&L comparison)
  → [[ATI GL 2023 - Apollo N-R Analysis]] (mechanism documentation)
  → [[DOC-QB-LOGS-2022-2026]] (QB-side confirmation)

FINDING:
  → [[Fuel Cost Manipulation]] ($287K markup, 66%)

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Must Hit")
```

### Finding 2: Net Cash Extraction ($915,887)
```
RAW DATA:
  [[Apollo Bank Rec Jan 2024]] through [[Apollo Bank Rec DEC 2024]] (13 files)
  [[Apollo Bank Rec JAN 2025]] + [[Apollo Bank Rec FEB 2025-QB]]
  [[Apollo Bank Recs 2025-TMS SYSTEM REPORT]] (SHA: 50f8c8bd...)
  [[Apollo bank transfers 2025]]

ANALYSIS:
  → [[Bank Rec Analysis 2024]] ($335,566 extracted, zero returned)
  → [[Bank Rec Analysis 2025]] ($866,092 gross, $580,321 net)
  → [[Intercompany Transfer Tracker]] (combined two-year view)
  → [[Cash Flow Dashboard]]

FINDING:
  → [[Intercompany Transfer Tracker]] ($1,201,658 gross / $915,887 net)

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Must Hit")
```

### Finding 3: Promissory Note Backdating ($858K)
```
RAW DATA:
  [[Apollo QuickBooks LOGS 2022-2026]] → Entry creating promissory note
  [[Apollo 2023 to dec 2024 General Ledger]] → GL record

ANALYSIS:
  → [[DOC-QB-LOGS-2022-2026]] → Backdating analysis
  → [[GL Audit Trail Anomalies]] → Pattern documentation

FINDING:
  → [[Promissory Note Backdating]] ($858K, 174-day backdate)

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Must Hit")
```

### Finding 4: GL Audit Trail Anomalies (476-day backdate)
```
RAW DATA:
  [[Apollo QuickBooks LOGS 2022-2026]] → Full transaction log (26,993 entries)
  [[Apollo Quickbooks Audit Trail 2023 to dec 2024]] → Supplementary audit trail

ANALYSIS:
  → [[DOC-QB-LOGS-2022-2026]] → User analysis, backdating statistics
  → [[Rosanna Karim]] profile (47.5% of GJ entries, 39.4% backdated >30d)
  → [[Cordee]] profile (476-day backdated entry #1169)

FINDING:
  → [[GL Audit Trail Anomalies]]

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Must Hit")
```

### Finding 5: Revenue Timing Shift (~$145K)
```
RAW DATA:
  [[Apollo ADJ Trail Balance 2024]] → Adjusted balances
  [[Apollo ADJ Trial Balance 2023]] → Prior year comparison
  [[Apollo ADJ Trial Balance 2025-QB]] → Following year comparison
  [[Apollo Trial Balance]] → Unadjusted baseline

ANALYSIS:
  → Revenue recognition timing analysis (1-month forward shift)

FINDING:
  → [[Revenue Timing Shift]] (~$145K understated in FY2024)

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Ought to Hit")
```

### Finding 6: ATI Monthly Billing Manipulation
```
RAW DATA:
  [[ATI GeneralLedger Report 2023]] → Monthly billing entries
  [[ATI General Ledger 2022]] → Prior year comparison
  [[Apollo QuickBooks LOGS 2022-2026]] → Apollo-side view
  [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] → ATI's claimed amounts

ANALYSIS:
  → [[ATI GL 2023 - Intercompany Billing]] → Billing pattern analysis

FINDING:
  → [[ATI Monthly Billing Manipulation]]

STRATEGY:
  → [[Evidence Tiers]] (Tier: "Ought to Hit")
```

### Finding 7: Gemini Record Manipulation (23 records deleted)
```
RAW DATA:
  [[Gemini January 2024]] through [[Gemini December 2024]] (12 files)
  [[Gemini 2025 January]] through [[Gemini 2025 December]] (12 files)

ANALYSIS:
  → [[ATI GL 2023 - Gemini N-R Analysis]] → Gemini intercompany analysis

FINDING:
  → [[Gemini Record Manipulation]] (23 records mass-deleted by [[Cordee]])

STRATEGY:
  → [[Evidence Tiers]]
```

## Unanalyzed Files (No Finding Yet)
These raw files have been indexed but not yet connected to a finding:

| File | Potential Relevance |
|------|-------------------|
| [[Apollo 2026 Chart of Accounts]] | Account structure — may reveal hidden accounts |
| [[APL GL work]] | Working analysis file — review for additional insights |
| [[Apollo_2010_2025_Detail]] | Account 2010 detail — identify what account this is |
| [[Apollo_2010_Monthly_Rollforward]] | Account 2010 rollforward — monthly movement |
| [[ATI 2025 Profit & Loss MoM]] | ATI P&L — compare against Apollo P&L for directional analysis |
| [[Fuel_vs_Financials_Forensic_Report]] | Pre-existing forensic analysis — review methodology |

## Chain Integrity Rules
1. Every finding MUST trace to at least one raw file
2. Every raw file with analytical value MUST connect to an evidence note
3. No finding should rely solely on ATI-controlled sources without independent corroboration
4. Each link in the chain must be documented with specific reference (page, row, cell)

## Related
- [[Source Registry]]
- [[Duplicate Tracker]]
- [[Investigation Dashboard]]
- [[Evidence Tiers]]
