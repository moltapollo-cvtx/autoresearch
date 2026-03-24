---
type: strategy
status: active
confidence: high
tags: [strategy]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[Grandparent Meeting Prep]]"
  - "[[Fuel Cost Manipulation]]"
  - "[[Promissory Note Backdating]]"
  - "[[Revenue Timing Shift]]"
  - "[[Gemini Record Manipulation]]"
evidence-refs: []
---

# Evidence Tiers — Grandparent Company Meeting

## Framework
Tiered presentation strategy. Frame findings as **misallocation and control failures** rather than direct accusations. The goal is investment capital as the top ask.

### Must Hit (Present no matter what)

| Item | Dollar Impact | Finding | Source Evidence |
|------|--------------|---------|-----------------|
| Fuel cost overstatement (~$287K gap with independent verification) | $287,000 (2024); $422,078 (2025) | [[Fuel Cost Manipulation]] | [[Apollo IFTA Filing 2024]], [[Apollo Fuel 2023 2025]], [[Forensic Cross-Reference Report]] |
| ATI's exclusive financial control with no audit trail | Systemic | [[GL Audit Trail Anomalies]] | [[DOC-QB-LOGS-2022-2026]] (no audit trail enabled) |
| Promissory note backdating (174 days, $858K) | $858,335 | [[Promissory Note Backdating]] | [[DOC-QB-LOGS-2022-2026]] (batch timestamp analysis) |
| Directional consistency of all anomalies | Systemic | [[Forensic Cross-Reference Report]] | All finding notes — every anomaly moves money Apollo→ATI |
| Fuel-to-NP-ATI journal entry mechanism confirmed BOTH sides | $234,683 (2023); $285,789 (2025) | [[Fuel Cost Manipulation]], [[Account 2010 Fuel Payable Mechanism]] | [[Apollo_Manual_Journal_Fuel_Targets]], [[ATI GeneralLedger Report 2023]] |
| October 2025 — $355K extracted (48% of monthly inflows) | $355,000 | [[Bank Rec Analysis 2025]] | [[Intercompany Transfer Tracker]], [[Bank Rec Analysis 2025]] |

### Ought to Hit (Present if time allows)

| Item | Dollar Impact | Finding | Source Evidence |
|------|--------------|---------|-----------------|
| Revenue timing shift (~$145K FY2024 understatement) | ~$145,000 | [[Revenue Timing Shift]] | [[APL GL work]], [[Apollo ADJ Trail Balance 2024]] |
| ATI monthly billing manipulation | Unquantified — requires ATI billing invoices | [[ATI Monthly Billing Manipulation]] | [[ATI GL 2023 - Intercompany Billing]], [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] |
| All 12 monthly statements batch-printed same date | Pattern evidence | [[Document Registry]] | [[Bank Rec Analysis 2025]] |
| Apollo bank paid $506K to EFS in 2025 vs P&L fuel $928K (83.3% overstatement) | $422,078 | [[Forensic Cross-Reference Report]] | [[Bank Rec Analysis 2025]], [[Apollo 2025 December]] |
| $84,960 bundled "Ins/Elog" charge with no supporting documentation | $84,960 | [[Bank Rec Analysis 2025]] | [[Bank Rec Analysis 2025]] (2025-11-30 entry) |

### Should Hit (Strong supporting evidence)

| Item | Dollar Impact | Finding | Source Evidence |
|------|--------------|---------|-----------------|
| GL retroactive entries (476-day backdating confirmed) | $26,452 (single entry); $1.9M total backdated | [[GL Audit Trail Anomalies]] | [[DOC-QB-LOGS-2022-2026]], [[Bridge - Backdating Pattern to Financial Impact]] |
| Gemini record manipulation (creation + deletion) | $282,416 (batch-created); deleted value requires QB backup | [[Gemini Record Manipulation]] | [[DOC-QB-LOGS-2022-2026]], [[ATI GL 2023 - Gemini N-R Analysis]] |
| Rosanna controls 47.5% of all GJ entries; 39.4% backdated >30 days | Systemic — she controls the manipulation mechanism | [[GL Audit Trail Anomalies]] | [[DOC-QB-LOGS-2022-2026]] (user activity summary) |
| Martha [Deleted User] — 3,030 entries from a deleted account | Pattern evidence — audit trail destruction | [[GL Audit Trail Anomalies]] | [[DOC-QB-LOGS-2022-2026]] |

### 50/50 (Use if audience is receptive)

| Item | Dollar Impact | Finding | Source Evidence |
|------|--------------|---------|-----------------|
| Individual fuel card fraud patterns (pending card pulls) | Unquantified — requires EFS transaction pulls | [[Fuel Card Overview]] | Awaiting EFS data for cards *0042, *0048 |
| Flagged system users (sknuckles) | Unassessed | [[Other Flagged Users]] | [[DOC-QB-LOGS-2022-2026]] or [[Apollo Quickbooks Audit Trail 2023 to dec 2024]] |
| November settlement check void/re-issue pattern ($61K) | $61,459 | [[Bank Rec Analysis 2025]] | [[Bank Rec Analysis 2025]] (2025-11-03) |
| December $0.00 settlement checks (settlements diverted?) | Unquantified — $0 issued to active drivers | [[Bank Rec Analysis 2025]] | [[Bank Rec Analysis 2025]] (2025-12-15) |
| UCNG Gemini $20,880 pass-through transaction | $20,880 | [[Gemini Record Manipulation]] | [[Bank Rec Analysis 2025]] (2025-11-12) |

### Leave Alone (Don't raise unless asked)
- Speculative connections without hard evidence
- Any findings where prior AI outputs haven't been fully stress-tested

## Presentation Principles
1. Lead with independent, verifiable evidence (IFTA, bank, EFS)
2. Show the pattern before the individual anomalies
3. Acknowledge where reasonable minds could differ — this builds credibility
4. Frame as "here's what the numbers show" not "here's what they did"
5. The ask: investment capital + independent financial controls for Apollo

## Finding Links
- [[Fuel Cost Manipulation]] | [[Intercompany Transfer Tracker]] | [[Promissory Note Backdating]]
- [[Revenue Timing Shift]] | [[ATI Monthly Billing Manipulation]]
- [[GL Audit Trail Anomalies]] | [[Gemini Record Manipulation]]
- [[Bank Rec Analysis 2024]] | [[Bank Rec Analysis 2025]]
- [[Cash Flow Dashboard]] | [[Master Timeline]]

## Chain of Custody
- [[Source Registry]] | [[Data Lineage]]
