---
type: evidence
tags: [evidence]
evidence_type: fuel-card
source: independent
status: documented
confidence: high
created: 2026-03-23
updated: 2026-03-24
related: ["[[Card 0048 - Henry Collins]]", "[[Fuel Cost Manipulation]]", "[[Other Flagged Users]]"]
---

# Fuel Card Overview
> 10 masked EFS fuel cards under Carrier ID 5725124 (Apollo)

## Card Inventory

| Card | Assigned Driver | Priority | Status | Notes |
|---|---|---|---|---|
| *0040 | Unidentified | Medium | Active | |
| *0041 | Unidentified | High | Active | 3rd priority for transaction pull |
| *0042 | Unidentified | High | Active | 2nd priority — immediate pull needed |
| *0043 | Unidentified | Medium | Active | |
| *0044 | Unidentified | Medium | Active | |
| *0045 | Unidentified | Medium | Active | |
| *0046 | Unidentified | High | Active | 4th priority for transaction pull |
| *0047 | Unidentified | Medium | Active | |
| *0048 | [[Henry Collins]] | **Critical** | Terminated driver | Highest spend. Immediate pull needed. See [[Card 0048 - Henry Collins]] |
| *0049 | Unidentified | High | Active | 5th priority for transaction pull |

> [!MISSING-EVIDENCE]
> **To identify drivers assigned to cards *0040–*0047 and *0049:** Requires EFS account management report for Carrier ID 5725124 (Apollo Energy Resources LLC) showing card-to-driver assignment history. Request from EFS LLC directly or from Apollo's EFS portal access. Without driver assignments, post-termination fraud analysis cannot be performed on 9 of 10 cards. Confidence remains **low** for all unidentified cards.

## Priority Order for Transaction Report Pulls
1. **Immediate:** *0048 and *0042
2. **Next:** *0041, *0046, *0049

## Parameters for Transaction Report Pulls
For each card, pull and analyze:
- [ ] Charges after driver termination date
- [ ] Cash advance transactions
- [ ] Activity on fraud-hold cards after hold date
- [ ] Periods of simultaneous dual-card holding

## Fraud-to-New-Card Pattern
Two drivers previously flagged for fraud on old cards were subsequently issued new active cards:
- **Alfredo Allen Wilson** — See [[Other Flagged Users]]
- **Jermaine Johnson** — See [[Other Flagged Users]]

## Connected Findings
- [[Fuel Cost Manipulation]]
- [[Card 0048 - Henry Collins]]
