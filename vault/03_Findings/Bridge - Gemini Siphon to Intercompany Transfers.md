---
type: finding
status: documented
confidence: critical
tags: [finding, critical, bridge]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Gemini Profit Siphon]]"
  - "[[Intercompany Transfer Tracker]]"
  - "[[Gemini Record Manipulation]]"
  - "[[GIG Transportation Services]]"
evidence-refs:
  - "[[ATI GL 2023 - Gemini N-R Analysis]]"
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[Apollo 2023 to dec 2024 General Ledger]]"
---

# Bridge: Gemini Profit Siphon → Intercompany Cash Extraction

> This note connects the **Gemini balance sheet manipulation** (phantom debt growth, profit trapping) to the **physical cash extraction** documented in bank reconciliations and intercompany transfer records.

---

## Two Sides of the Same Mechanism

### The Gemini Side (Balance Sheet)
- Gemini earned $127,964 in net profit over 24 months ([[Gemini Profit Siphon]])
- NONE flowed to Apollo (zero dividends, zero distributions)
- Instead, Gemini's "Note Receivable from Apollo" grew by $212,945 — $85K MORE than Gemini even earned
- Apollo's NP Gemini (2410) reached $924,186 by Dec 2025
- Gemini's own retained earnings DECREASED by $55,460 despite positive net income (~$183K removed via unidentified adjustments)

### The Cash Side (Bank Transfers)
- ATI extracted $1,201,658 gross from Apollo over 2024-2025 ([[Intercompany Transfer Tracker]])
- The "paydowns" are labeled as debt service on intercompany notes
- Apollo's total intercompany debt (Jan 2025): $2,089,420 — NP Gemini ($815K) + NP ATI ($416K) + ATI Promissory ($858K)
- GIG Transportation received $111,924 from Apollo in 2024, appears to be Gemini-related ([[GIG Transportation Services]])

### The Connection

```
GEMINI earns profit ($127,964)
    │
    ▼ (profits trapped — never distributed)
NR APOLLO grows on Gemini's books (+$212,945)
    │
    ▼ (mirror image)
NP GEMINI grows on Apollo's books → $924,186
    │
    ▼ (combined with NP ATI + Promissory = $2.09M)
TOTAL INTERCOMPANY DEBT justifies...
    │
    ▼
"PAYDOWNS" — $1.2M extracted from Apollo's bank
    │
    ▼ (verified independently)
BANK STATEMENTS confirm cash left Apollo
```

**The Gemini profit siphon is not separate from the cash extraction — it is one of the mechanisms creating the JUSTIFICATION for it.** By growing Apollo's paper debt to Gemini (and ATI), the entities controlled by ATI create a pretext for extracting cash from Apollo.

---

## The GIG Transportation Connection

GIG Transportation Services received $111,924 from Apollo's bank account in 2024 ([[GIG Transportation Services]]):
- Biweekly payments Jan–May 2024
- GIG appears in EFS fuel card payables as "GIGTRANSPORTATIONSER"
- Payments stopped abruptly in May 2024

If GIG is a Gemini affiliate (under investigation), this represents an additional $112K extraction channel beyond the documented $916K net — potentially raising the two-year total from $915,887 to $1,027,811.

---

## Evidence That the Debt Is Fabricated

| Indicator | Detail | Source |
|-----------|--------|--------|
| Promissory note backdated | $858K note proven backdated by 174 days | [[Promissory Note Backdating]] |
| Gemini records mass-deleted | 23 records destroyed by [[Cordee]] in ~25 minutes | [[Gemini Record Manipulation]] |
| Gemini liabilities batch-entered | All NP entries created in single session by [[Rosanna Karim]] | [[Gemini Record Manipulation]] |
| NR Apollo exceeds Gemini's earnings | Debt grew $85K more than Gemini's total net income | [[Gemini Profit Siphon]] |
| Customer payments reclassified | Apollo revenue credited to NP Gemini ("overpayment for Gemini invoices") | [[Forensic Cross-Reference Report]] |

---

## Connected
- [[Forensic Cross-Reference Report]] — NP Gemini balance sheet analysis
- [[Account 2010 Fuel Payable Mechanism]] — Parallel manipulation mechanism (fuel instead of intercompany)
- [[Master Timeline]] — Chronological view of extraction events
- [[Cash Flow Dashboard]] — Running totals
