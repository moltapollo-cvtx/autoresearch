---
type: finding
status: documented
confidence: critical
tags: [finding, critical]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Fuel Cost Manipulation]]"
  - "[[GL Audit Trail Anomalies]]"
  - "[[Forensic Cross-Reference Report]]"
evidence-refs:
  - "[[Bank Rec Analysis 2025]]"
  - "[[Apollo_2010_2025_Detail]]"
  - "[[Apollo_2010_Monthly_Rollforward]]"
dollar-amount: 527073
estimated_impact: "$285,789 fuel expense inflation + $241,284 unexplained cash reduction"
direction: apollo-inflated
documented_date: 2026-03-24
---

# Account 2010 — Fuel Payable Clearing Mechanism

## SMOKING GUN — This is How the Fuel Overstatement Works in 2025

### Summary
Account 2010 ("Fuel Payable") accumulated **$322,639.29** throughout all of 2024, growing every single month. On **March 31, 2025**, this balance was zeroed out via two manual journal entries — one dumping **$285,789.46 into Fuel Expense** (inflating the 2025 P&L) and the other reducing Cash by **$241,284.09** (the previously unexplained "ADJ TO STMT").

Both entries were posted to GL on **June 18-23, 2025** — nearly **3 months after** the stated transaction date. This is textbook backdated record manipulation.

---

## The Account 2010 Accumulation (2024)

Source: [[Apollo_2010_Monthly_Rollforward]]

| Month | Balance | Monthly Growth |
|-------|---------|---------------|
| Jan 2024 | $147,771.84 | $147,771.84 |
| Feb 2024 | $165,893.92 | $18,122.08 |
| Mar 2024 | $194,861.04 | $28,967.12 |
| Apr 2024 | $208,223.92 | $13,362.88 |
| May 2024 | $222,350.24 | $14,126.32 |
| Jun 2024 | $239,183.69 | $16,833.45 |
| Jul 2024 | $263,255.17 | $24,071.48 |
| Aug 2024 | $279,180.10 | $15,924.93 |
| Sep 2024 | $292,082.45 | $12,902.35 |
| Oct 2024 | $302,779.49 | $10,697.04 |
| Nov 2024 | $312,873.61 | $10,094.12 |
| **Dec 2024** | **$322,639.29** | $9,765.68 |

Account 2010 grew **every single month** of 2024 without being cleared. This is not normal accounting — payables should be settled periodically.

---

## The March 31, 2025 Clearing Entries

Source: [[Apollo_Manual_Journal_Fuel_Targets]]

### Entry 1: ADJ TO STMT (Transaction 03000015)
- **Transaction date:** 2025-03-31
- **Posted to GL:** 2025-06-18 (79-day lag!)
- **Memo:** "ADJ TO STMT"

| GL Account | Description | Amount |
|-----------|-------------|--------|
| 2000-00-00 | Accounts Payable | -$3,311.38 |
| 1100-00-00 | Accounts Receivable | **+$282,426.08** |
| 1000-00-00 | Cash | **-$241,284.09** |
| 2010-00-00 | Fuel Payable | -$37,830.61 |
| | **Net** | **$0.00** |

**RED FLAGS:**
- Why does clearing Fuel Payable require reducing CASH by $241K? If fuel was already paid via EFS bank draws, this is double-counting.
- Why does clearing Fuel Payable increase AR by $282K? Creating a receivable from nothing.
- This is the previously unexplained "$241,284 ADJ TO STMT" finding from [[Bank Rec Analysis 2025]].

### Entry 2: Fuel Expense Leg (Transactions 03000017/03000018)
- **Transaction date:** 2025-03-31
- **Posted to GL:** 2025-06-23 (84-day lag!)
- **Memo:** "ADJ TO BALANCE"

| GL Account | Description | Amount |
|-----------|-------------|--------|
| 2040-00-00 | Clearing Account | -$285,789.46 / +$285,789.46 |
| 5500-00-00 | **Fuel Expense** | **+$285,789.46** |
| 2010-00-00 | Fuel Payable | -$285,789.46 |

**This single journal entry added $285,789.46 to Apollo's 2025 fuel expense.** The entire amount was routed through a clearing account (2040) with the vague memo "ADJ TO BALANCE."

### Total Account 2010 Cleared
- Via ADJ TO STMT: $37,830.61
- Via Fuel Expense: $285,789.46
- **Total:** $323,620.07 (= Feb 2025 ending balance of $322,639.29 + $980.78 Feb activity)

---

## Additional Fuel Journal Entries (2025)

Source: [[Apollo_Manual_Journal_Fuel_Targets]]

### April 2025 entries (posted 2025-06-18 and 2025-06-23)
- Transaction 04000031: $1,820.26 reclassed from 2010 → 5500 Fuel
- Transaction 04000031: $559.98 reclassed from 2011 → 5100-01-00 (Owner Operator Pay)

### July 2025 entry (posted 2025-08-20)
- Transaction 07000029: $4,359.23 reclassed from 2010 → 5500 Fuel
- Transaction 07000031: **-$4,833.83** REDUCED fuel (2090 Escrow → 5500), labeled "ADJ ESCROW TO STMTS"

### August 2025 entry (posted 2025-08-20)
- Transaction 08000006: **-$1,217.45** REDUCED fuel (2020 → 5500), labeled "ADJ TO BAL"

---

## Impact Analysis

### 2025 Fuel Expense Decomposition
| Component | Amount | % of Total |
|-----------|--------|-----------|
| Normal EFS fuel operations | ~$506,492 | 54.6% |
| **Manual GJ from Account 2010** | **$285,789** | **30.8%** |
| Other fuel charges | ~$136,066 | 14.7% |
| **Total P&L Fuel (5500)** | **$700,425** | 100.0% |

### What Apollo Actually Paid for Fuel (2025)
| Source | Amount |
|--------|--------|
| EFS bank payments (verified) | $506,491.82 |
| P&L Fuel Expense (5500 accounts) | $700,424.65 |
| **Overstated by** | **$193,932.83 (38.3%)** |

Including Fuel Surcharge Pay (5310): $208,766.41 and DEF (5520): $19,378.55
- **Grand total fuel on P&L: $928,570**
- **Vs EFS actual: $506,492**
- **Grand overstatement: $422,078 (83.3%)**

### Compared to ATI's Own Numbers
| Entity | Revenue | Fuel Expense | Fuel % |
|--------|---------|-------------|--------|
| ATI | $37,102,495 | $1,134,795 | 3.1% |
| Apollo | $3,734,804 | $928,570 | 24.9% |
| **Apollo pays 8.1x more of its revenue on fuel than ATI** |

---

## Why This Matters

1. **The $285,789 journal entry is the 2025 equivalent of the 2023 "$234,683 fuel" entries.** Same mechanism: single lump-sum GJ entries labeled "fuel" that bypass the normal AP cycle.

2. **The backdating pattern repeats.** All entries are dated 3/31/2025 but posted 6/18-6/23/2025. The 2023 entries were also backdated months.

3. **The $241,284 "ADJ TO STMT" is now explained** — it was part of zeroing out account 2010, and it REDUCED Apollo's cash. Combined with the $285K fuel hit, this single day's entries cost Apollo **$527,073**.

4. **Account 2010 accumulated for ALL of 2024 without being cleared.** This suggests deliberate timing — build up the balance, then dump it when convenient.

---

## Connected
- [[Fuel Cost Manipulation]] — This IS the 2025 fuel manipulation mechanism
- [[Bank Rec Analysis 2025]] — The $241,284 ADJ TO STMT explained
- [[GL Audit Trail Anomalies]] — Same backdating pattern
- [[Rosanna Karim]] — Sole authorizer of financial entries
- [[Master Timeline]] — Add: 3/31/2025 (posted 6/18) clearing events

## Source Files
- [[Apollo_Manual_Journal_Fuel_Targets]] — The entries themselves
- [[Apollo_2010_Monthly_Rollforward]] — Monthly accumulation proof
- [[Apollo_2010_2025_Detail]] — Transaction-level detail
- [[Apollo QuickBooks LOGS 2022-2026]] — QB confirmation
- [[Source Registry]] | [[Data Lineage]]
