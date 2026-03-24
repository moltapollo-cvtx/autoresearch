---
type: finding
status: documented
confidence: critical
tags: [finding, critical, synthesis]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Account 2010 Fuel Payable Mechanism]]"
  - "[[Fuel Cost Manipulation]]"
  - "[[Forensic Cross-Reference Report]]"
  - "[[Henry Collins]]"
  - "[[EFS LLC]]"
  - "[[Asphalt Transport Inc (ATI)]]"
evidence-refs:
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo_2010_Monthly_Rollforward]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[Apollo Fuel 2023 2025]]"
  - "[[Apollo IFTA Filing 2024]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[Forensic Cross-Reference Report]]"
dollar-amount: 656761
---

# SYNTHESIS: Fuel Fraud — The Complete Picture

> **This note unifies all three fuel fraud mechanisms** into a single narrative showing how ATI systematically inflated Apollo's fuel costs across multiple years using different but interconnected techniques. Combined exposure: **$656,761+ documented, with additional unquantified card-level fraud.**

---

## The Three Mechanisms

### Mechanism 1: Account 2010 Fuel Payable Dump ($285,789)

**What happened:** Throughout all of 2024, GL account 2010 ("Fuel Payable") accumulated $322,639 — growing every single month without being cleared. On **March 31, 2025**, two manual journal entries zeroed the account:

- **Entry 1 (ADJ TO STMT):** Reduced Cash by **$241,284**, increased AR by $282,426, reduced Fuel Payable by $37,831. Posted to GL on **2025-06-18** (79-day lag).
- **Entry 2 (Fuel dump):** Moved **$285,789** from Fuel Payable through a clearing account (2040) into Fuel Expense (5500). Posted to GL on **2025-06-23** (84-day lag).

**Combined single-day impact: $527,073** ($285,789 fuel inflation + $241,284 cash reduction).

**Why it's fraud, not accounting:**
- Payables should be settled periodically, not accumulated for 12 months then dumped
- Both entries backdated 79-84 days (Q1 dates, posted in Q2 after books were "closed")
- The $285,789 has no corresponding EFS fuel transaction — no cash actually moved for fuel
- The vague memos ("ADJ TO BALANCE", "ADJ TO STMT") are designed to evade scrutiny

Source: [[Account 2010 Fuel Payable Mechanism]], [[Apollo_Manual_Journal_Fuel_Targets]], [[Apollo_2010_Monthly_Rollforward]]

### Account 2010 Monthly Accumulation (2024)

| Month | Running Balance | Monthly Growth |
|-------|----------------|---------------|
| Jan | $147,772 | $147,772 |
| Feb | $165,894 | $18,122 |
| Mar | $194,861 | $28,967 |
| Apr | $208,224 | $13,363 |
| May | $222,350 | $14,126 |
| Jun | $239,184 | $16,833 |
| Jul | $263,255 | $24,071 |
| Aug | $279,180 | $15,925 |
| Sep | $292,082 | $12,902 |
| Oct | $302,779 | $10,697 |
| Nov | $312,874 | $10,094 |
| **Dec** | **$322,639** | $9,766 |

Source: [[Apollo_2010_Monthly_Rollforward]]

---

### Mechanism 2: EFS/IFTA vs P&L Gap ($287K in 2023, $422K in 2025)

**What happened:** Apollo's ATI-prepared P&L reports dramatically higher fuel costs than what independent third-party records show Apollo actually paid.

#### 2025 Gap

| Source | Amount | Independence |
|--------|--------|-------------|
| EFS bank payments (actual cash to fuel vendor) | **$506,492** | Bank-verified (Stellar Bank) |
| P&L Fuel (5500 accounts only) | $700,425 | ATI-prepared |
| P&L Grand Total Fuel (5500 + 5310 + 5520) | **$928,570** | ATI-prepared |
| **5500 Overstatement** | **$193,933 (38.3%)** | |
| **Grand Total Overstatement** | **$422,078 (83.3%)** | |

Source: [[Forensic Cross-Reference Report]], [[Apollo 2025 December]], [[Bank Rec Analysis 2025]]

#### 2023 Gap

Six manual journal entries totaling **$234,683** debited "Fuel Expense - Company" and credited "NP ATI" — simultaneously inflating Apollo's fuel cost AND increasing Apollo's recorded debt to ATI. All entries used single-word memo "fuel" with no supporting invoices or EFS references.

| Trans# | Date | Entered | By | Amount | Lag |
|--------|------|---------|-----|--------|-----|
| 258 | 2023-04-28 | 2023-09-18 | Rosanna | $25,521 | 143d |
| 272 | 2023-05-10 | 2023-09-19 | Admin | $44,452 | 132d |
| 273 | 2023-06-13 | 2023-09-19 | Admin | $39,757 | 98d |
| 274 | 2023-07-13 | 2023-09-19 | Admin | $62,382 | 68d |
| 286 | 2023-08-16 | 2023-09-22 | Rosanna | $36,119 | 37d |
| **1169** | **2023-09-20** | **2025-01-08** | **Cordee** | **$26,452** | **476d** |
| **Total** | | | | **$234,683** | |

Source: [[DOC-QB-LOGS-2022-2026]], [[Fuel Cost Manipulation]]

#### ATI Comparison (2025)

| Entity | Revenue | Fuel on P&L | Fuel % of Revenue |
|--------|---------|-------------|-------------------|
| ATI | $37,102,495 | $1,134,795 | **3.1%** |
| Apollo (P&L) | $3,734,804 | $928,570 | **24.9%** |
| Apollo (actual EFS) | $3,734,804 | $506,492 | **13.6%** |

Apollo's P&L fuel burden is **8.1x ATI's** as a percentage of revenue. Even the actual EFS payments (13.6%) are 4.4x ATI's rate.

Source: [[ATI 2025 Profit & Loss MoM]], [[Forensic Cross-Reference Report]]

#### IFTA Government Filing Confirmation

Apollo's government-sworn IFTA filing (2024): **170,954 gallons at $537,061** ($3.14/gal).
ATI's IFTA filing (2024): 1,309,965 gallons at $4,278,193 ($3.27/gal).

Apollo pays **less per gallon** than ATI at the pump. The overcharge is entirely in the ACCOUNTING — via manual journal entries that bypass the normal fuel payment cycle.

Source: [[Apollo IFTA Filing 2024]], [[ATI IFTA 2024]]

---

### Mechanism 3: Card *0048 — Henry Collins Anomalies

**What happened:** Fuel card *0048, assigned to terminated driver [[Henry Collins]], shows the highest spend of all 10 masked fuel cards in Apollo's fleet. The critical evidentiary threshold is Collins' termination date — every dollar charged after his departure is direct fraud.

**Current status:** Termination date unknown. Full EFS transaction history for *0048 not yet obtained.

**Potential exposure:** Unquantified until termination date and card-level transaction data are secured. If *0048 was used for months or years after Collins' departure, the fraud could be substantial.

**Priority actions:**
1. Obtain Henry Collins' exact termination date from Walker or HR records
2. Pull EFS transaction report for card *0048 (Carrier ID 5725124)
3. Filter all transactions after termination date
4. Identify who had physical possession of the card

Source: [[Card 0048 - Henry Collins]], [[Fuel Card Overview]], [[Henry Collins]]

---

## How the Three Mechanisms Interconnect

```
MECHANISM 2 (Journal Entries)         MECHANISM 1 (Account 2010)
Creates fake fuel costs on P&L ←───── Accumulates payable, then dumps
   2023: $234,683                        2024: $322,639 accumulated
   2025: additional GJ entries           2025: $285,789 dumped to fuel
         │                                      │
         ▼                                      ▼
   APOLLO'S P&L SHOWS 83.3%          APOLLO'S CASH REDUCED $241K
   MORE FUEL THAN ACTUALLY PAID       (the "ADJ TO STMT" explained)
         │                                      │
         └──────────────┬───────────────────────┘
                        ▼
              INFLATED EXPENSES MAKE
              APOLLO APPEAR UNPROFITABLE
                        │
                        ▼
              JUSTIFIES "PAYDOWNS" TO ATI
              ($1.2M gross over 2 years)
                        │
         ┌──────────────┴───────────────────────┐
         ▼                                      ▼
   NP ATI grows on books              MECHANISM 3 (Card Fraud)
   "Proving" Apollo owes ATI           Physical fuel cards may be
   more than it actually does          used after driver departure
                                       → direct cash theft at pump
```

---

## Combined Exposure Timeline

| Year | Mechanism | Amount | Status |
|------|-----------|--------|--------|
| **2023** | 6 fuel GJ entries to NP ATI | $234,683 | PROVEN |
| **2024** | Account 2010 accumulation (building for 2025 dump) | $322,639 (deferred) | PROVEN |
| **2024** | P&L vs EFS gap (est.) | ~$13K | LOW (2024 P&L close to EFS) |
| **2025** | Account 2010 fuel dump | $285,789 | PROVEN |
| **2025** | ADJ TO STMT cash reduction | $241,284 | PROVEN |
| **2025** | P&L vs EFS overstatement (5500 only) | $193,933 | HIGH |
| **2025** | Grand total fuel overstatement (all accounts) | $422,078 | HIGH |
| **2023-2025** | Card *0048 post-termination | Unknown | PENDING |
| | | | |
| **TOTAL DOCUMENTED** | | **$656,761** | (GJ entries + Account 2010 dump, no double-counting) |
| **TOTAL INCLUDING P&L GAP** | | **$422,078** (2025 alone) | (alternative measure: actual vs reported) |

**Note on double-counting:** The $285,789 Account 2010 dump is a subset of the $422,078 P&L overstatement. The $234,683 in 2023 GJ entries are separate and additional. The non-overlapping total of documented fuel fraud is:
- 2023: $234,683 (GJ entries)
- 2025: $422,078 (P&L vs EFS grand total, which includes the $285,789 dump)
- **Combined: $656,761**

---

## Year-by-Year Evolution

### 2023: The Journal Entry Method
ATI posts six round-ish "fuel" entries directly to N/R Apollo account. No invoices, no EFS references, bypass AP cycle entirely. Entries backdated 37-476 days. Creates both expense inflation AND intercompany debt.

### 2024: The Accumulation Phase
Account 2010 begins collecting fuel payable — growing every month, never cleared. Meanwhile, $705,265 in actual EFS payments flow normally through the bank. The 2024 P&L is close to EFS actual because the Account 2010 balance is building on the balance sheet, not yet hitting the P&L.

### 2025: The Dump
Account 2010 is zeroed in a single day (March 31, 2025) via two backdated entries. The $285,789 hits Fuel Expense, the $241,284 hits Cash. Combined with ongoing fuel allocations, Apollo's 2025 P&L shows $928,570 in fuel — 83.3% more than the $506,492 actually paid.

### Pattern: Evolving Sophistication
- 2023: Simple journal entries labeled "fuel" (detectable by auditor)
- 2024-2025: Balance sheet accumulation → single-day dump (harder to detect in monthly reviews because the P&L impact is concentrated in one period)

---

## Connected
- [[Account 2010 Fuel Payable Mechanism]] — Mechanism 1 detail
- [[Fuel Cost Manipulation]] — Mechanism 2 detail (original finding)
- [[Forensic Cross-Reference Report]] — Penny-level cross-reference
- [[Henry Collins]] — Card *0048 driver
- [[EFS LLC]] — Independent fuel data source
- [[Asphalt Transport Inc (ATI)]] — Controlling entity
- [[Fuel Spend Reconciliation]] — Bank-level EFS reconciliation
- [[Bridge - GL Manipulation to Bank Evidence]] — How GL manipulation connects to bank evidence
- [[Master Narrative]] — Where this fits in the overall case
- [[Evidence Strength Matrix]] — Admissibility assessment for fuel findings
