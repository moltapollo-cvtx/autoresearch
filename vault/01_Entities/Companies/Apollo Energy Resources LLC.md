---
type: entity-company
tags: [entity, company]
parent: "[[Asphalt Transport Inc (ATI)]]"
status: confirmed
created: 2026-03-23
updated: 2026-03-24
related: ["[[Asphalt Transport Inc (ATI)]]", "[[Gemini Logistics USA LLC]]", "[[Stellar Bank]]"]
total-extracted: -915887
key-accounts: ["Stellar Bank 21920400", "EFS Carrier ID 5725124", "QB GL 1000-00-00"]
---

# Apollo Energy Resources LLC

## Structure
- **Parent entity:** [[Asphalt Transport Inc (ATI)]]
- **Grandparent:** ATI's parent company (target audience for evidence presentation)
- **Owner:** Walker
- **Team:** [[Cordee]], [[Cody]]

## Financial Footprint
- **EFS Carrier ID:** 5725124
- **Bank:** [[Stellar Bank]] — Account 21920400
- **Accounting system:** Controlled exclusively by ATI. No audit trail. Apollo has no independent access.

## The Core Problem
Apollo generates revenue and incurs costs, but ATI exclusively controls all bank accounts, cash flows, asset titles, the accounting system, and financial record-keeping. Walker, as owner, cannot independently verify what ATI reports.

## Key Accounts
| Account | Type | Controlled By |
|---------|------|--------------|
| Stellar Bank 21920400 | Operating bank account | [[Rosanna Karim]] (sole authorizer) |
| EFS Carrier ID 5725124 | Fuel card carrier | ATI |
| GL 1000-00-00 | Cash account | ATI (no audit trail) |
| GL 2010-00-00 | Fuel Payable | ATI — accumulated $322,639 in 2024 |
| GL 2410 | NP Gemini | $924,186 (Dec 2025) |
| GL 2420 | NP ATI | $534,601 (Dec 2025) |
| GL 2430 | ATI Promissory | $858,335 (backdated) |

## Connected Findings
- [[Fuel Cost Manipulation]] — P&L inflated by ~$287K on fuel
- [[Revenue Timing Shift]] — ~$145K revenue shifted out of FY2024
- [[ATI Monthly Billing Manipulation]] — Intercompany charges inflated
- [[Promissory Note Backdating]] — $858K note backdated 174 days
- [[Fuel Card Overview]] — 10 masked fuel cards under investigation
- [[GL Audit Trail Anomalies]] — No audit trail, 476-day backdated entry
- [[Intercompany Transfer Tracker]] — $1.2M gross / $916K net extracted

## Key Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — Full transaction log (SHA: `d918f3c9...ef9a0a82`)
- [[Apollo 2023 to dec 2024 General Ledger]] — Consolidated GL
- [[Apollo IFTA Filing 2024]] | [[Apollo 2025 IFTA Filing]] — Government-sworn filings
- [[Apollo Fuel 2023 2025]] — EFS fuel card data
- Bank Recs: [[Apollo Bank Rec Jan 2024]] through [[Apollo Bank Rec DEC 2024]]
- Trial Balances: [[Apollo ADJ Trail Balance 2024]] | [[Apollo ADJ Trial Balance 2023]] | [[Apollo ADJ Trial Balance 2025-QB]]
- See [[Source Registry]] for full catalog
