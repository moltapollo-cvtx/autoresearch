---
type: entity-person
tags: [entity, person, critical]
role: Controller / VP Finance
organization: "[[Asphalt Transport Inc (ATI)]]"
risk_level: high
status: confirmed
created: 2026-03-23
updated: 2026-03-24
related: ["[[Asphalt Transport Inc (ATI)]]", "[[Jimmy]]", "[[Cordee]]", "[[GL Audit Trail Anomalies]]"]
known-accounts: ["QB Admin", "Stellar Bank 21920400 (authorizer)"]
---

# Rosanna Karim

## Role & Access
- **Title:** Controller / VP Finance
- **Organization:** [[Asphalt Transport Inc (ATI)]]
- **System access:** Full administrative access to accounting system
- **Financial authority:** **Sole authorizer** of all bank transfers out of Apollo's account

## Relevance to Investigation
Rosanna is the single point of control for Apollo's finances. She is the primary user identified in the audit trail making suspicious journal entries and bulk data modifications. She has provided only partial ATI financials despite repeated requests.

## Known Actions

| Event | Evidence |
|---|---|
| Sole authorizer of all transfers from Apollo bank account | Account structure |
| Batch-entered ALL Gemini liability records in single session | [[Gemini Record Manipulation]] |
| Primary user on suspicious journal entries | [[GL Audit Trail Anomalies]] |
| Bulk data modifications in accounting system | Audit trail analysis |
| Provided only partial ATI financials despite requests | [[Outstanding Document Demands]] |
| All 12 monthly statements batch-printed same date | [[Document Registry]] |

## QB Log Statistics (from [[DOC-QB-LOGS-2022-2026]])
- **Total entries:** 4,924 (18.2% of all transactions)
- **General Journal entries:** 2,651 (**47.5% of ALL GJ entries in the system**)
- **Backdating >30 days:** 1,942 entries (39.4% of her entries)
- **Avg backdating lag:** 36 days
- **Max backdating lag:** 300 days

## Known Accounts
- QuickBooks administrative access (full system control)
- Sole authorizer of bank transfers from Apollo Stellar Bank account 21920400

## Key Transactions
| Date | Amount | Type | Source |
|------|--------|------|--------|
| 2023-04-28 | $25,520.83 | Fuel GJ (Trans #258) | [[DOC-QB-LOGS-2022-2026]] |
| 2023-05-10 | $44,452.17 | Fuel GJ (Trans #272) | [[DOC-QB-LOGS-2022-2026]] |
| 2023-06-13 | $39,756.77 | Fuel GJ (Trans #273) | [[DOC-QB-LOGS-2022-2026]] |
| 2023-07-13 | $62,382.14 | Fuel GJ (Trans #274) | [[DOC-QB-LOGS-2022-2026]] |
| 2023-08-16 | $36,119.05 | Fuel GJ (Trans #286) | [[DOC-QB-LOGS-2022-2026]] |
| 2023-11-02 | $282,416.38 | Gemini NP batch (Trans #760-762) | [[DOC-QB-LOGS-2022-2026]] |
| 2025-03-31 | $285,789.46 | Acct 2010 fuel dump (posted 2025-06-23) | [[Apollo_Manual_Journal_Fuel_Targets]] |
| 2025-03-31 | $241,284.09 | ADJ TO STMT (posted 2025-06-18) | [[Apollo_Manual_Journal_Fuel_Targets]] |

## Connected Findings
- [[Fuel Cost Manipulation]] — Posted 2 of 6 undocumented "fuel" GJ entries ($61,640)
- [[Gemini Record Manipulation]] — Batch-entered ALL Gemini liabilities ($282,416)
- [[GL Audit Trail Anomalies]] — Controls 47.5% of all GJ entries; 39.4% backdated
- [[ATI Monthly Billing Manipulation]] — Primary operator of intercompany entries
- [[Promissory Note Backdating]] — Primary system user for $858K note
- [[Intercompany Transfer Tracker]] — Sole authorizer of all bank transfers out
- [[Revenue Timing Shift]] — Controlled the revenue recognition process

## Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — Activity documented (SHA: `d918f3c9...ef9a0a82`)
- [[ATI GeneralLedger Report 2023]] — ATI-side entries

## Strategic Notes
Strong ego — communications should be crafted to secure commitments without triggering defensive responses.
