---
tags: [chain-of-custody]
status: active
updated: 2026-03-24
---

# Duplicate Tracker

> Tracks overlapping, duplicate, or conflicting data across raw files. When versions conflict, this note documents which is authoritative and why.

## Known Overlaps

### 1. Apollo Monthly GL CSVs vs. Consolidated GL
- **Files:** Apollo 2024 {Month}.csv (×12) + Apollo 2025 {Month}.csv (×12) vs. [[Apollo 2023 to dec 2024 General Ledger]]
- **Overlap:** The consolidated GL covers 2023–Dec 2024, overlapping with all 12 monthly 2024 CSVs
- **Resolution:** Monthly CSVs are point-in-time snapshots. Consolidated GL may reflect retroactive changes. **Compare totals** — any discrepancy is evidence of post-hoc manipulation.
- **Status:** Needs reconciliation
- **Significance:** HIGH — if consolidated GL differs from sum of monthly snapshots, it proves retroactive alteration

### 2. Apollo Trial Balances (Multiple Versions)
- **Files:** [[Apollo ADJ Trail Balance 2024]] (note typo: "Trail"), [[Apollo ADJ Trial Balance 2023]], [[Apollo ADJ Trial Balance 2025-QB]], [[Apollo Trial Balance]]
- **Overlap:** Multiple trial balance files covering overlapping periods
- **Resolution:** The "ADJ" versions are adjusted trial balances (post-adjusting entries). The plain "Apollo Trial Balance.CSV" may be unadjusted. Compare to identify what adjustments were made.
- **Status:** Needs reconciliation
- **Significance:** MEDIUM — adjusting entries are where manipulation hides

### 3. Apollo QB Logs vs. Audit Trail
- **Files:** [[Apollo QuickBooks LOGS 2022-2026]] vs. [[Apollo Quickbooks Audit Trail 2023 to dec 2024]]
- **Overlap:** Both cover 2023-2024 period from QuickBooks
- **Resolution:** QB Logs (xlsm) is the primary analyzed source (26,993 transactions). Audit Trail (CSV) may contain different data fields. Cross-reference for completeness.
- **Status:** QB Logs is primary; Audit Trail supplementary
- **Significance:** MEDIUM — Audit Trail may show edit history not in transaction log

### 4. September 2024 Bank Recs (Two Files)
- **Files:** [[Apollo Bank Rec Sept 1 2024]] vs. [[Apollo Bank Rec SEPT 30-2024]]
- **Overlap:** Both cover September 2024
- **Resolution:** Likely two separate reconciliation periods within September (split month). Verify date ranges. Both feed into [[Bank Rec Analysis 2024]].
- **Status:** Needs verification
- **Significance:** LOW — likely legitimate split-month reconciliation

### 5. ATI Fuel Data (Multiple Sources)
- **Files:** [[ATI Fuel 2023 2025]] (xlsx, 2023-2025) vs. [[ATI FUEL 2024]] (pdf, 2024 only)
- **Overlap:** 2024 fuel data appears in both files
- **Resolution:** The xlsx is the broader dataset. The PDF may be a report or printout. Compare 2024 figures.
- **Status:** Needs reconciliation
- **Significance:** HIGH — fuel cost discrepancy is a core finding ([[Fuel Cost Manipulation]])

### 6. IFTA Filings (Apollo vs ATI)
- **Files:** Apollo IFTA (2024 csv + 2025 pdf) vs. ATI IFTA (2024 csv + 2025 pdf)
- **Overlap:** Not duplicates but should be cross-referenced — Apollo's IFTA fuel costs should NOT appear on ATI's IFTA and vice versa
- **Resolution:** Compare fuel volumes. If ATI's IFTA understates by ~$2M and Apollo's overstates by ~$287K, that confirms the directional pattern.
- **Status:** Partially analyzed in [[Fuel Cost Manipulation]]
- **Significance:** CRITICAL — government-sworn documents that contradict ATI's internal books

### 7. Apollo Fuel Sources
- **Files:** [[Apollo Fuel 2023 2025]] vs. fuel entries in [[Apollo QuickBooks LOGS 2022-2026]] vs. [[Apollo_Manual_Journal_Fuel_Targets]]
- **Overlap:** All contain fuel cost data for Apollo
- **Resolution:** The "Manual Journal Fuel Targets" file name itself is suspicious — suggests targeted journal entries for fuel. Compare against EFS/IFTA actuals.
- **Status:** Needs deep analysis
- **Significance:** CRITICAL — this may document the mechanism for fuel cost inflation

### 8. Apollo_2010 Files
- **Files:** [[Apollo_2010_2025_Detail]] vs. [[Apollo_2010_Monthly_Rollforward]]
- **Overlap:** Both reference "2010" account (likely an account number, not year 2010)
- **Resolution:** Detail is transaction-level, Rollforward is monthly summary. Should reconcile.
- **Status:** Needs analysis
- **Significance:** MEDIUM — depends on what account 2010 is

## Deconfliction Rules
1. **Government filings > Internal books** — IFTA filings are sworn; internal GL can be altered
2. **Bank statements > Internal books** — Stellar Bank data is independent
3. **Point-in-time snapshots > Consolidated reports** — Consolidation allows retroactive changes
4. **Earlier-dated exports > Later-dated exports** — Later exports may reflect alterations
5. **Third-party data (EFS) > ATI-controlled data** — EFS fuel card records can't be altered by ATI

## Related
- [[Source Registry]]
- [[Data Lineage]]
- [[Fuel Cost Manipulation]]
- [[GL Audit Trail Anomalies]]
