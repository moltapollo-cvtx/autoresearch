---
type: cash-flow
status: active
tags: [synthesis, critical]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Intercompany Transfer Tracker]]"
  - "[[Account 2010 Fuel Payable Mechanism]]"
  - "[[Forensic Cross-Reference Report]]"
  - "[[Gemini Profit Siphon]]"
  - "[[Promissory Note Backdating]]"
  - "[[Revenue Timing Shift]]"
  - "[[Cross-Entity Transaction Map]]"
  - "[[Master Narrative]]"
evidence-refs:
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo 2025 December]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[ATI GL 2023 - Gemini N-R Analysis]]"
---

# Master Financial Reconciliation

> Every dollar figure in this investigation, reconciled to source, with double-counting risks identified. This is the single note an attorney or CPA should use to validate the financial claims.

---

## A. Cash Extraction (Bank-Verified)

These are actual cash movements confirmed via independent Stellar Bank statements.

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| A1 | Gross Apollo → ATI transfers (2024) | $335,566 | [[Intercompany Transfer Tracker]] | Bank statements |
| A2 | Gross Apollo → ATI transfers (2025) | $866,092 | [[Intercompany Transfer Tracker]] | Bank statements |
| A3 | **Total gross ATI extraction** | **$1,201,658** | [[Intercompany Transfer Tracker]] | Bank statements |
| A4 | ATI → Apollo advances (2025 only) | ($285,771) | [[Intercompany Transfer Tracker]] | Bank statements |
| A5 | **Total documented ATI extraction (net)** | **$915,887** | [[Intercompany Transfer Tracker]] | Bank statements |

---

## B. Fuel Overstatement (P&L vs Independent Sources)

These are P&L inflation amounts — what Apollo's books say versus what Apollo actually paid.

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| B1 | 2025 P&L grand total fuel | $928,570 | [[Forensic Cross-Reference Report]] | ATI-prepared P&L |
| B2 | 2025 EFS actual cash paid for fuel | ($506,492) | [[Fuel Spend Reconciliation]] | Bank + EFS (independent) |
| B3 | **2025 fuel overstatement (all mechanisms)** | **$422,078** | [[Forensic Cross-Reference Report]] | Triple-verified |
| B4 | 2023 fuel journal entries (GJ to NP ATI) | $234,683 | [[Fuel Cost Manipulation]] | QB logs + ATI GL |
| B5 | **Total documented fuel fraud (non-overlapping)** | **$656,761** | [[SYNTHESIS - Fuel Fraud Complete Picture]] | See note below |

> [!WARNING] Double-Counting Risk — Lines B3 and B4
> B3 ($422,078) covers the 2025 overstatement, which INCLUDES the $285,789 Account 2010 dump. B4 ($234,683) covers 2023 only. These do NOT overlap. The $656,761 combined total is clean.

---

## C. Account 2010 Fuel Payable Mechanism (Subset of B)

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| C1 | Account 2010 fuel dump to Fuel Expense | $285,789 | [[Account 2010 Fuel Payable Mechanism]] | GL entries |
| C2 | ADJ TO STMT cash reduction | $241,284 | [[Account 2010 Fuel Payable Mechanism]] | GL + bank |
| C3 | **Combined Account 2010 impact** | **$527,073** | [[Account 2010 Fuel Payable Mechanism]] | GL + bank |

> [!WARNING] Double-Counting Risk — Lines C1 and B3
> C1 ($285,789) is a SUBSET of B3 ($422,078). Do not add these. The Account 2010 dump is one component of the total 2025 fuel overstatement. C2 ($241,284 cash reduction) is a separate balance sheet impact not captured in B3.

---

## D. Gemini-Related Exposure

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| D1 | Gemini net profits earned, not distributed to Apollo | $127,964 | [[Gemini Profit Siphon]] | Cross-entity P&L |
| D2 | NP Gemini growth (phantom debt increase, 24 months) | $212,945 | [[Gemini Profit Siphon]] | Balance sheet |
| D3 | **Gemini total exposure (trapped profit + phantom debt)** | **$340,909** | [[Gemini Profit Siphon]] | Cross-entity P&L |
| D4 | NP Gemini balance (Dec 2025) | $924,186 | [[Forensic Cross-Reference Report]] | Balance sheet |
| D5 | Gemini batch entries (Rosanna, single session) | $282,416 | [[Gemini Record Manipulation]] | QB logs |

> [!WARNING] Double-Counting Risk — Lines D2 and D5
> D5 ($282,416) represents the batch journal entries that CREATED part of the Gemini liability in 2023. D2 ($212,945) is the 2024–2025 growth. These cover different time periods and do NOT overlap. However, D5 is a subset of the total NP Gemini balance (D4), not additional exposure.

---

## E. Balance Sheet Manipulation

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| E1 | Backdated promissory note | $858,000 | [[Promissory Note Backdating]] | QB timestamps |
| E2 | Wire Payable disappearance (2011 collapse) | $868,535 | [[Forensic Cross-Reference Report]] | Balance sheet delta |
| E3 | Total intercompany debt on Apollo books (Jan 2025) | $2,089,420 | [[Gemini Profit Siphon]] | Balance sheet |
| E4 | Apollo retained earnings (Jan 2025) | ($1,182,612) | [[Gemini Profit Siphon]] | Balance sheet |

> [!WARNING] Double-Counting Risk — Lines E1 and E2
> E1 ($858K promissory) and E2 ($868K Wire Payable collapse) likely represent the SAME money reclassified. The Wire Payable disappeared as the Promissory Note appeared. Do NOT add these — they are almost certainly the same transaction relabeled. The net new exposure from the promissory note is the difference between what was legitimately owed and what was fabricated, which cannot be determined without the executed note.

---

## F. Revenue and Billing Manipulation

| Line | Description | Amount | Source Finding | Verification |
|------|-------------|--------|---------------|-------------|
| F1 | Revenue timing understatement (FY2024) | ~$145,000 | [[Revenue Timing Shift]] | Year-over-year TB comparison |
| F2 | ATI monthly billing overcharge | Unquantified | [[ATI Monthly Billing Manipulation]] | Needs intercompany agreement |
| F3 | GIG Transportation payments (entity unconfirmed) | $111,924 | [[Intercompany Transfer Tracker]] | Bank-verified |

---

## G. Unquantified Exposure

| Item | Status | What Would Resolve It |
|------|--------|-----------------------|
| Card *0048 post-termination fuel charges | Pending Collins termination date | EFS transaction pull + HR records |
| $84,960 "Ins/Elog" charge (Nov 2025) | Undocumented | Itemized invoices from ATI |
| ATI billing overcharge total | Unquantified | Intercompany billing agreement |
| Value of 23 deleted Gemini records | Unknown | QB database backup predating deletion |
| Insurance allocation gap (Nov-Dec 2024) | ~$102,520 estimated | Insurance policy + allocation explanation |

---

## GRAND TOTAL — DOCUMENTED EXPOSURE

| Category | Amount | Overlap Notes |
|----------|--------|---------------|
| **Net cash extraction (A5)** | **$915,887** | Bank-verified; standalone |
| **2025 fuel overstatement (B3)** | **$422,078** | P&L vs actual; OVERLAPS with cash extraction mechanism |
| **2023 fuel journal entries (B4)** | **$234,683** | Does NOT overlap with B3 |
| **Gemini trapped profits (D1)** | **$127,964** | Cross-entity; standalone |
| **Gemini phantom debt growth (D2)** | **$212,945** | Balance sheet; standalone |
| **Promissory note backdating (E1)** | **$858,000** | Balance sheet; likely overlaps E2 |
| **Revenue timing shift (F1)** | **~$145,000** | Partially documented |
| **GIG payments (F3)** | **$111,924** | Bank-verified; entity unconfirmed |

### How to Read These Numbers

**For a cash-focused analysis (what has Apollo actually lost):**
- Net cash out the door: **$915,887** (A5)
- Plus GIG payments if affiliate confirmed: **$111,924** (F3)
- **Cash total: $1,027,811**

**For a P&L inflation analysis (how Apollo's profitability has been suppressed):**
- 2025 fuel overstatement: **$422,078** (B3)
- 2023 fuel journal entries: **$234,683** (B4)
- Revenue timing shift: **~$145,000** (F1)
- **P&L total: ~$801,761**

**For a balance sheet exposure analysis (fabricated obligations on Apollo's books):**
- Total intercompany debt: **$2,089,420** (E3)
- Of which promissory note (backdated): **$858,000** (E1)
- Of which NP Gemini (phantom growth): **$924,186** (D4)
- Apollo retained earnings: **($1,182,612)** (E4)

> [!CRITICAL] These three categories (cash, P&L, balance sheet) are INTERCONNECTED, not additive.
> The fuel overstatement (P&L) creates the inflated debt (balance sheet), which ATI uses to justify the cash extraction. Adding all three would triple-count. **The single most conservative, independently verified number is the $915,887 net cash extraction.** Everything else explains HOW it was accomplished.

---

## Connected
- [[Master Narrative]] — Start here
- [[Cross-Entity Transaction Map]] — Every documented money flow
- [[Evidence Strength Matrix]] — Admissibility assessment
- [[Executive Summary - ATI Financial Misconduct]] — Attorney-ready summary
- [[Forensic Cross-Reference Report]] — Penny-level source data
- [[SYNTHESIS - Fuel Fraud Complete Picture]] — All fuel mechanisms unified
