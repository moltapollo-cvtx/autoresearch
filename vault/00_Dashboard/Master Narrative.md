---
type: dashboard
tags: [dashboard, synthesis]
created: 2026-03-24
updated: 2026-03-24
---

# Master Narrative — Apollo Energy Resources Investigation

> **Read this note first.** It is the single-page summary of the entire forensic investigation into how ATI has been extracting cash from Apollo Energy Resources while inflating Apollo's recorded expenses and debts.

---

## Core Thesis

**Asphalt Transport Inc (ATI) has exclusive, unaudited control over Apollo Energy Resources LLC's finances — bank accounts, journal entries, asset titles, and financial reporting.** ATI has used this control to systematically inflate Apollo's recorded expenses (primarily fuel), fabricate intercompany debts, and extract over $900,000 in cash from Apollo's bank account over two years. Every anomaly moves money in the same direction: Apollo loses, ATI gains.

---

## The 5 Most Critical Proven Findings

> [!SMOKING-GUN] 1. Net Cash Extraction: $915,887
> ATI extracted **$1,201,658 gross** from Apollo's [[Stellar Bank]] account over 2024-2025, returning only $285,771 — a **net drain of $915,887**. Verified penny-for-penny against independent bank statements. Source: [[Intercompany Transfer Tracker]], [[Bank Rec Analysis 2024]], [[Bank Rec Analysis 2025]]

> [!SMOKING-GUN] 2. Account 2010 Fuel Payable Dump: $527,073
> ATI allowed $322,639 to accumulate in a fuel payable account throughout 2024, then zeroed it on 2025-03-31 via two backdated manual journal entries: **$285,789 dumped into Fuel Expense** (inflating Apollo's P&L) and **$241,284 deducted from Cash** (the previously unexplained "ADJ TO STMT"). Both entries were posted 79-84 days after their stated date. Source: [[Account 2010 Fuel Payable Mechanism]], [[Apollo_Manual_Journal_Fuel_Targets]]

> [!SMOKING-GUN] 3. Fuel Expense Overstatement: 83.3% ($422,078)
> Apollo's 2025 P&L shows **$928,570** in total fuel costs. Independent EFS fuel card records and bank payments show Apollo actually paid **$506,492**. The difference — **$422,078 (83.3%)** — exists entirely in manual journal entries with no supporting invoices. ATI's own fleet pays 3.1% of revenue on fuel; Apollo's P&L shows 24.9%. Source: [[Forensic Cross-Reference Report]], [[Apollo Fuel 2023 2025]], [[Bank Rec Analysis 2025]]

> [!CRITICAL] 4. $858,000 Promissory Note Backdated 174 Days
> A promissory note creating $858,000 in debt on Apollo's books was proven backdated by **174 days** via QuickBooks batch timestamp analysis. The note appeared on Apollo's balance sheet in 2025 despite no corresponding account activity in 2023-2024. Source: [[Promissory Note Backdating]], [[DOC-QB-LOGS-2022-2026]]

> [!CRITICAL] 5. Gemini Profit Siphon: $340,909
> [[Gemini Logistics USA LLC]] earned **$127,964 in net profit** over 24 months — none flowed to Apollo. Instead, Apollo's recorded debt to Gemini grew by **$212,945** (more than Gemini even earned), reaching $924,186 by Dec 2025. Gemini's retained earnings actually *decreased* despite positive income. Source: [[Gemini Profit Siphon]], [[ATI GL 2023 - Gemini N-R Analysis]]

---

## The Mechanism: How Money Moves

```
ATI CONTROLS APOLLO'S BOOKS (no audit trail, no independent access)
        │
        ├──► STEP 1: INFLATE EXPENSES
        │    Manual journal entries labeled "fuel" bypass normal AP cycle
        │    Account 2010 accumulates payable → dumps into Fuel Expense
        │    Apollo's P&L shows 83.3% more fuel cost than actually paid
        │
        ├──► STEP 2: FABRICATE DEBTS
        │    $858K promissory note backdated 174 days
        │    NP Gemini grows $213K (more than Gemini earned)
        │    NP ATI carries $535K
        │    Total intercompany debt: $2,089,420
        │
        └──► STEP 3: EXTRACT CASH
             "Paydowns" on fabricated debts: $1.2M gross over 2 years
             October 2025 alone: $355,000 (48% of that month's inflows)
             Net extracted: $915,887
```

---

## Every Actor and Their Role

### ATI Side (Controllers)
| Person | Role | Key Actions |
|--------|------|-------------|
| [[Jimmy]] | ATI President | Executive authority over all ATI operations; strong ego, will deny |
| [[Rosanna Karim]] | Controller/VP Finance | **Sole bank authorizer**; 47.5% of all GJ entries; batch-entered all Gemini liabilities ($282K); 39.4% of her entries backdated >30 days |
| [[Cordee]] | QB Power User | Most active user (43.3% of entries); mass-deleted 23 Gemini records in ~25 min; 476-day backdated entry |
| [[James Luhr Jr]] | Signatory | Signed the $858K backdated promissory note |

### Apollo Side (Victim)
| Person | Role | Key Facts |
|--------|------|-----------|
| [[Walker]] | Apollo Owner | No access to own bank account; no QB access; initiated investigation |
| [[Cody]] | Team Member | Zero QB activity; no financial system access |

### Entities
| Entity | Role | Dollar Exposure |
|--------|------|----------------|
| [[Asphalt Transport Inc (ATI)]] | Parent company, sole controller | $915,887 net received from Apollo |
| [[Apollo Energy Resources LLC]] | Subsidiary, victim | $915,887 net extracted |
| [[Gemini Logistics USA LLC]] | Related entity, profit trap | $924,186 in phantom NP on Apollo's books |
| [[GIG Transportation Services]] | Suspected Gemini affiliate | $111,924 received from Apollo (2024) |
| [[EFS LLC]] | Independent fuel card provider | $1.2M in verified fuel payments (anchor evidence) |
| [[Stellar Bank]] | Apollo's bank | Independent verification source |

---

## Timeline Arc

### 2023 — Pattern Established
- Six "fuel" journal entries totaling $234,683 posted to inflate Apollo's costs (backdated 37-476 days)
- Gemini liabilities ($282,416) batch-created by [[Rosanna Karim]] in a single session
- $858K promissory note created (later proven backdated 174 days)
- 23 Gemini records mass-deleted by [[Cordee]]

### 2024 — The Drain Year
- Apollo's bank balance drained from **$364,745 → -$44,470** (Nov overdraft)
- ATI extracted **$335,566** from Apollo; returned **$0**
- Account 2010 quietly accumulated **$322,639** in fuel payable (never cleared)
- GIG Transportation received **$111,924** in biweekly payments (Jan-May)

### 2025 — The Escalation
- Account 2010 zeroed via backdated entries: **$285,789** to fuel + **$241,284** from cash
- ATI gross extraction: **$866,092** (up 158% from 2024)
- October 2025: **$355,000** extracted in a single month (48% of inflows)
- Apollo's total intercompany debt reached **$2,089,420**
- Apollo's retained earnings: **($1,182,612)** — technically insolvent

### 2026 — Investigation Begins
- Walker uploads QB logs and bank recs (March 23)
- Forensic analysis quantifies $915,887 net extraction
- Account 2010 mechanism fully documented
- This vault created as evidence presentation platform

---

## What We Still Need

The investigation has proven the mechanism and quantified the damage. Critical gaps remain:

> [!OPEN-QUESTION] Unresolved Questions
> See [[Open Questions]] for 17 tracked questions including:
> - What justifies $1.2M in "paydowns"? (no loan documentation produced)
> - Where did $868K in Wire Payable go? (disappeared from balance sheet)
> - What is the exact breakdown of the $84,960 "Ins/Elog" charge?
> - Is [[GIG Transportation Services]] a Gemini affiliate? (adds $112K to extraction)

> [!MISSING-EVIDENCE] Outstanding Document Demands
> See [[Outstanding Document Demands]] for the priority list:
> - **EFS portal exports** — the single most important missing document
> - **Full-year ATI financials** — only partial data provided despite requests
> - **Henry Collins termination date** — unlocks fuel card fraud quantification
> - **Intercompany billing agreement** — should document the basis for all charges

---

## Cumulative Damage to Apollo (Documented)

```dataview
TABLE dollar-amount AS "Dollar Impact", confidence AS "Confidence", status AS "Status"
FROM #finding
WHERE dollar-amount > 0
SORT dollar-amount DESC
```

| Finding | Amount | Confidence |
|---------|--------|-----------|
| [[Intercompany Transfer Tracker\|Net Cash Extraction]] | $915,887 | VERIFIED (bank) |
| [[Promissory Note Backdating\|Backdated Promissory Note]] | $858,000 | PROVEN (timestamps) |
| [[Account 2010 Fuel Payable Mechanism\|Account 2010 Combined]] | $527,073 | PROVEN (GL + bank) |
| [[Forensic Cross-Reference Report\|2025 Fuel Overstatement (grand)]] | $422,078 | HIGH (P&L vs EFS) |
| [[Gemini Profit Siphon\|Gemini Trapped Profits + Phantom Debt]] | $340,909 | CRITICAL (cross-entity) |
| [[Fuel Cost Manipulation\|2023 Fuel GJ Mechanism]] | $287,000 | HIGH (IFTA vs P&L) |
| [[Gemini Record Manipulation\|Gemini Batch Entries]] | $282,416 | HIGH (QB logs) |
| [[Revenue Timing Shift]] | $145,000 | MEDIUM-HIGH |
| [[GIG Transportation Services\|GIG Payments (unverified)]] | $111,924 | CONFIRMED (bank) |

---

## Navigation

- **Dashboards:** [[Investigation Dashboard]] · [[Cash Flow Dashboard]] · [[Document Registry]] · [[Master Timeline]]
- **Synthesis:** [[SYNTHESIS - Fuel Fraud Complete Picture]] · [[Cross-Entity Transaction Map]] · [[Evidence Strength Matrix]]
- **Strategy:** [[Evidence Tiers]] · [[Grandparent Meeting Prep]] · [[Open Questions]] · [[Outstanding Document Demands]]
- **Chain of Custody:** [[Source Registry]] · [[Data Lineage]] · [[Duplicate Tracker]]
- **Deliverables:** [[Deliverables Index]]
