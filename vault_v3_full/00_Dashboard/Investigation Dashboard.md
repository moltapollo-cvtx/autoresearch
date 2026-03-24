---
tags: [dashboard]
updated: 2026-03-23
---

# Investigation Dashboard
> **Project Codename:** Whoopsie
> **Subject:** ATI / Apollo Energy Resources Financial Investigation
> **Owner:** Walker (Apollo Energy Resources LLC)
> **Status:** Active — Building evidentiary record for grandparent company meeting

---

## Quick Links
- [[Cash Flow Dashboard]] — Follow the money
- [[Document Registry]] — Every document received, when, from whom
- [[Master Timeline]] — Chronological event reconstruction
- [[Evidence Tiers]] — Must Hit / Ought to Hit / Should Hit / 50/50 / Leave Alone
- [[Outstanding Document Demands]] — What we still need

---

## Core Thesis

ATI (Asphalt Transport, Inc.) holds exclusive financial control over Apollo Energy Resources LLC — bank accounts, cash flows, asset titles, and the accounting system. There is **no audit trail** on the finance system, meaning journal entries can be altered without record. The investigation has identified a consistent, one-directional pattern of anomalies: Apollo's books are inflated on the expense side, ATI's books are deflated. The largest single category of concern is **fuel transactions**, where the gap between independently verifiable fuel spend (~$433K per IFTA/EFS) and ATI-reported fuel cost (~$720K on P&L) is approximately **$287K (~66% markup)**.

**As of 03/23/2026:** Bank-level cash flow data now covers the full 24-month period (Jan 2024–Dec 2025), confirming ATI extracted a gross **$1,201,658** from Apollo ($916K net of advances returned).

---

## Key Findings Summary

| # | Finding | Est. Impact | Confidence | Status | Link |
|---|---|---|---|---|---|
| 1 | Net ATI cash extraction (2024+2025) | **$915,887** | HIGH | Bank-verified | [[Intercompany Transfer Tracker]] |
| 2 | Gross ATI extraction (2024+2025) | **$1,201,658** | HIGH | Bank-verified | [[Intercompany Transfer Tracker]] |
| 3 | Fuel cost overstatement | ~$287K | HIGH | Documented | [[Fuel Cost Manipulation]] |
| 4 | Promissory note backdating | $858K note | HIGH | Confirmed | [[Promissory Note Backdating]] |
| 5 | Revenue timing shift (1-mo forward) | ~$145K understated FY2024 | MED-HIGH | Partial | [[Revenue Timing Shift]] |
| 6 | ATI monthly billing manipulation | TBD | MED-HIGH | Documented | [[ATI Monthly Billing Manipulation]] |
| 7 | Gemini record mass deletion | 23 records | HIGH | Confirmed | [[Gemini Record Manipulation]] |
| 8 | GL retroactive journal entries | 476-day backdated entry | HIGH | Confirmed via QB | [[GL Audit Trail Anomalies]] |
| 9 | Fuel charging mechanism (2023 GL) | $234,683 undocumented | HIGH | Confirmed both sides | [[Fuel Cost Manipulation]] |
| 10 | Oct 2025 peak extraction | $355K in single month | HIGH | Bank-verified | [[Bank Rec Analysis 2025]] |
| 11 | Nov void/re-issue pattern | $61,459 voided same-day | MED-HIGH | Documented | [[Bank Rec Analysis 2025]] |
| 12 | Dec $0.00 settlement checks | Unknown — diverted? | MEDIUM | Needs investigation | [[Bank Rec Analysis 2025]] |
| 13 | $84,960 Ins/Elog charge | $84,960 undocumented | HIGH | Action needed | [[Bank Rec Analysis 2025]] |
| 14 | $241,284 "ADJ TO STMT" | $241,284 unexplained | **CRITICAL** | Action needed | [[Bank Rec Analysis 2025]] |
| 15 | Unidentified user "Mauree" | 4,379 entries | MEDIUM | Needs ID | [[Mauree]] |
| 16 | 2024 account drain ($365K→$9K in 6mo) | Cash flow pattern | HIGH | Bank-verified | [[Bank Rec Analysis 2024]] |
| 17 | 2024 ATI extraction (zero returned) | $335,566 | HIGH | Bank-verified | [[Bank Rec Analysis 2024]] |
| 18 | GIG Transportation (suspected Gemini) | $111,924 | MEDIUM | Entity unconfirmed | [[Bank Rec Analysis 2024]] |
| 19 | 2024 Nov overdraft (-$44,470) | Cash starvation | HIGH | Bank-verified | [[Bank Rec Analysis 2024]] |
| 20 | Fuel card fraud (post-termination) | TBD — awaiting pulls | MEDIUM | In progress | [[Fuel Card Overview]] |

---

## Entity Map

```
Grandparent Company (ATI's Parent)  ← Target audience for meeting
        │ owns
        ▼
ATI (Asphalt Transport, Inc.)       Jimmy (President)
  Carrier ID: 318067                Rosanna Karim (Controller/VP Finance)
                                    James Luhr Jr. (Signatory)
        │ subsidiary / controls finances
        ▼
Apollo Energy Resources LLC         Walker (Owner)
  Carrier ID: 5725124              Cordee, Cody (Team)
  Bank: Stellar Bank Acct 21920400

Gemini Logistics USA LLC            ← Related entity under investigation
                                      Records mass-deleted by Cordee
                                      Confirmed transacting through Apollo's bank

GIG Transportation Services         ← 2024: $112K paid from Apollo
                                      Suspected Gemini affiliate — needs verification
```

---

## Methodology

1. **External evidence triangulation** — Because ATI controls Apollo's books with no audit trail, internal records are unreliable. We anchor to independent sources: IFTA government filings, EFS fuel card data, Stellar Bank statements/reconciliations.
2. **Document receipt timestamping** — Every document is logged with receipt date, generation date, and submitting party. Any YTD figure that changes between successive submittals is proof of retroactive manipulation.
3. **Directional consistency test** — Any single anomaly might have an innocent explanation. But when every anomaly moves money in the same direction (Apollo inflated, ATI deflated), the probability of innocence collapses.
4. **Adversarial self-critique** — We actively identify where reasonable minds could differ, strengthening the case by preemptively addressing counterarguments.
5. **Two-year reconstruction** — With 2024 and 2025 bank recs, we now have a complete cash flow picture showing escalating extraction.

---

## Tags Reference
- `#finding` — A documented investigative conclusion
- `#evidence` — A specific piece of source evidence
- `#entity` — A person or company
- `#document` — A received financial document
- `#timeline` — A dated event
- `#cash-flow` — Money movement tracking
- `#action-needed` — Requires follow-up
- `#strategy` — Meeting prep and legal strategy
- `#template` — Reusable note template

---

## Session Log

| Date | Session Summary | Key Outputs |
|---|---|---|
| — | Initial vault creation — backfilled all findings to date | Vault v1 |
| 03/23/2026 | QB Transaction Log forensic analysis (26,993 rows); Bank Rec PDF verification & SHA-256 hashing; Confirmed all prior findings from primary source data | [[DOC-QB-LOGS-2022-2026]], [[Mauree]], SHA-256 hashes, 5 new bank rec findings, vault v2 |
| 03/23/2026 | **2024 bank recs (13 .xlsm files) ingested; Two-year cash flow reconstruction; ATI extraction quantified at $1.2M gross / $916K net; GIG Transportation entity flagged; Forensic workbook produced** | [[Bank Rec Analysis 2024]], updated [[Intercompany Transfer Tracker]], updated [[Fuel Spend Reconciliation]], updated [[Cash Flow Dashboard]], `Apollo_Forensic_CashFlow_Analysis.xlsx`, vault v3 |
| — | _Next session..._ | |
