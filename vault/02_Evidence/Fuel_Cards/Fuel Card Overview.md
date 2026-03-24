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
| *0040 | TBD | Medium | Active | |
| *0041 | TBD | High | Active | 3rd priority for transaction pull |
| *0042 | TBD | High | Active | 2nd priority — immediate pull needed |
| *0043 | TBD | Medium | Active | |
| *0044 | TBD | Medium | Active | |
| *0045 | TBD | Medium | Active | |
| *0046 | TBD | High | Active | 4th priority for transaction pull |
| *0047 | TBD | Medium | Active | |
| *0048 | [[Henry Collins]] | **Critical** | Terminated driver | Highest spend. Immediate pull needed. See [[Card 0048 - Henry Collins]] |
| *0049 | TBD | High | Active | 5th priority for transaction pull |

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
