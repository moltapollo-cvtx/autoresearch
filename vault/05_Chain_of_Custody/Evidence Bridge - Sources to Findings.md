---
type: chain-of-custody
tags: [evidence, source]
status: active
created: 2026-03-24
updated: 2026-03-24
related: ["[[Source Registry]]", "[[Data Lineage]]", "[[Investigation Dashboard]]"]
---

# Evidence Bridge — Sources to Findings

> Maps which raw source files support each finding. Every claim must trace back to at least one source. This bridge note provides a quick cross-reference.

---

## Bridge Matrix

| Finding | Confidence | Primary Sources | Independent Verification |
|---|---|---|---|
| [[Fuel Cost Manipulation]] | HIGH | [[Apollo IFTA Filing 2024]], [[ATI IFTA 2024]], [[DOC-ATI-GL-2023]], [[DOC-QB-LOGS-2022-2026]] | IFTA (govt-sworn), EFS (3rd party), Bank (independent) |
| [[Account 2010 Fuel Payable Mechanism]] | CRITICAL | [[Apollo_2010_2025_Detail]], [[Apollo_2010_Monthly_Rollforward]], [[Bank Rec Analysis 2025]] | Bank statements (independent) |
| [[Intercompany Transfer Tracker]] | CRITICAL | [[Apollo Bank Rec Jan 2024]]–[[Apollo Bank Rec DEC 2024]], [[Apollo Bank Recs 2025-TMS SYSTEM REPORT]] | Bank statements (independent) |
| [[Promissory Note Backdating]] | HIGH | [[DOC-QB-LOGS-2022-2026]], [[Apollo 2023 to dec 2024 General Ledger]] | QB timestamps (system-generated) |
| [[GL Audit Trail Anomalies]] | HIGH | [[DOC-QB-LOGS-2022-2026]], [[Apollo Quickbooks Audit Trail 2023 to dec 2024]] | QB timestamps (system-generated) |
| [[Gemini Record Manipulation]] | HIGH | [[DOC-QB-LOGS-2022-2026]], [[ATI GL 2023 - Gemini N-R Analysis]] | QB deletion log (system-generated) |
| [[Gemini Profit Siphon]] | CRITICAL | [[ATI GL 2023 - Gemini N-R Analysis]], [[ATI 2025 Profit & Loss MoM]], Gemini monthly GLs | Cross-entity P&L comparison |
| [[Forensic Cross-Reference Report]] | CRITICAL | Multiple — see [[Data Lineage]] for full chain | Multi-source triangulation |
| [[Revenue Timing Shift]] | MED-HIGH | [[Apollo ADJ Trail Balance 2024]], [[Apollo ADJ Trial Balance 2023]], [[Apollo ADJ Trial Balance 2025-QB]] | Year-over-year comparison |
| [[ATI Monthly Billing Manipulation]] | MED-HIGH | [[ATI GeneralLedger Report 2023]], [[ATI General Ledger 2022]], [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] | Multi-year comparison |
| [[Monthly GL vs Consolidated Reconciliation]] | HIGH | Apollo monthly GLs (24 files), [[Apollo ADJ Trail Balance 2024]] | Internal consistency check |

---

## Unlinked Source Files

These raw data index files are **not yet connected to any finding**:

```dataview
TABLE WITHOUT ID
  file.link AS "Source File",
  entity AS "Entity",
  period AS "Period",
  status AS "Status"
FROM "09_Raw_Data_Index"
WHERE !contains(file.outlinks, [[Fuel Cost Manipulation]])
  AND !contains(file.outlinks, [[Intercompany Transfer Tracker]])
  AND !contains(file.outlinks, [[Promissory Note Backdating]])
  AND !contains(file.outlinks, [[GL Audit Trail Anomalies]])
  AND !contains(file.outlinks, [[Gemini Record Manipulation]])
  AND !contains(file.outlinks, [[Revenue Timing Shift]])
  AND !contains(file.outlinks, [[ATI Monthly Billing Manipulation]])
  AND !contains(file.outlinks, [[Account 2010 Fuel Payable Mechanism]])
  AND !contains(file.outlinks, [[Gemini Profit Siphon]])
  AND !contains(file.outlinks, [[Forensic Cross-Reference Report]])
  AND !contains(file.outlinks, [[Monthly GL vs Consolidated Reconciliation]])
SORT entity, period
```

---

## Evidence Reliability Hierarchy

| Tier | Source Type | Can ATI Alter? | Examples |
|---|---|---|---|
| 1 — Government | IFTA filings | No (sworn) | [[Apollo IFTA Filing 2024]], [[ATI IFTA 2024]] |
| 2 — Bank | Stellar Bank statements | No (independent) | [[Bank Rec Analysis 2024]], [[Bank Rec Analysis 2025]] |
| 3 — Third-party | EFS fuel card records | No (vendor-controlled) | [[Apollo Fuel 2023 2025]], [[EFS LLC]] |
| 4 — System logs | QB timestamps, McLeod reports | Difficult (system-generated) | [[DOC-QB-LOGS-2022-2026]] |
| 5 — Internal | ATI-prepared financials | Yes (no audit trail) | [[ATI GeneralLedger Report 2023]] |

---

## Related
- [[Source Registry]] — Master file catalog
- [[Data Lineage]] — Full traceability chains
- [[Duplicate Tracker]] — Conflicting versions
- [[Evidence Tiers]] — Presentation strategy
