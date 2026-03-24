---
type: dashboard
status: active
tags: [dashboard, timeline]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[Fuel Cost Manipulation]]"
  - "[[Promissory Note Backdating]]"
  - "[[Gemini Record Manipulation]]"
  - "[[GL Audit Trail Anomalies]]"
evidence-refs:
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[Intercompany Transfer Tracker]]"
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo 2023 to dec 2024 General Ledger]]"
---

# Master Timeline
> Chronological reconstruction of events. Each entry links to source evidence.

## Dataview: Auto-Pulled Timeline Events

```dataview
TABLE WITHOUT ID
  file.link AS "Note",
  documented_date AS "Date",
  dollar-amount AS "Amount ($)",
  confidence AS "Confidence"
FROM ""
WHERE documented_date AND type = "finding"
SORT documented_date ASC
```

---

## 2023 — Manipulation Events (Backdated)

| Date (Recorded) | Date (Entered) | Lag | Event | Amount | Source |
|---|---|---|---|---|---|
| 2023-04-28 | 2023-09-18 | 143 days | Fuel GJ entry #258 by [[Rosanna Karim]] | $25,521 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-05-10 | 2023-09-19 | 132 days | Fuel GJ entry #272 by Admin | $44,452 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-06-13 | 2023-09-19 | 98 days | Fuel GJ entry #273 by Admin | $39,757 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-07-13 | 2023-09-19 | 68 days | Fuel GJ entry #274 by Admin | $62,382 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-07-31 | 2023-11-02 | 94 days | Gemini NP batch entry #760 by [[Rosanna Karim]] | $17,974 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-08-16 | 2023-09-22 | 37 days | Fuel GJ entry #286 by [[Rosanna Karim]] | $36,119 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-08-31 | 2023-11-02 | 63 days | Gemini NP batch entry #761 by [[Rosanna Karim]] | $122,752 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-09-20 | **2025-01-08** | **476 days** | Fuel GJ entry #1169 "co driver fuel" by [[Cordee]] | $26,452 | [[GL Audit Trail Anomalies]] |
| 2023-09-30 | 2023-11-02 | 33 days | Gemini NP batch entry #762 by [[Rosanna Karim]] | $141,691 | [[DOC-QB-LOGS-2022-2026]] |
| 2023-10-20 | — | — | MES "overpayment for Gemini invoice 30003, 30005" | $100,218 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2023-11-02 | 2023-11-02 | 0 days | All Gemini liabilities ($282,416) batch-entered single session | $282,416 | [[Gemini Record Manipulation]] |
| 2023-12-29 | — | — | Sapphire Gas "overpayment for Gemini invoices" | $258,045 | [[Apollo 2023 to dec 2024 General Ledger]] |
| ~2023 | ~6 months later | **174 days** | $858K promissory note backdated | $858,000 | [[Promissory Note Backdating]] |
| Unknown | Unknown | — | 23 Gemini records mass-deleted by [[Cordee]] in ~25 min | — | [[Gemini Record Manipulation]] |

---

## 2024 — The Drain Year

| Date | Event | Amount | Source |
|---|---|---|---|
| 2024-01-01 | Apollo beginning balance | $364,745 | [[Bank Rec Analysis 2024]] |
| 2024-01-06 | CH Robinson payment (RECON) to ATI | -$6,400 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-01-09 | CH Robinson payment (RECON) to ATI | -$4,375 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-01-17 | ATI extraction #1 | -$50,000 | [[Apollo Bank Rec Jan 2024]] |
| 2024-01-29 | ATI extraction #2 | -$29,437 | [[Apollo Bank Rec Jan 2024]] |
| 2024-01-30 | CH Robinson payment (RECON) to ATI | -$8,177 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-02-02 | ATI extraction #3 (largest 2024) | -$100,000 | [[Apollo Bank Rec FEB 2024]] |
| 2024-02-07 | CH Robinson payment (RECON) to ATI | -$2,510 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-02-16 | ATI extraction #4 / wire to NP ATI | -$19,782 | [[Apollo Bank Rec FEB 2024]] |
| 2024-03-18 | ATI extraction #5 | -$110,453 | [[Apollo Bank Rec MAR 2024]] |
| 2024-04-10 | ATI extraction #6 (last large one) + $15K NP paydown | -$20,750 | [[Apollo Bank Rec APR 2024]] |
| 2024-05 | GIG Transportation biweekly payments cease | — | [[Bank Rec Analysis 2024]] |
| 2024-05 to 2024-10 | ATI switches to recurring ~$1,076/mo | ~-$6,456 | [[Bank Rec Analysis 2024]] |
| 2024-06-14 | ATI 401k drafted from ATI payroll (NP ATI credit) | -$1,306 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-07 | Balance hits $8,903 (97.6% decline from Jan) | — | [[Apollo Bank Rec JULY 2024]] |
| 2024-07-10 | ATI advance to Apollo | +$60,000 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-08-29 | ATI advance to Apollo (O/O settlement) | +$40,000 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-09-17 | ATI advance to Apollo (overdraft) | +$30,000 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-11 | **Account goes negative: -$44,470** | — | [[Apollo Bank Rec NOV 2024]] |
| 2024-11-06 | ATI advance to Apollo | +$50,000 | [[Apollo 2023 to dec 2024 General Ledger]] |
| 2024-12-12 | $100K deposit to NP Gemini (year-end spike) | -$100,000 | [[Monthly GL vs Consolidated Reconciliation]] |
| 2024-12-31 | Balance recovers to $61,743 | — | [[Apollo Bank Rec DEC 2024]] |

**2024 ATI total: -$335,566 out, +$181,306 advances in (NP ATI). Net cash: Apollo drained from $365K to $62K.** Source: [[Intercompany Transfer Tracker]], [[Bank Rec Analysis 2024]]

---

## 2025 — The Escalation Year

| Date | Event | Amount | Source |
|---|---|---|---|
| 2025-01-08 | [[Cordee]] enters 476-day backdated fuel entry (#1169) | -$26,452 | [[GL Audit Trail Anomalies]] |
| 2025-03-31 | **Account 2010 zeroed: "ADJ TO STMT" cash reduction** (posted 2025-06-18, 79-day lag) | -$241,284 | [[Account 2010 Fuel Payable Mechanism]] |
| 2025-03-31 | **Account 2010 zeroed: Fuel expense dump** (posted 2025-06-23, 84-day lag) | -$285,789 | [[Account 2010 Fuel Payable Mechanism]] |
| 2025-03 to 2025-05 | Q1 bank recs batch-reconciled 2025-06-18/19 (retroactive) | — | [[Bank Rec Analysis 2025]] |
| 2025-04-16 | April fuel reclass from Acct 2010 (posted 2025-06-18) | -$1,820 | [[Apollo_Manual_Journal_Fuel_Targets]] |
| 2025-05-19 | First ATI advance INTO Apollo | +$60,000 | [[Intercompany Transfer Tracker]] |
| 2025-05-23 | Second ATI advance | +$45,000 | [[Intercompany Transfer Tracker]] |
| 2025-05 | **Account goes negative: -$21,197** | — | [[Bank Rec Analysis 2025]] |
| 2025-06-03 | Gemini advance into Apollo | +$40,000 | [[Intercompany Transfer Tracker]] |
| 2025-06-17 | ATI paydown extraction begins | -$90,000 | [[Intercompany Transfer Tracker]] |
| 2025-06 to 2025-09 | Steady extraction: 6 paydowns | -$361,000 | [[Intercompany Transfer Tracker]] |
| 2025-07-15 | July fuel adj from Acct 2010 (posted 2025-08-20) | -$4,359 | [[Apollo_Manual_Journal_Fuel_Targets]] |
| 2025-10-16 | **Single largest extraction** | -$230,000 | [[Bank Rec Analysis 2025]] |
| 2025-10-31 | Loan paydown | -$125,000 | [[Bank Rec Analysis 2025]] |
| 2025-10 | **$355,000 extracted in one month (48% of inflows)** | -$355,000 | [[Bank Rec Analysis 2025]] |
| 2025-11-03 | Settlement checks voided & re-issued same day | -$61,459 | [[Bank Rec Analysis 2025]] |
| 2025-11-12 | UCNG Gemini pass-through | -$20,880 | [[Bank Rec Analysis 2025]] |
| 2025-11-19 | NP ATI Auto paydown | -$15,132 | [[Intercompany Transfer Tracker]] |
| 2025-11-30 | **"Ins/Elog" — undocumented bundled charge** | -$84,960 | [[Bank Rec Analysis 2025]] |
| 2025-12-08 | ATI note paydown | -$50,000 | [[Intercompany Transfer Tracker]] |
| 2025-12-15 | $0.00 settlement checks issued to active drivers | — | [[Bank Rec Analysis 2025]] |
| 2025-12-15 | Gemini Invoice deposit | +$6,164 | [[Bank Rec Analysis 2025]] |
| 2025-12-31 | Year-end balance: $108,490 (stmt) / $86,472 (adjusted) | — | [[Bank Rec Analysis 2025]] |

**2025 ATI total: -$866,092 out, +$285,771 in. Net: -$580,320.**

---

## Investigation Milestones

| Date | Event | Source |
|---|---|---|
| — | Investigation initiated (Project Whoopsie) | |
| — | Fuel card fraud pattern identified | [[Fuel Card Overview]] |
| — | IFTA vs P&L discrepancy quantified (~$287K) | [[Fuel Cost Manipulation]] |
| — | Grandparent company meeting prep begun | [[Evidence Tiers]] |
| 2026-03-23 | QB Transaction Log forensic analysis completed (26,993 rows) | [[DOC-QB-LOGS-2022-2026]] |
| 2026-03-23 | Bank Rec 2025 PDF analyzed & SHA-256 hashed | [[Bank Rec Analysis 2025]] |
| 2026-03-23 | **2024 bank recs ingested — two-year picture complete** | [[Bank Rec Analysis 2024]] |
| 2026-03-23 | **$1.2M gross / $916K net ATI extraction quantified** | [[Intercompany Transfer Tracker]] |
| 2026-03-24 | Account 2010 Fuel Payable mechanism identified (smoking gun) | [[Account 2010 Fuel Payable Mechanism]] |
| 2026-03-24 | Gemini Profit Siphon documented ($128K trapped) | [[Gemini Profit Siphon]] |
| 2026-03-24 | Forensic Cross-Reference Report completed (penny-level) | [[Forensic Cross-Reference Report]] |
| 2026-03-24 | Vault Pass 1 completed (schema, entities, graph, CSS) | [[CHANGELOG]] |
| 2026-03-24 | Vault Pass 2 completed (deep citations, enrichment) | [[CHANGELOG]] |

---

## Key Pattern: Year-Over-Year Escalation

| Metric | 2024 | 2025 | Trend |
|---|---|---|---|
| Gross ATI extraction | $335,566 | $866,092 | ↑ 158% |
| Net ATI extraction | $335,566 | $580,320 | ↑ 73% |
| Largest single extraction | $110,453 | $355,000 | ↑ 221% |
| ATI returned anything? | **No — zero** | Yes, starting May | New pattern |
| Account went negative? | Yes (Nov) | Yes (May) | Recurring |

The extraction is accelerating. In 2024, ATI took $336K and gave nothing back. In 2025, ATI took $866K, gave back $286K, and net drained $580K — while October alone saw $355K extracted in two transactions.

---

## Source Files & Chain of Custody
- Bank Reconciliations: [[Apollo Bank Rec Jan 2024]] through [[Apollo Bank Rec DEC 2024]], [[Apollo Bank Rec JAN 2025]], [[Apollo Bank Rec FEB 2025-QB]]
- [[Apollo Bank Recs 2025-TMS SYSTEM REPORT]] (SHA: `50f8c8bd...08923`)
- [[Apollo QuickBooks LOGS 2022-2026]] (SHA: `d918f3c9...ef9a0a82`)
- [[ATI GeneralLedger Report 2023]] | [[ATI General Ledger 2022]]
- See [[Source Registry]] for full file catalog | [[Data Lineage]] for traceability
