---
tags: [document, evidence, gl-entry]
doc_id: DOC-QB-LOGS-2022-2026
received_date: 2026-03-23
received_from: Walker (uploaded to investigation)
generation_date: unknown
sha256: d918f3c9134d06e26fd2724abd8806c22090e5d8a3976f5f64e9a503ef9a0a82
status: under-review
---

# Apollo QuickBooks Transaction Log — Jan 2022 to Mar 2026

## Receipt Details
- **Received:** 2026-03-23 (uploaded to investigation)
- **File:** Apollo_QB_LOGS_2022-2026.xlsm
- **Format:** Excel with macros (.xlsm) — 26,993 data rows, 100 columns (50 data + 50 spacers), single sheet
- **Period:** Transaction dates Feb 2023 – Apr 2025; Entry dates Jun 2023 – May 2025

## Document Description
This is the complete Apollo-side QuickBooks transaction log — every transaction entered into Apollo's books across the full investigation period. Contains transaction number, type, transaction date, entry/modification date, modifying user, account, debit/credit amounts, memo, and payee/vendor information.

## Critical Metadata

### User Activity Summary
| User | Entries | % of Total | GJ Entries | Notes |
|---|---|---|---|---|
| Cordee | 11,698 | 43.3% | 760 | Most active user; 476-day backdated entry |
| Rosanna | 4,924 | 18.2% | 2,651 | Controls 47.5% of all GJ entries; avg 36-day lag |
| Mauree | 4,379 | 16.2% | 699 | **NEW — unidentified user, needs immediate ID** |
| Martha [Deleted User] | 3,030 | 11.2% | 479 | Account deleted — audit trail destruction |
| Admin | 2,819 | 10.4% | 896 | Generic account |
| Rikki | 111 | 0.4% | 95 | |
| walker | 21 | 0.1% | 0 | Walker's own entries |
| Jimmy | 10 | <0.1% | 0 | ATI President — minimal direct involvement |

### Transaction Type Summary
| Type | Count | Manipulation Risk |
|---|---|---|
| Invoice | 10,039 | Low (revenue recognition) |
| Bill | 8,055 | Medium (expense recognition) |
| **General Journal** | **5,580** | **HIGH — bypasses AP/AR cycle** |
| Bill Pmt -Check | 1,490 | Low |
| Deposit | 755 | Medium |
| Payment | 680 | Low |

### Key Account Activity
| Account | Entries | Notes |
|---|---|---|
| Driver Advances | 3,567 | Largest single account |
| Accounts Receivable | 2,427 | Revenue tracking |
| Fuelsurcharge | 1,946 | Revenue line |
| Stellar Bank | 1,822 | Cash account |
| Purchased Transportation | 1,546 | O/O settlements + fuel advances |
| NP ATI | 79 (GJ only) | **Intercompany debt — all manipulation risk** |
| N/P Gemini | 3 (GJ only) | $282,417 in "reconciliation adj" entries |

## Cross-References
- [[GL Audit Trail Anomalies]] — Backdating confirmed with exact timestamps
- [[Fuel Cost Manipulation]] — Fuel-to-NP-ATI journal entries confirmed from Apollo side
- [[Gemini Record Manipulation]] — N/P Gemini batch entries confirmed
- [[Promissory Note Backdating]] — Equipment loan entries ($293,750) confirmed
- [[Other Flagged Users]] — Mauree/Martha downgraded (incompetent, not malicious)
- [[Mauree]] — Not a subject (routine fuel card settlements)
- [[ATI Monthly Billing Manipulation]] — Intercompany billing visible in GJ entries

## Source File
- [[Apollo QuickBooks LOGS 2022-2026]] — Raw data index note (SHA: `d918f3c9...ef9a0a82`)
- [[Apollo Quickbooks Audit Trail 2023 to dec 2024]] — Supplementary audit trail

## Chain of Custody
- [[Source Registry]] | [[Data Lineage]] | [[Duplicate Tracker]]

## Entities
- [[Apollo Energy Resources LLC]] | [[Asphalt Transport Inc (ATI)]] | [[Gemini Logistics USA LLC]]
- [[Rosanna Karim]] | [[Cordee]] | [[Jimmy]] | [[Mauree]]
