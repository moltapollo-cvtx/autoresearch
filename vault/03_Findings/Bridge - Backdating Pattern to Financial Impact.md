---
type: finding
status: documented
confidence: high
tags: [finding, high, bridge]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[GL Audit Trail Anomalies]]"
  - "[[Promissory Note Backdating]]"
  - "[[Account 2010 Fuel Payable Mechanism]]"
  - "[[Fuel Cost Manipulation]]"
evidence-refs:
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo Quickbooks Audit Trail 2023 to dec 2024]]"
---

# Bridge: Backdating Pattern → Financial Impact Quantification

> This note connects the **systematic backdating pattern** (timestamps, user behavior, no audit trail) to the **quantified financial damage** (dollar amounts, expense inflation, cash extraction).

---

## The Pattern

Every major manipulation entry in the vault shares the same structural signature:

1. **Large round-ish dollar amounts** — not tied to specific invoices or transactions
2. **Backdated by weeks to months** — transaction date far before GL posting date
3. **Manual General Journal entries** — bypass normal AP/AR controls
4. **Concentration in 2-3 users** — [[Rosanna Karim]] (47.5% of all GJ entries) and [[Cordee]] (476-day extreme)
5. **Vague memos** — "fuel", "co driver fuel", "ADJ TO BALANCE", "ADJ TO STMT"

---

## Complete Backdating → Dollar Impact Map

| Entry | Recorded Date | Entered Date | Lag | Amount | Financial Impact | Source |
|-------|--------------|-------------|-----|--------|-----------------|--------|
| Fuel GJ #258 | 2023-04-28 | 2023-09-18 | 143d | $25,521 | Inflated Apollo fuel expense, increased NP ATI | [[DOC-QB-LOGS-2022-2026]] |
| Fuel GJ #272 | 2023-05-10 | 2023-09-19 | 132d | $44,452 | Inflated Apollo fuel expense, increased NP ATI | [[DOC-QB-LOGS-2022-2026]] |
| Fuel GJ #273 | 2023-06-13 | 2023-09-19 | 98d | $39,757 | Inflated Apollo fuel expense, increased NP ATI | [[DOC-QB-LOGS-2022-2026]] |
| Fuel GJ #274 | 2023-07-13 | 2023-09-19 | 68d | $62,382 | Inflated Apollo fuel expense, increased NP ATI | [[DOC-QB-LOGS-2022-2026]] |
| Fuel GJ #286 | 2023-08-16 | 2023-09-22 | 37d | $36,119 | Inflated Apollo fuel expense, increased NP ATI | [[DOC-QB-LOGS-2022-2026]] |
| **Fuel GJ #1169** | **2023-09-20** | **2025-01-08** | **476d** | **$26,452** | **Most extreme backdate in dataset** | [[GL Audit Trail Anomalies]] |
| Gemini NP #760-762 | 2023-07-31 to 2023-09-30 | 2023-11-02 | 33-94d | $282,416 | Created $282K Gemini liability on Apollo books | [[Gemini Record Manipulation]] |
| $858K Promissory | ~2024 | ~6 months later | **174d** | $858,000 | Created retroactive $858K debt on Apollo | [[Promissory Note Backdating]] |
| **ADJ TO STMT** | **2025-03-31** | **2025-06-18** | **79d** | **$241,284** | **Reduced Apollo cash by $241K** | [[Account 2010 Fuel Payable Mechanism]] |
| **Fuel dump** | **2025-03-31** | **2025-06-23** | **84d** | **$285,789** | **Inflated 2025 fuel expense by $286K** | [[Account 2010 Fuel Payable Mechanism]] |
| April reclass | 2025-04-16 | 2025-06-18 | 63d | $1,820 | Additional fuel inflation | [[Apollo_Manual_Journal_Fuel_Targets]] |
| July fuel adj | 2025-07-15 | 2025-08-20 | 36d | $4,359 | Additional fuel inflation | [[Apollo_Manual_Journal_Fuel_Targets]] |

### Total quantified from backdated entries: **$1,908,351**

---

## Why Backdating Proves Intent

Backdating is not a byproduct of sloppy bookkeeping. It serves a specific purpose:

1. **Fuel entries (2023):** Backdated to spread the inflation across multiple months → harder to spot in any single month's review
2. **Gemini batch entries:** Backdated to create the appearance of organic month-end accruals → disguises the retrospective construction
3. **$858K Promissory:** Backdated to make the note appear as if it predated the cash extractions → creates retroactive justification
4. **Account 2010 clearing (2025):** Backdated to Q1 but posted in Q2 → the manipulation occurred during a period when Q1 books were supposedly "closed"

**The no-audit-trail environment is critical.** Without audit trail enabled, there is no independent record of WHEN entries were truly created. The only evidence is the batch timestamp analysis from [[DOC-QB-LOGS-2022-2026]], which was preserved before it could be altered.

---

## The Escalation

| Year | Backdated Amount | Avg Lag | Trend |
|------|-----------------|---------|-------|
| 2023 | $234,683 (fuel) + $282,416 (Gemini) + $858,000 (note) = **$1,375,099** | 37-476 days | Established pattern |
| 2025 | $285,789 (fuel dump) + $241,284 (ADJ TO STMT) + $6,179 (other) = **$533,252** | 36-84 days | Tighter timing but larger amounts per entry |

The backdating is getting more efficient — fewer entries, larger amounts, shorter but still significant lags.

---

## Connected
- [[Forensic Cross-Reference Report]] — Cumulative damage table
- [[Rosanna Karim]] — 1,942 entries backdated >30 days (39.4% of her work)
- [[Cordee]] — 1,417 entries backdated >30 days, 476-day extreme
- [[Master Timeline]] — Chronological view with all backdated entries
- [[Open Questions]] — Q6: total value of 23 deleted Gemini records unknown
