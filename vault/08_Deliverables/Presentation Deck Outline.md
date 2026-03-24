---
type: deliverable
status: draft
tags: [deliverable]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Master Narrative]]"
  - "[[Grandparent Meeting Prep]]"
  - "[[Evidence Strength Matrix]]"
  - "[[Executive Summary - ATI Financial Misconduct]]"
---

# Presentation Deck Outline — Apollo Energy Investigation

> 12-slide deck for meeting with grandparent company or attorneys. Each slide includes title, talking points, and suggested exhibit.

---

## Slide 1 — Title

**Apollo Energy Resources LLC — Financial Review Findings**

- Prepared by: Internal Investigation Team
- Date: 2026-03-24
- Status: Preliminary
- Confidential — For authorized recipients only

*Exhibit: None (cover slide)*

---

## Slide 2 — Apollo in Context

**What is Apollo Energy Resources?**

- Trucking subsidiary of ATI, owned by Walker Anderson
- ATI has exclusive control of Apollo's bank accounts, QuickBooks, journal entries, asset titles, and financial reporting
- Apollo's owner has no independent access to financial systems
- Apollo generates $3.7M in annual revenue (2025)
- Investigation initiated March 2026 after owner obtained bank recs and QB logs

*Exhibit: Organizational chart showing ATI → Apollo control relationship*

---

## Slide 3 — The Core Problem

**Every Financial Anomaly Moves Money the Same Direction**

- 10+ independent findings identified — all favor ATI, none favor Apollo
- Three independent data sources confirm: bank statements, EFS fuel card records, government IFTA filings
- ATI-prepared books tell one story; independent sources tell another
- No audit trail enabled on accounting system — a deliberate absence

*Exhibit: One-slide directional summary arrow diagram (Apollo → ATI on every line)*

---

## Slide 4 — Finding #1: Cash Extraction ($915,887)

**$1.2M Out, $286K Back — Net: $916K Extracted Over 2 Years**

- 2024: $335,566 extracted, $0 returned
- 2025: $866,092 extracted, $285,771 returned (net $580K)
- October 2025 alone: $355,000 (48% of that month's inflows)
- Only documented basis: an $858K promissory note proven backdated 174 days
- Every transfer verified penny-for-penny against independent bank statements

*Exhibit: [[Intercompany Transfer Tracker]] — two-year transfer table with running balance*

---

## Slide 5 — Finding #2: Fuel Cost Inflation (83.3%)

**Apollo's Books Say $929K in Fuel — Apollo Actually Paid $506K**

- EFS fuel card payments (bank-verified): $506,492
- ATI-prepared P&L total fuel: $928,570
- Overstatement: $422,078 (83.3%)
- ATI's own fleet: fuel = 3.1% of revenue; Apollo's P&L: 24.9%
- IFTA (government-sworn) confirms Apollo pays LESS per gallon than ATI at the pump
- The overcharge is entirely in the accounting, not at the pump

*Exhibit: [[Forensic Cross-Reference Report]] — three-column comparison (EFS actual / P&L reported / gap)*

---

## Slide 6 — Finding #3: The Mechanism (Account 2010)

**How the Fuel Inflation Works — Step by Step**

- Account 2010 "Fuel Payable" accumulated $322,639 through all of 2024
- Never cleared — grew every month for 12 consecutive months
- On March 31, 2025: two manual entries zeroed the account
- Entry 1: $285,789 dumped into Fuel Expense (inflating P&L)
- Entry 2: $241,284 deducted from Cash (the previously unexplained "ADJ TO STMT")
- Both entries posted 79–84 days after stated date (backdated)

*Exhibit: [[Account 2010 Fuel Payable Mechanism]] — monthly accumulation chart + entry screenshots*

---

## Slide 7 — Finding #4: Backdated Promissory Note ($858K)

**$858,000 in Debt Created 174 Days After Its Supposed Date**

- QuickBooks batch timestamps prove the entry was created ~6 months after the note's purported date
- No executed copy of the note has been produced
- This single document = 41% of Apollo's total intercompany debt
- Wire Payable ($870K) disappeared from balance sheet at the same time — likely relabeled, not new debt
- If the note is fabricated, the $1.2M in "paydowns" has no documented basis

*Exhibit: [[Promissory Note Backdating]] — timestamp comparison (purported date vs system entry date)*

---

## Slide 8 — Finding #5: Gemini Profit Siphon ($341K)

**Gemini Earned $128K — Apollo Got Nothing; Apollo's "Debt" to Gemini Grew $213K**

- Gemini Logistics: ATI-related entity operating through Apollo
- 24-month net income: $127,964
- Zero distributed to Apollo
- Apollo's recorded debt to Gemini grew by $212,945 (more than Gemini earned)
- NP Gemini balance: $924,186 by Dec 2025
- 23 Gemini records mass-deleted by a single user in ~25 minutes

*Exhibit: [[Gemini Profit Siphon]] — NR Apollo growth chart vs Gemini net income*

---

## Slide 9 — Total Exposure Summary

**Aggregate Documented Amounts**

- Net cash extracted: **$915,887** (bank-verified)
- Fuel overstatement (2025): **$422,078** (triple-verified)
- Fuel journal entries (2023): **$234,683** (QB logs + ATI GL)
- Promissory note (backdated): **$858,000** (QB timestamps)
- Gemini trapped profits + phantom debt: **$340,909** (cross-entity P&L)
- Total intercompany debt on Apollo's books: **$2,089,420**
- Apollo retained earnings: **($1,182,612)** — technically insolvent
- These categories interconnect; see [[Master Financial Reconciliation]] for double-counting analysis

*Exhibit: [[Master Financial Reconciliation]] — reconciliation table*

---

## Slide 10 — What We Still Need

**Critical Outstanding Documents**

- EFS portal exports (raw transaction data — the single most important missing document)
- Executed copy of the $858K promissory note
- Full-year ATI-prepared financials for Apollo (only partial provided)
- Henry Collins termination date (unlocks fuel card fraud quantification)
- Intercompany billing agreement (if one exists)
- $84,960 "Ins/Elog" itemized breakdown
- Gemini LLC corporate filings (establishes ATI relationship)

*Exhibit: [[Outstanding Document Demands]] — priority-ranked document list*

---

## Slide 11 — Evidence Quality

**What Makes These Findings Reliable**

- Bank statements: Independent (Stellar Bank) — ATI cannot alter
- EFS fuel cards: Third-party vendor — ATI cannot alter
- IFTA filings: Government-sworn — highest reliability
- QB transaction logs: SHA-256 preserved (hash: `d918f3c9...ef9a0a82`)
- Bulletproof findings: Net cash extraction, Account 2010 mechanism, fuel overstatement
- Strong findings: Gemini siphon, record deletion, GL anomalies
- Every claim traces to at least one source outside ATI's control

*Exhibit: [[Evidence Strength Matrix]] — finding-by-finding strength assessment*

---

## Slide 12 — Recommended Next Steps

**What We're Asking For**

1. **Immediate:** Grant Walker direct access to Apollo's bank account and QuickBooks
2. **Within 14 days:** Formal document demand to ATI (template prepared)
3. **Within 30 days:** Engage independent forensic accountant to verify findings
4. **Within 30 days:** Enable audit trail on accounting system
5. **Within 60 days:** Restructure financial controls (segregation of duties)
6. **If confirmed:** Reimburse Apollo for documented overcharges and unauthorized extractions
7. **Investment:** Provide capital injection for Apollo to operate independently

*Exhibit: [[Document Demand Letter Template]] — ready to send on counsel's letterhead*

---

## Appendix Materials (Bring to Meeting)

| Item | Source | Format |
|------|--------|--------|
| Full investigation vault | This Obsidian vault | Laptop (live navigation) |
| Two-year transfer table | [[Intercompany Transfer Tracker]] | Printed, 2 pages |
| Fuel cost comparison | [[Forensic Cross-Reference Report]] | Printed, 1 page |
| Account 2010 monthly chart | [[Account 2010 Fuel Payable Mechanism]] | Printed, 1 page |
| Evidence strength matrix | [[Evidence Strength Matrix]] | Printed, 1 page |
| Document demand letter | [[Document Demand Letter Template]] | Printed, ready to sign |
| Executive summary | [[Executive Summary - ATI Financial Misconduct]] | Printed, 1 page |

---

## Connected
- [[Grandparent Meeting Prep]] — Full meeting strategy (opening statement, Q&A, red lines)
- [[Master Narrative]] — The complete story
- [[Evidence Strength Matrix]] — What's bulletproof vs needs work
- [[Executive Summary - ATI Financial Misconduct]] — Attorney-ready one-pager
- [[Master Financial Reconciliation]] — Dollar figure reconciliation with double-counting analysis
