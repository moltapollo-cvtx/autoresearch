---
type: dashboard
tags: [dashboard]
status: active
created: 2026-03-24
updated: 2026-03-24
---

# Map of Content — Master Hub

> Central navigation hub linking every cluster in the investigation vault.

---

## Dashboards & Navigation
- [[Investigation Dashboard]] — **Start here.** All findings, entity map, methodology
- [[Cash Flow Dashboard]] — Follow the money: headline numbers, balance trajectory, fuel gap
- [[Master Timeline]] — Chronological event reconstruction (2023–2025)
- [[Document Registry]] — Every document received, logged with timestamps and hashes
- [[AUDIT]] — Vault audit report

---

## Entities

### Companies
| Entity | Role | Key Finding Link |
|---|---|---|
| [[Asphalt Transport Inc (ATI)]] | Parent/controller | [[Intercompany Transfer Tracker]] |
| [[Apollo Energy Resources LLC]] | Subsidiary/victim | [[Cash Flow Dashboard]] |
| [[Gemini Logistics USA LLC]] | Related entity | [[Gemini Profit Siphon]] |
| [[Stellar Bank]] | Apollo's bank | [[Bank Rec Analysis 2024]] |
| [[EFS LLC]] | Fuel card provider | [[Fuel Spend Reconciliation]] |
| [[GIG Transportation Services]] | Suspected Gemini affiliate | [[Bank Rec Analysis 2024]] |

### People
| Person | Role | Risk | Key Link |
|---|---|---|---|
| [[Jimmy]] | ATI President | HIGH | [[Asphalt Transport Inc (ATI)]] |
| [[Rosanna Karim]] | Controller/VP Finance | **CRITICAL** | [[GL Audit Trail Anomalies]] |
| [[Cordee]] | Team member | HIGH | [[Gemini Record Manipulation]] |
| [[Walker]] | Apollo Owner | COMPLAINANT | [[Investigation Dashboard]] |
| [[James Luhr Jr]] | Signatory | MEDIUM | [[Promissory Note Backdating]] |
| [[Henry Collins]] | Terminated driver | HIGH | [[Card 0048 - Henry Collins]] |
| [[Cody]] | Team member | LOW | [[Apollo Energy Resources LLC]] |
| [[Mauree]] | Data entry | CLOSED | [[Other Flagged Users]] |
| [[Martha]] | Deleted QB user | LOW | [[Other Flagged Users]] |
| [[McLeod]] | System user | LOW | [[DOC-BankRec-2025-McLeod]] |
| [[Other Flagged Users]] | Various | VARIES | [[DOC-QB-LOGS-2022-2026]] |

---

## Findings (by confidence)

### Critical
- [[Forensic Cross-Reference Report]] — Master cross-reference of all evidence streams
- [[Account 2010 Fuel Payable Mechanism]] — $285,789 fuel + $241,284 cash dump (SMOKING GUN)
- [[Gemini Profit Siphon]] — $127,964 trapped + $212,945 phantom debt

### High
- [[Fuel Cost Manipulation]] — ~$287K overstatement, 66% markup
- [[Promissory Note Backdating]] — $858K note, 174-day backdate
- [[GL Audit Trail Anomalies]] — 476-day backdated entry, no audit trail
- [[Gemini Record Manipulation]] — 23 records mass-deleted in 25 minutes
- [[Monthly GL vs Consolidated Reconciliation]] — Internal consistency check

### Medium
- [[ATI Monthly Billing Manipulation]] — Variable→fixed billing modification
- [[Revenue Timing Shift]] — ~$145K understated FY2024

---

## Evidence Clusters

### Bank Statements
- [[Bank Rec Analysis 2024]] — Full year 2024 ($335,566 extracted, zero returned)
- [[Bank Rec Analysis 2025]] — Full year 2025 ($866,092 gross, $580,320 net)
- [[DOC-BankRec-2025-McLeod]] — Source document wrapper (SHA-256 verified)

### Fuel Cards
- [[Fuel Card Overview]] — 10 card inventory, priority order, fraud patterns
- [[Card 0048 - Henry Collins]] — Highest-spend card, terminated driver

### General Ledger
- [[DOC-ATI-GL-2023]] — ATI GL source document (266,513 rows)
- [[DOC-QB-LOGS-2022-2026]] — QB Transaction Log (26,993 rows, SHA-256 verified)
- [[ATI GL 2023 - Apollo N-R Analysis]] — $510K claimed receivable mechanism
- [[ATI GL 2023 - Gemini N-R Analysis]] — $341K Gemini intercompany
- [[ATI GL 2023 - Intercompany Billing]] — $311K billing analysis

---

## Cash Flow
- [[Intercompany Transfer Tracker]] — $1.2M gross / $916K net extraction (2024+2025)
- [[Fuel Spend Reconciliation]] — Three-source comparison + bank-level EFS payments

---

## Chain of Custody
- [[Source Registry]] — Master catalog of 90+ raw files with SHA-256 hashes
- [[Data Lineage]] — Raw file → analysis → finding → deliverable traceability
- [[Duplicate Tracker]] — Conflicting/overlapping data versions and deconfliction rules

---

## Strategy & Deliverables
- [[Evidence Tiers]] — Must Hit / Ought to Hit / Should Hit / 50-50 / Leave Alone
- [[Grandparent Meeting Prep]] — Meeting objectives, framing, risk assessment
- [[Outstanding Document Demands]] — Critical documents still needed
- [[Deliverables Index]] — Formal documents produced from the investigation

---

## Raw Data Index
> 90+ source file index notes organized by entity. See [[Source Registry]] for the master catalog.

- `09_Raw_Data_Index/ATI/` — 7 ATI source files
- `09_Raw_Data_Index/Apollo/` — ~55 Apollo source files (GL, bank recs, IFTA, fuel, trial balances)
- `09_Raw_Data_Index/Gemini/` — 24 Gemini monthly GL files

---

## Graph Narratives

| Narrative | Description | Key Entry Points |
|---|---|---|
| **Concepts** | Forensic concepts (fuel markup, backdating, extraction) | [[Evidence Tiers]], [[Fuel Cost Manipulation]] |
| **Sources** | Raw documents and chain of custody | [[Source Registry]], [[Data Lineage]] |
| **People** | Named individuals and roles | [[Rosanna Karim]], [[Jimmy]], [[Walker]] |
| **Entities** | Companies and accounts | [[Asphalt Transport Inc (ATI)]], [[Apollo Energy Resources LLC]] |
| **Findings** | Numbered findings with confidence | [[Investigation Dashboard]], [[Forensic Cross-Reference Report]] |
| **Timeline** | Chronological events | [[Master Timeline]] |
