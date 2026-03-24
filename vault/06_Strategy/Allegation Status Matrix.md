---
type: strategy
tags: [strategy, critical]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Master Narrative]]"
  - "[[Evidence Strength Matrix]]"
  - "[[Master Financial Reconciliation]]"
  - "[[Executive Summary - ATI Financial Misconduct]]"
---

# Allegation Status Matrix

> The single most important strategic document in this vault. Every allegation, claim, and finding — confirmed or not — in one place. Cross-referenced against all source evidence and raw data.
>
> **Last updated:** 2026-03-24 | **Total allegations tracked:** 18

---

## CONFIRMED

| # | Allegation | Status | Confidence | Dollar Amount | Best Evidence | Evidence Type | Missing To Confirm | Finding Link |
|---|-----------|--------|-----------|--------------|---------------|---------------|--------------------|--------------|
| 1 | **Net Cash Extraction** — ATI extracted $1,201,658 gross from Apollo over 2024-2025, returning only $285,771. Net drain: $915,887. October 2025 alone: $355,000 (48% of inflows). | CONFIRMED | CRITICAL | $915,887 | [[Bank Rec Analysis 2024]], [[Bank Rec Analysis 2025]] matching GL transfers penny-for-penny via [[Stellar Bank]] | bank-statement | None — fully verified against independent bank records | [[Intercompany Transfer Tracker]] |
| 2 | **Account 2010 Fuel Payable Dump** — $322,639 accumulated through all of 2024 (never cleared), zeroed 2025-03-31 via $285,789 fuel expense dump + $241,284 cash reduction, both backdated 79-84 days | CONFIRMED | CRITICAL | $527,073 | [[Apollo_Manual_Journal_Fuel_Targets]], [[Apollo_2010_Monthly_Rollforward]], [[Bank Rec Analysis 2025]] | GL-entry + bank-statement | None — mechanism documented from both GL and bank sides | [[Account 2010 Fuel Payable Mechanism]] |
| 3 | **2025 Fuel P&L Overstatement** — Apollo P&L shows $928,570 total fuel vs $506,492 actual EFS payments = 83.3% overstatement ($422,078). ATI's own fleet pays 3.1% of revenue on fuel; Apollo's P&L shows 24.9%. | CONFIRMED | CRITICAL | $422,078 | [[Apollo Fuel 2023 2025]] (EFS) + [[Bank Rec Analysis 2025]] (bank) + [[Apollo IFTA Filing 2024]] (govt) vs [[Apollo 2025 December]] (P&L) | third-party + bank + IFTA | EFS portal exports would further strengthen | [[Forensic Cross-Reference Report]] |
| 4 | **2023 Fuel Journal Entry Fabrication** — Six backdated GJ entries labeled "fuel" totaling $234,683, no supporting invoices, bypass AP cycle. Credited to NP ATI (simultaneously inflating fuel cost AND intercompany debt). | CONFIRMED | HIGH | $234,683 | [[DOC-QB-LOGS-2022-2026]] (Apollo side) + [[ATI GeneralLedger Report 2023]] (ATI side) | QB-log + GL-entry | Fuel invoices for $234K (unlikely to exist) | [[Fuel Cost Manipulation]] |
| 5 | **Systematic GL Backdating** — 39.4% of Rosanna's entries backdated >30 days; Cordee's 476-day extreme; no audit trail enabled; $1.9M+ in total affected entries. QB export preserved with SHA-256 hash. | CONFIRMED | CRITICAL | $1,908,351 (affected) | [[DOC-QB-LOGS-2022-2026]] — system-generated timestamps | QB-log | None — timestamps are system-generated and cannot be disputed | [[GL Audit Trail Anomalies]] |

---

## PARTIAL

| # | Allegation | Status | Confidence | Dollar Amount | Best Evidence | Evidence Type | Missing To Confirm | Finding Link |
|---|-----------|--------|-----------|--------------|---------------|---------------|--------------------|--------------|
| 6 | **Promissory Note Backdating** — $858K note backdated 174 days per QB batch timestamps. *Confirmed:* 174-day timestamp gap proven. *Not confirmed:* Executed copy of note not produced; ATI could claim administrative delay. | PARTIAL | HIGH | $858,000 | [[DOC-QB-LOGS-2022-2026]] batch timestamp vs transaction date | QB-log | Executed copy of $858K promissory note with signatures and notarization | [[Promissory Note Backdating]] |
| 7 | **Gemini Profit Siphon** — $127,964 net profit earned over 24 months, zero distributed; NP Gemini grew $212,945 (more than earned). *Confirmed:* Profit trapping documented from 24 monthly P&Ls. *Not confirmed:* Gemini's legal relationship to ATI — if independent, debt could be legitimate. | PARTIAL | CRITICAL | $340,909 | 24 monthly Gemini P&L CSVs + Apollo balance sheets showing NP growth | GL-entry | Gemini LLC articles of incorporation and operating agreement (TX SOS) | [[Gemini Profit Siphon]] |
| 8 | **Gemini Record Manipulation** — $282,416 batch-created by Rosanna in single session (3 entries, all backdated to month-end dates); 23 records mass-deleted by Cordee in ~25 min. *Confirmed:* Batch entry + deletion events with timestamps. *Not confirmed:* Dollar value of deleted records; who directed deletion. | PARTIAL | HIGH | $282,416 (known) + unknown (deleted) | [[DOC-QB-LOGS-2022-2026]] showing session logs with user identification | QB-log | QB database backup predating deletion session; internal communications re: Gemini | [[Gemini Record Manipulation]] |
| 9 | **GIG Transportation Payments** — $111,924 paid from Apollo in biweekly pattern (Jan-May 2024, 9 payments). *Confirmed:* Payments are bank-verified; GIG appears in EFS fuel card payables. *Not confirmed:* Whether GIG is a Gemini/ATI affiliate — if so, adds to extraction total. | PARTIAL | HIGH (amount) / LOW (significance) | $111,924 | [[Bank Rec Analysis 2024]] showing 9 settlement payments | bank-statement | GIG entity registration (TX SOS); Gemini vendor/subhauler list | [[Forensic Cross-Reference Report]], [[GIG Transportation Services]] |
| 10 | **Monthly GL vs P&L Discrepancies** — $8,669 retained earnings gap + $20,999 missing December depreciation + ~$102,520 insurance allocation gap (Nov-Dec 2024). *Confirmed:* Discrepancies documented penny-for-penny. *Not confirmed:* Whether gaps are year-end errors or intentional manipulation. | PARTIAL | HIGH | ~$131,188 | [[Apollo 2024 January]] through [[Apollo 2024 December]] vs [[Apollo 2023 to dec 2024 General Ledger]] | GL-entry | December 2024 closing journal entries and prior-year adjustments | [[Monthly GL vs Consolidated Reconciliation]] |
| 11 | **Revenue Timing Shift** — ~$145K understated FY2024 via systematic one-month forward shift in revenue recognition. *Confirmed:* Pattern visible in year-over-year trial balance comparison. *Not confirmed:* Whether pattern holds across all 12 months (APL_GL_Comparison_Report analysis was interrupted). | PARTIAL | MEDIUM-HIGH | ~$145,000 | [[Apollo ADJ Trail Balance 2024]] vs [[Apollo ADJ Trial Balance 2023]] | GL-entry | Completed APL_GL_Comparison_Report.xlsx (monthly revenue comparison) | [[Revenue Timing Shift]] |

---

## UNCONFIRMED

| # | Allegation | Status | Confidence | Dollar Amount | Best Evidence | Evidence Type | Missing To Confirm | Finding Link |
|---|-----------|--------|-----------|--------------|---------------|---------------|--------------------|--------------|
| 12 | **ATI Monthly Billing Overcharge** — Variable-to-fixed billing modification visible in GL; every change moved upward. No intercompany billing agreement has been produced. | UNCONFIRMED | MEDIUM | Unquantified | [[ATI GeneralLedger Report 2023]] + [[ATI General Ledger 2022]] showing variable→fixed modification | GL-entry | Intercompany billing agreement; itemized invoices 2022-2025 | [[ATI Monthly Billing Manipulation]] |
| 13 | **Undocumented Ins/Elog Charge** — $84,960 single charge on 2025-11-30 with no supporting invoices or itemized breakdown | UNCONFIRMED | HIGH (amount) / LOW (fraud proof) | $84,960 | [[Bank Rec Analysis 2025]] showing charge in bank data | bank-statement | Itemized invoices comprising the $84,960 from ATI | [[Undocumented Ins-Elog Charge]] |
| 14 | **ATI Chargeback Calculation Errors** — Insurance: $1,100/mo vs $198,000/yr (15x error). E-Logs: $32/mo vs $5,760/yr (15x). Incompetence or deliberate obfuscation unclear. | UNCONFIRMED | MEDIUM | Indeterminate | [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] — ATI's own document with internal math errors | ATI-document | ATI internal insurance billing calculations; actual insurance invoices | [[Forensic Cross-Reference Report]] |

---

## NEEDS-INVESTIGATION

| # | Allegation | Status | Confidence | Dollar Amount | Best Evidence | Evidence Type | Missing To Confirm | Finding Link |
|---|-----------|--------|-----------|--------------|---------------|---------------|--------------------|--------------|
| 15 | **Wire Payable Disappearance** — Account 2011 collapsed from $869,942 to $1,407 between Dec 2024 and Dec 2025. Likely reclassified to ATI Promissory (2430). If so, the $858K note is relabeled existing debt, not new obligation. | NEEDS-INVESTIGATION | MEDIUM | $868,535 | [[Apollo 2024 December]] vs [[Apollo 2025 December]] balance sheet delta | balance-sheet | Account 2011 journal entry detail showing reclassification entries | [[Wire Payable Disappearance]] |
| 16 | **Card \*0048 Post-Termination Fraud** — Highest-spend fuel card in fleet assigned to terminated driver Henry Collins. Every dollar charged after termination is direct theft at the pump. | NEEDS-INVESTIGATION | LOW (pending data) | Unquantified | [[Card 0048 - Henry Collins]] showing highest card spend in fleet | fuel-card | Collins termination date (HR/payroll) + EFS transaction pull for card \*0048 | [[SYNTHESIS - Fuel Fraud Complete Picture]] |
| 17 | **Equipment Loan Pass-Through** — $785K in equipment loans (Truist, WFB) titled to "Asphalt" (ATI) being charged to Apollo at $36,863/month ($442K/year). Apollo may be paying for equipment ATI owns. | NEEDS-INVESTIGATION | MEDIUM | ~$442,358/year | [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] showing loan details and titling | ATI-document | Truist and WFB loan agreements; equipment title documentation | [[Equipment Loan Pass-Through]] |
| 18 | **Gemini Retained Earnings Anomaly** — Gemini RE decreased $55,460 despite earning $127,964 net income. ~$183K removed via unidentified adjustments — likely reclassified to NR Apollo or transferred to ATI. | NEEDS-INVESTIGATION | MEDIUM | ~$183,424 | [[Gemini January 2024]] vs [[Gemini 2025 December]] retained earnings line | GL-entry | Gemini 2024-2025 adjusting journal entries affecting retained earnings | [[Gemini Profit Siphon]] |

---

## Unanalyzed Sources

The following raw data sources in `09_Raw_Data_Index/` contain data that could confirm open allegations but have not been fully analyzed for these specific questions:

| Raw Data File | Relevant Allegation | What It Could Confirm | Priority |
|--------------|---------------------|----------------------|----------|
| [[Apollo 2023 to dec 2024 General Ledger]] | #15 Wire Payable Disappearance | Account 2011 journal entries showing where $868,535 was reclassified | HIGH |
| [[APL GL work]] | #11 Revenue Timing Shift | Monthly revenue comparison — analysis was interrupted before completion | HIGH |
| [[Apollo Fuel 2023 2025]] | #16 Card \*0048 Post-Termination | Card-level transaction data (if card \*0048 identifiable in EFS data) | HIGH |
| [[ATI General Ledger 2022]] | #12 ATI Monthly Billing | Pre-modification billing amounts for baseline comparison | MEDIUM |
| [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] | #17 Equipment Loan Pass-Through | Loan payment schedules and equipment descriptions for cross-reference | MEDIUM |

---

## Summary

### Allegation Count

| Status | Count |
|--------|-------|
| CONFIRMED | 5 |
| PARTIAL | 6 |
| UNCONFIRMED | 3 |
| NEEDS-INVESTIGATION | 4 |
| **Total** | **18** |

### Dollar Exposure

**Total confirmed cash exposure: $915,887** (bank-verified net extraction — most conservative, independently verified number)

**Total confirmed P&L fraud: $656,761** (non-overlapping: $234,683 in 2023 fuel GJ entries + $422,078 in 2025 fuel overstatement)

**Total partial dollar exposure: ~$1,587,021** ($858K promissory + $341K Gemini siphon + $112K GIG + $131K GL discrepancies + $145K revenue timing — significant overlaps exist; see [[Master Financial Reconciliation]])

**Total unconfirmed claims: 3** (at least $84,960 documented + unquantified billing overcharge and chargeback errors)

**Total needs-investigation exposure: ~$1,494K** ($869K Wire Payable + $442K/yr equipment loans + $183K Gemini RE anomaly + unquantified card fraud)

> [!CRITICAL] Double-Counting Warning
> These categories are INTERCONNECTED, not additive. The fuel overstatement creates inflated expenses → generates fabricated intercompany debt → ATI uses that debt to justify cash extraction. See [[Master Financial Reconciliation]] for careful reconciliation of all overlapping figures. The single most defensible number is the **$915,887 net cash extraction** verified against independent bank statements.

### Strongest Case Summary

The investigation's strongest case rests on three independently verified pillars: (1) **$915,887 in net cash extraction** verified penny-for-penny against Stellar Bank statements ATI cannot alter; (2) **$422,078 fuel overstatement** confirmed by triple cross-reference of EFS card data, bank payments, and IFTA government filings vs ATI-prepared P&L; and (3) **systematic backdating pattern** with 39.4% of Rosanna's entries posted >30 days late, including a 476-day extreme, all preserved with SHA-256 hash before alteration was possible. Together, these prove the mechanism (inflate expenses → fabricate debt → extract cash) and the damage ($916K+ out the door).

### Weakest Point / Biggest Gap

The biggest gap is the **absence of Gemini's legal relationship documentation**. If ATI can show Gemini is a genuinely independent entity with legitimate claims, the $924K NP Gemini becomes defensible and the total intercompany debt narrative weakens significantly. Obtaining Gemini's articles of incorporation from the Texas Secretary of State is the single highest-priority document need. Secondary gap: the revenue timing shift analysis ($145K) was interrupted and remains incomplete — completing the APL_GL_Comparison_Report would either confirm or dismiss a $145K allegation.

---

## Graph View Filter Presets

Use these filter strings in Obsidian's graph view search bar:

| View | Filter String | Shows |
|------|--------------|-------|
| **Clean (default)** | `-path:09_Raw_Data_Index -path:07_Templates -file:Untitled` | Core investigation only — findings, evidence, entities, strategy, deliverables |
| **Full** | *(clear search field)* | Everything including all 91 raw data stubs |
| **Smoking Guns** | `tag:#critical` | Only CRITICAL-confidence findings |
| **Presentation Ready** | `path:08_Deliverables OR path:06_Strategy` | Strategy and deliverable documents only |
| **Entities Only** | `path:01_Entities` | All people and companies |

---

## Connected
- [[Master Narrative]] — Start here for the investigation story
- [[Evidence Strength Matrix]] — Admissibility assessment per finding
- [[Master Financial Reconciliation]] — Dollar reconciliation with double-counting analysis
- [[Executive Summary - ATI Financial Misconduct]] — Attorney-ready summary
- [[Open Questions]] — 17 tracked investigative questions
- [[Outstanding Document Demands]] — What documents resolve which gaps
- [[Allegation Status Matrix]] — You are here
