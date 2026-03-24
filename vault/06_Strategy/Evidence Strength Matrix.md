---
type: strategy
tags: [synthesis]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Evidence Tiers]]"
  - "[[Master Narrative]]"
  - "[[Grandparent Meeting Prep]]"
evidence-refs:
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo Fuel 2023 2025]]"
  - "[[Apollo IFTA Filing 2024]]"
---

# Evidence Strength Matrix

> For each finding: what is our best evidence, how admissible is it, and can ATI rebut it? This tells Walker exactly which findings are bulletproof and which need more work.

---

## Strength Assessment

| Finding | Best Evidence | Evidence Type | Admissibility | Can ATI Rebut? | Missing Evidence | Confidence |
|---------|-------------|--------------|---------------|----------------|-----------------|------------|
| **Net Cash Extraction ($915,887)** | [[Stellar Bank]] statements matching GL transfers penny-for-penny | bank-statement | **strong** | **no** — bank records are independent; ATI cannot alter Stellar Bank data | None — fully verified | CRITICAL |
| **Account 2010 Fuel Dump ($527,073)** | [[Apollo_Manual_Journal_Fuel_Targets]] showing exact entries + [[Apollo_2010_Monthly_Rollforward]] showing accumulation + [[Bank Rec Analysis 2025]] confirming $241K cash impact | GL-entry + bank-statement | **strong** | **unlikely** — entries are in ATI's own system with matching bank impact; would have to explain why $286K "fuel" has no EFS transaction | None — mechanism fully documented from both GL and bank | CRITICAL |
| **Fuel Overstatement 83.3% ($422,078)** | [[Apollo Fuel 2023 2025]] (EFS third-party) vs [[Apollo 2025 December]] (P&L) vs [[Bank Rec Analysis 2025]] (bank payments to EFS) | third-party + bank-statement | **strong** | **unlikely** — three independent sources agree (EFS records, bank payments, IFTA); ATI would need to produce $422K in non-EFS fuel purchases | EFS portal exports would strengthen further | CRITICAL |
| **Promissory Note Backdating ($858K)** | [[DOC-QB-LOGS-2022-2026]] batch timestamp vs transaction date showing 174-day lag | QB-log | **moderate** — needs authentication of QB export; ATI could challenge export methodology | **possible** — ATI could claim "administrative delay" in recording; but 174 days for $858K is implausible | QB database backup for independent verification | HIGH |
| **Gemini Profit Siphon ($340,909)** | 24 monthly Gemini P&L CSVs + Apollo balance sheets showing NP Gemini growth | GL-entry | **moderate** — ATI-generated files; need to establish they are authentic | **possible** — ATI could claim Gemini owes Apollo for legitimate services; but NR grew $85K more than Gemini earned | Gemini articles of incorporation; formal intercompany agreement | CRITICAL |
| **Gemini Record Manipulation (23 deleted)** | [[DOC-QB-LOGS-2022-2026]] showing deletion timestamps and user ([[Cordee]]) | QB-log | **moderate** — QB log preserved with SHA-256 hash | **unlikely** — deletion is deletion; ATI would have to explain why 23 records were destroyed in 25 minutes | QB database backup predating deletion; internal communications | HIGH |
| **2023 Fuel GJ Mechanism ($234,683)** | [[DOC-QB-LOGS-2022-2026]] showing 6 entries + [[ATI GeneralLedger Report 2023]] showing ATI-side entries | QB-log + GL-entry | **moderate** | **possible** — ATI could claim fuel costs were legitimate but poorly documented; IFTA/EFS data rebuts this | Detailed fuel invoices for $234K (unlikely to exist) | HIGH |
| **GL Audit Trail Anomalies (476-day)** | [[DOC-QB-LOGS-2022-2026]] showing entry #1169 by [[Cordee]] | QB-log | **moderate** | **no** — 476 days cannot be explained as clerical lag; the entry also happens to inflate fuel and increase NP ATI | None — timestamps are system-generated | HIGH |
| **ATI Monthly Billing Manipulation** | [[ATI GeneralLedger Report 2023]] + [[ATI General Ledger 2022]] showing variable→fixed modification | GL-entry | **moderate** | **yes-easily** — ATI can claim flat-rate billing was a deliberate business decision; without the intercompany agreement showing terms, hard to prove overcharge | Intercompany billing agreement; itemized invoices | MEDIUM |
| **Revenue Timing Shift ($145K)** | [[Apollo ADJ Trail Balance 2024]] vs [[Apollo ADJ Trial Balance 2023]] year-over-year comparison | GL-entry | **needs-authentication** | **possible** — timing differences can be legitimately explained as accrual method; pattern matters but each individual month is defensible | Completed APL GL Comparison Report | MEDIUM-HIGH |
| **GIG Transportation ($111,924)** | [[Bank Rec Analysis 2024]] bank statements showing 9 payments | bank-statement | **strong** — payments are bank-verified | **yes-easily** — ATI can claim GIG is a legitimate subhauler; without proving Gemini affiliation, this is just a vendor payment | GIG entity registration; Gemini vendor list | CONFIRMED (bank) but OPEN (significance) |
| **$84,960 Ins/Elog (undocumented)** | [[Bank Rec Analysis 2025]] showing single 11/30/2025 charge | bank-statement | **strong** — amount is bank-verified | **yes-easily** — ATI can claim this is a legitimate bundled charge; without itemized breakdown, hard to challenge | Itemized breakdown of the $84,960 | HIGH (amount) / LOW (fraud proof) |

---

## Summary by Strength

### Bulletproof (present with confidence)
1. **Net Cash Extraction** — bank-verified, penny-matched, independent
2. **Account 2010 Mechanism** — GL + bank cross-verified, backdating proven
3. **Fuel Overstatement** — triple-verified (EFS + bank + IFTA vs P&L)

### Strong (present with supporting context)
4. **Gemini Profit Siphon** — cross-entity P&L + balance sheet; ATI rebuttal is weak
5. **Gemini Record Manipulation** — deletion timestamps with SHA-256 preserved export
6. **GL Audit Trail Anomalies** — system-generated timestamps; 476 days is indefensible
7. **2023 Fuel GJ Mechanism** — confirmed from both Apollo and ATI sides

### Needs Work (present carefully, note gaps)
8. **Promissory Note Backdating** — strong on timestamps but needs QB authentication
9. **Revenue Timing Shift** — pattern is clear but individual months are defensible
10. **ATI Monthly Billing** — needs intercompany agreement to prove overcharge
11. **GIG Transportation** — bank-confirmed payments but entity affiliation unproven

---

## Evidence Type Legend

| Type | Description | Reliability |
|------|-------------|-------------|
| bank-statement | Stellar Bank records — independent, cannot be altered by ATI | Highest |
| IFTA-filing | Government-sworn fuel data — filed with state authorities | Very High |
| third-party | EFS fuel card records — held by EFS, not ATI | High |
| QB-log | QuickBooks transaction log — ATI-controlled but timestamps reveal backdating; SHA-256 preserved | Moderate-High |
| GL-entry | General Ledger entries — ATI-controlled, no audit trail | Moderate |

See: [[Evidence Bridge - Sources to Findings]] for the complete reliability hierarchy.

---

## Connected
- [[Evidence Tiers]] — Presentation priority (Must Hit / Ought to Hit / Should Hit)
- [[Grandparent Meeting Prep]] — How to present each tier
- [[Master Narrative]] — The story these findings tell
- [[Outstanding Document Demands]] — What would fill the gaps
