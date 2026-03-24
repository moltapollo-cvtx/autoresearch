---
tags: [finding]
status: documented
confidence: critical
estimated_impact: "$127,964 trapped profits + $212,945 phantom debt growth"
direction: apollo-inflated
documented_date: 2026-03-24
---

# Gemini Profit Siphon — Profits Earned, Never Delivered

## CRITICAL FINDING: Gemini is Profitable, But Apollo Never Sees a Dime

### 24-Month Gemini P&L (Jan 2024 – Dec 2025)

| Metric | 2024 | 2025 | 24-Month Total |
|--------|------|------|---------------|
| Total Revenue | $752,928.83 | $1,179,074.22 | **$1,932,003.05** |
| Total Expenses | $686,263.46 | $1,117,775.63 | $1,804,039.09 |
| **Net Income** | **$66,665.37** | **$61,298.59** | **$127,963.96** |

Source: All 24 Gemini monthly P&L CSVs (Gemini January 2024.csv through Gemini 2025 December.csv)

**Gemini generated $127,964 in net profit over 24 months. NONE of it flowed to Apollo.**

---

## The Mechanism: NR Apollo (Note Receivable)

Instead of distributing profits to Apollo, Gemini's books show an ever-growing "Note Receivable from Apollo":

| Date | NR Apollo (Gemini's books) | NP Gemini (Apollo's books) | Verified Match |
|------|--------------------------|---------------------------|----------------|
| Jan 2024 | $711,240.69 | $711,240.69 | YES |
| Dec 2024 | $803,663.10 | $803,663.10 | YES |
| Jan 2025 | $815,445.37 | $815,445.37 | YES |
| Dec 2025 | $924,185.80 | $924,185.80 | YES |

**24-month growth: +$212,945.11**

The receivable grew by MORE than Gemini's total profits ($212K > $128K). Not only did Apollo not receive Gemini's profits — Apollo's DEBT to Gemini increased by $85K more than Gemini even earned.

---

## Apollo's Total Intercompany Debt (Jan 2025)

| Creditor | Amount | Controlled By |
|----------|--------|---------------|
| NP Gemini (2410) | $815,445.37 | ATI |
| NP ATI (2420) | $415,639.99 | ATI |
| ATI Promissory (2430) | $858,334.89 | ATI |
| **TOTAL** | **$2,089,420.25** | **ALL ATI** |

Apollo's Retained Earnings: **($1,182,612.17)** — deeply negative.

Apollo is technically insolvent on a retained earnings basis, while carrying $2.09M in intercompany debt to entities controlled by the same parent company that controls Apollo's books.

---

## Gemini Retained Earnings Anomaly

| Date | Gemini RE | Expected Change | Actual Change |
|------|-----------|----------------|---------------|
| Jan 2024 | $297,667.18 | — | — |
| Dec 2025 | $242,207.08 | +$127,964 (net income) | **-$55,460** |

Gemini's retained earnings **DECREASED** by $55,460 despite earning $127,964 in net income. That means approximately **$183,424** was removed from Gemini's retained earnings through unidentified adjustments — likely reclassified to build the NR Apollo receivable or transferred to ATI.

---

## How the Money Flows (The Complete Picture)

```
CUSTOMERS pay for freight services
        │
        ▼
GEMINI earns revenue ($1.93M over 24 months)
  - Pays carriers ($1.80M)
  - Net income: $127,964
        │
        ▼ (profits DO NOT flow to Apollo)
GEMINI'S BALANCE SHEET
  - NR Apollo grows (+$212,945)
  - Apollo "owes" Gemini more each month
  - No dividends, no distributions
        │
        ▼
APOLLO'S BALANCE SHEET
  - NP Gemini grows to $924,186
  - NP ATI: $534,601
  - ATI Promissory: $858,335
  - Total intercompany debt: $2.09M
  - Retained Earnings: ($1.18M)
        │
        ▼
ATI EXTRACTS CASH
  - $1.2M gross extraction (2024-2025)
  - "Paydowns" on fabricated notes
  - Fuel GJ entries inflate expenses
```

---

## Gemini Expense Anomalies

1. **Feb 2024: $18,203 Professional Service Fee** — 44.5% of that month's revenue, never repeated
2. **Mar 2024: $13,726 Cargo Insurance** — one-time charge, never repeated in 2024
3. **Jun 2024: ($10,130) Revenue Reversal** — drove Gemini to $22,789 loss that month
4. **Jan 2025: Carrier Pay ($184,176) exceeds Revenue ($148,863)** — $35K loss when carrier pay shouldn't exceed freight revenue
5. **No management fees or back-office charges appear in Gemini P&L** — extraction happens entirely through balance sheet manipulation

---

## ATI's Own Financial Position (2025)

Source: [[ATI 2025 Profit & Loss MoM]]

| Metric | ATI 2025 |
|--------|----------|
| Revenue | $37,102,495 |
| Total Expenses | $37,070,364 |
| EBITDA | $32,131 |
| Net Loss | **($1,968,494)** |

ATI itself is losing nearly $2M despite $37M in revenue. This raises the question: is ATI pushing its own costs onto Apollo to make ATI's P&L look less catastrophic?

---

## Connected
- [[Gemini Record Manipulation]] — 23 records mass-deleted by [[Cordee]]
- [[Gemini Logistics USA LLC]] — Entity profile
- [[Intercompany Transfer Tracker]] — Cash extraction
- [[Forensic Cross-Reference Report]] — NP Gemini balance sheet analysis
- [[Account 2010 Fuel Payable Mechanism]] — Fuel cost inflation
- [[ATI GL 2023 - Gemini N-R Analysis]] — ATI-side Gemini entries
- [[Master Timeline]]

## Source Files
- All 24 Gemini monthly P&L CSVs (2024-2025)
- [[ATI 2025 Profit & Loss MoM]] — ATI financials
- Apollo 2024 January.csv / Apollo 2025 January.csv — Balance sheet verification
- [[Source Registry]] | [[Data Lineage]]
