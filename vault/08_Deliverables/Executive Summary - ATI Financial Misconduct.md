---
type: deliverable
status: preliminary
tags: [deliverable, critical]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Master Narrative]]"
  - "[[Evidence Strength Matrix]]"
  - "[[Intercompany Transfer Tracker]]"
  - "[[Forensic Cross-Reference Report]]"
  - "[[Grandparent Meeting Prep]]"
---

# Executive Summary — Financial Irregularities in the Management of Apollo Energy Resources LLC

---

**APOLLO ENERGY RESOURCES LLC (Claimant)**
v.
**ASPHALT TRANSPORT INC (Respondent)**

---

**Prepared by:** Internal Investigation Team
**Date:** 2026-03-24
**Status:** Preliminary — Subject to supplementation upon receipt of outstanding documents

---

## Background

1. Apollo Energy Resources LLC ("Apollo") is a trucking subsidiary whose financial operations — including bank accounts, accounting systems, journal entries, asset titles, and financial reporting — are exclusively controlled by its parent company, Asphalt Transport Inc ("ATI"). Apollo's owner has no independent access to Apollo's bank accounts or accounting system.

2. In March 2026, an internal investigation was initiated after Apollo's owner obtained bank reconciliation files and QuickBooks transaction logs. Forensic analysis of these records, cross-referenced against independent third-party data, revealed a pattern of financial irregularities spanning 2023–2025.

---

## Summary of Findings

The investigation has identified the following accounting anomalies and unexplained financial transfers, supported by independent verification where noted:

**Finding 1 — Unexplained Net Cash Transfers: $915,887.** Between January 2024 and December 2025, ATI transferred $1,201,658 out of Apollo's Stellar Bank account in cumulative "paydowns." ATI returned $285,771 during the same period, resulting in a net outflow of $915,887 from Apollo. These transfers are verified penny-for-penny against independent bank statements. No executed loan agreements or board resolutions authorizing these transfers have been produced. *(Source: [[Intercompany Transfer Tracker]], [[Bank Rec Analysis 2024]], [[Bank Rec Analysis 2025]])*

**Finding 2 — Fuel Expense Overstatement: $422,078 (83.3%).** Apollo's 2025 profit-and-loss statement reports $928,570 in total fuel costs. Independent EFS fuel card records and corresponding bank payments show Apollo actually paid $506,492. The $422,078 difference exists entirely in manual journal entries with no supporting invoices. ATI's own fleet reports fuel costs at 3.1% of revenue; Apollo's P&L shows 24.9%. *(Source: [[Forensic Cross-Reference Report]], [[Apollo Fuel 2023 2025]], [[Bank Rec Analysis 2025]])*

**Finding 3 — Fuel Payable Account Manipulation: $527,073.** GL Account 2010 ("Fuel Payable") accumulated $322,639 throughout 2024 without being cleared. On March 31, 2025, two manual journal entries zeroed the account: $285,789 was reclassified to Fuel Expense and $241,284 was deducted from Cash. Both entries were posted 79–84 days after their stated transaction date. *(Source: [[Account 2010 Fuel Payable Mechanism]], [[Apollo_Manual_Journal_Fuel_Targets]])*

**Finding 4 — Promissory Note Backdating: $858,000.** A promissory note creating $858,000 in liability on Apollo's balance sheet was entered into the accounting system 174 days after its purported execution date, as confirmed by QuickBooks batch timestamp analysis. No executed copy of this note has been produced. *(Source: [[Promissory Note Backdating]], [[DOC-QB-LOGS-2022-2026]])*

**Finding 5 — Intercompany Profit Retention: $340,909.** Gemini Logistics USA LLC, an ATI-related entity, earned $127,964 in net profit over 24 months operating through Apollo. None of this profit was distributed to Apollo. Meanwhile, Apollo's recorded debt to Gemini grew by $212,945 — exceeding Gemini's total earnings. *(Source: [[Gemini Profit Siphon]], [[ATI GL 2023 - Gemini N-R Analysis]])*

**Finding 6 — Record Destruction.** Twenty-three Gemini-related accounting records were deleted by a single user in approximately 25 minutes. The content and dollar value of the deleted records cannot be determined without a database backup predating the deletion event. *(Source: [[Gemini Record Manipulation]], [[DOC-QB-LOGS-2022-2026]])*

**Finding 7 — Systematic Backdating of Journal Entries.** The primary financial operator (responsible for 47.5% of all journal entries) has a backdating rate of 39.4% for entries exceeding 30-day lag. The most extreme instance is a 476-day retroactive entry. The accounting system has no audit trail enabled. *(Source: [[GL Audit Trail Anomalies]], [[DOC-QB-LOGS-2022-2026]])*

---

## Aggregate Documented Exposure

| Category | Amount | Verification Level |
|----------|--------|--------------------|
| Net cash transferred from Apollo to ATI | $915,887 | Bank-verified |
| 2025 fuel expense overstatement (P&L vs actual) | $422,078 | Triple-verified (EFS + bank + IFTA) |
| Backdated promissory note | $858,000 | QB timestamps |
| Intercompany profit retained / phantom debt | $340,909 | Cross-entity P&L |
| Total intercompany debt on Apollo books | $2,089,420 | Balance sheet |

*Note: Certain figures above overlap (e.g., fuel overstatement is a component of the mechanism enabling cash extraction). A detailed reconciliation with double-counting analysis is maintained in [[04_Cash_Flow/Master Financial Reconciliation]].*

---

## Directional Consistency

Every identified anomaly moves value in a single direction: away from Apollo and toward ATI or ATI-controlled entities. No anomaly was identified that disadvantages ATI or benefits Apollo.

---

## Recommended Next Steps

1. **Formal document demand** to ATI for all items listed in [[Outstanding Document Demands]], with particular urgency for EFS portal exports, executed loan agreements, and the $858,000 promissory note.
2. **Independent forensic accounting review** of the findings documented in this investigation.
3. **Immediate implementation** of accounting system audit trail.
4. **Grant Apollo's owner** independent access to Apollo's bank accounts and accounting system.
5. **Preservation notice** to ATI regarding all electronic records, accounting databases, and communications related to Apollo, Gemini, and intercompany transactions.

---

## Evidentiary Basis

This summary is supported by bank statements (independent), government-sworn IFTA filings, third-party EFS fuel card records, QuickBooks transaction logs (SHA-256 preserved), and ATI's own general ledger files. A complete chain of custody is maintained in the investigation vault. See [[Evidence Strength Matrix]] for a finding-by-finding admissibility assessment.

---

*This document is preliminary and subject to revision upon receipt of outstanding documents. It does not constitute legal advice.*
