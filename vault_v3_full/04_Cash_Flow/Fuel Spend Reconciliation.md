---
tags: [cash-flow, finding]
updated: 2026-03-23
---

# Fuel Spend Reconciliation

## Three-Source Comparison (Original Finding)

| Source | Type | Amount | Gallons | Can ATI Alter? |
|---|---|---|---|---|
| Apollo IFTA Filing | Government-sworn | ~$433K | ~145K | No |
| EFS Card Records | Third-party | Corroborates IFTA | Corroborates IFTA | No |
| ATI-Prepared P&L | Internal | ~$720K | N/A | Yes (no audit trail) |
| **Discrepancy** | | **~$287K** | | |

## ATI's Own Fuel Discrepancy

| Source | ATI Fuel Cost |
|---|---|
| ATI IFTA Filing | Understated by ~$2M |
| ATI Internal Books | Higher than IFTA |

**Both discrepancies move in the same direction:** Apollo pays more than it should on paper, ATI pays less.

---

## NEW: Bank-Level EFS Payments (Added 03/23/2026)

Actual cash paid to EFS LLC from Apollo's Stellar Bank account — independently verifiable via bank statements.

### 2024 EFS Payments (Full Year)

| Month | Amount |
|---|---|
| Jan 2024 | -$78,445.66 |
| Feb 2024 | -$52,573.37 |
| Mar 2024 | -$81,120.49 |
| Apr 2024 | -$50,523.16 |
| May 2024 | -$59,153.31 |
| Jun 2024 | -$57,924.38 |
| Jul 2024 | -$69,688.68 |
| Aug 2024 | -$74,414.31 |
| Sep 2024 | -$53,807.60 |
| Oct 2024 | -$51,178.33 |
| Nov 2024 | -$46,105.81 |
| Dec 2024 | -$30,330.18 |
| **2024 TOTAL** | **-$705,265.28** |

### 2025 EFS Payments (Mar–Dec)

| Month | Amount |
|---|---|
| Mar 2025 | -$35,890.90 |
| Apr 2025 | -$33,354.26 |
| May 2025 | -$38,045.84 |
| Jun 2025 | -$54,578.12 |
| Jul 2025 | -$60,295.85 |
| Aug 2025 | -$71,078.01 |
| Sep 2025 | -$62,538.87 |
| Oct 2025 | -$65,552.52 |
| Nov 2025 | -$41,392.27 |
| Dec 2025 | -$43,765.18 |
| **2025 TOTAL** | **-$506,491.82** |

### Two-Year EFS Total: **$1,211,757.10**

---

## Reconciliation Status

| Data Point | 2024 | 2025 |
|---|---|---|
| EFS at bank (verified) | $705,265 | $506,492 |
| ATI-prepared P&L fuel line | ~$720K (est.) | **NOT PROVIDED** |
| IFTA fuel cost | ~$433K (partial period) | Not yet filed? |
| Fuel journal entries via NP ATI (2023 GL) | $234,683 (2023) | TBD |

**CRITICAL GAP:** The 2025 ATI-prepared P&L has not been provided. Without it, we cannot calculate the 2025 fuel overstatement. **Demand immediately.**

---

## Where Could the Overstatement Be?

The mechanism has been confirmed via QB Transaction Logs ([[DOC-QB-LOGS-2022-2026]]):

1. ATI posts journal entries labeled "fuel" to NP ATI account — no invoices, no EFS reference
2. These entries simultaneously inflate Apollo's fuel expense AND increase Apollo's recorded debt to ATI
3. ATI then collects on this inflated "debt" via the "paydowns" tracked in [[Intercompany Transfer Tracker]]

**It's a two-step extraction:** First fabricate the expense (creating a fake receivable), then collect on it.

---

## What We Need
- [x] Bank-level EFS payment data for 2024 — **OBTAINED 03/23/2026**
- [x] Bank-level EFS payment data for 2025 — **OBTAINED 03/23/2026**
- [ ] 2025 ATI-prepared P&L fuel line detail — **DEMAND IMMEDIATELY**
- [ ] Unaltered EFS portal exports → card-level transaction detail
- [ ] Volume discount agreements → rule out legitimate explanations
- [ ] Stellar Bank raw statements → independent verification

## Connected Findings
- [[Fuel Cost Manipulation]] — The $287K gap finding
- [[Bank Rec Analysis 2024]] — Full 2024 bank data
- [[Bank Rec Analysis 2025]] — Full 2025 bank data
- [[Intercompany Transfer Tracker]] — The collection mechanism
- [[Fuel Card Overview]] — Card-level investigation
