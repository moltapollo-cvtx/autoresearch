---
tags: [entity, person]
role: Team member
organization: "[[Apollo Energy Resources LLC]]"
risk_level: medium-high
---

# Cordee

## Role & Access
- **Organization:** [[Apollo Energy Resources LLC]]
- **System access:** Appears in accounting system audit trail

## QB Log Statistics (from [[DOC-QB-LOGS-2022-2026]])
- **Total entries:** 11,698 (43.3% of all transactions — most active user)
- **General Journal entries:** 760
- **Backdating >30 days:** 1,417 entries (12.1%)
- **Max backdating lag:** **476 days** (Entry #1169, the most extreme in the dataset)

## Known Actions

| Event | Evidence |
|---|---|
| Mass-deleted 23 Gemini-related records in ~25 minutes | [[Gemini Record Manipulation]] |
| 476-day backdated entry: $26,452 "co driver fuel" (Trans #1169) | [[GL Audit Trail Anomalies]], [[Fuel Cost Manipulation]] |
| Entry #1169: Tx date 09/20/2023, entered 01/08/2025 14:33 | [[DOC-QB-LOGS-2022-2026]] |

## Relevance to Investigation
Two critical actions: (1) Mass deletion of Gemini records — overt evidence destruction. (2) The most extreme backdated entry in the dataset (476 days) — a "co driver fuel" entry that simultaneously inflates Apollo's fuel cost and increases Apollo's debt to ATI. Whether Cordee acted independently or at direction from ATI personnel (e.g., [[Rosanna Karim]] or [[Jimmy]]) is a key question.

## Connected Findings
- [[Gemini Record Manipulation]] — 23 records mass-deleted
- [[GL Audit Trail Anomalies]] — 476-day backdated entry
- [[Fuel Cost Manipulation]] — Entry #1169 is part of the fuel GJ mechanism

## Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — Activity documented (SHA: `d918f3c9...ef9a0a82`)
