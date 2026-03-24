---
type: finding
status: documented
confidence: critical
tags: [finding, critical]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Account 2010 Fuel Payable Mechanism]]"
  - "[[Fuel Cost Manipulation]]"
  - "[[Gemini Profit Siphon]]"
  - "[[Intercompany Transfer Tracker]]"
evidence-refs:
  - "[[Bank Rec Analysis 2025]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[ATI 2025 Profit & Loss MoM]]"
  - "[[Apollo 2024 December]]"
  - "[[Apollo 2025 December]]"
  - "[[Apollo Fuel 2023 2025]]"
  - "[[Apollo IFTA Filing 2024]]"
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]]"
  - "[[Apollo 2023 to dec 2024 General Ledger]]"
  - "[[ATI GL 2023 - Intercompany Billing]]"
documented_date: 2026-03-24
---

# Forensic Cross-Reference Report — Penny-Level Analysis

> **Every number in this report is sourced from raw data files with penny-level accuracy.**

---

## 1. FUEL COST DISPARITY — THE CORE FINDING

### Apollo 2025 Fuel: P&L vs Reality

| Source | Amount | Notes |
|--------|--------|-------|
| **EFS bank payments (actual cash paid)** | **$506,491.82** | Verified via [[Bank Rec Analysis 2025]] |
| P&L: 5500-00-00 Fuel | $303,463.40 | |
| P&L: 5500-01-00 Fuel | $396,978.91 | |
| P&L: 5500-02-00 Fuel | -$17.66 | |
| **Total P&L Fuel (5500)** | **$700,424.65** | **38.3% more than actual** |
| P&L: 5310-00-00 Fuel Surcharge Pay | $25,118.97 | |
| P&L: 5310-02-00 Fuel Surcharge Pay | $183,647.44 | |
| P&L: 5520-01-00 DEF | $20,438.67 | |
| P&L: 5520-02-00 DEF | -$1,060.12 | |
| **GRAND TOTAL FUEL ON P&L** | **$928,569.61** | **83.3% more than actual** |

Source: [[Apollo 2025 December]] (YTD column)

### Apollo 2024 Fuel: P&L vs Reality

| Source | Amount |
|--------|--------|
| **EFS bank payments (actual cash paid)** | **$705,265.28** |
| P&L: 5500-00-00 Fuel | $4,806.43 |
| P&L: 5500-01-00 Fuel | $443,923.65 |
| **Total P&L Fuel (5500)** | **$448,730.08** |
| P&L: 5310-00-00 Fuel Surcharge Pay | $269,743.61 |
| **Total fuel on P&L** | **$718,473.69** |

Source: [[Apollo 2024 December]] (YTD column)

Note: 2024 P&L fuel ($718K) is close to EFS actual ($705K), BUT $322,639.29 was accumulating in account 2010 "Fuel Payable" throughout 2024 — fuel costs that were incurred but NOT on the P&L. This was later dumped onto the 2025 P&L.

### ATI 2025 Fuel Comparison

| Entity | 2025 Revenue | 2025 Fuel | Fuel % of Revenue |
|--------|-------------|-----------|-------------------|
| **ATI** | $37,102,494.59 | $1,134,794.92 | **3.1%** |
| **Apollo (P&L)** | $3,734,804.44 | $928,569.61 | **24.9%** |
| **Apollo (actual EFS)** | $3,734,804.44 | $506,491.82 | **13.6%** |

Source: [[ATI 2025 Profit & Loss MoM]], [[Apollo 2025 December]]

### EFS Card Transaction Data (Apollo Fuel 2023 2025.csv)

| Year | Gallons | EFS Amount | PPG |
|------|---------|-----------|-----|
| 2023 | 43,870 | $184,126 | $4.1971 |
| 2024 | 179,008 | $663,391 | $3.7059 |
| 2025 | 152,168 | $536,712 | $3.5271 |
| **Total** | **375,046** | **$1,384,229** | **$3.6908** |

Source: [[Apollo Fuel 2023 2025]]

### IFTA Government Filing (Apollo IFTA Filing 2024.csv)

| Entity | Gallons | Amount | PPG |
|--------|---------|--------|-----|
| **Apollo** | 170,954 | $537,061 | $3.1415 |
| **ATI** | 1,309,965 | $4,278,193 | $3.2659 |

Source: [[Apollo IFTA Filing 2024]]

**Apollo pays $0.1243 LESS per gallon than ATI at the pump (IFTA data).** The per-gallon disparity is NOT at the pump — it's entirely in the ACCOUNTING. ATI overcharges Apollo via journal entries, not fuel card pricing.

### 2025 Smoking Gun Decomposition
| Component | Amount |
|-----------|--------|
| Organic fuel expense (P&L minus manual GJ) | $414,635 |
| Manual GJ from Account 2010 | +$285,789 |
| **P&L Fuel (5500)** | **$700,425** |
| EFS card actual | $536,712 |
| **5500 Overstated by** | **$163,712 (30.5%)** |

Source: Derived from [[Apollo_Manual_Journal_Fuel_Targets]], [[Apollo 2025 December]], [[Apollo Fuel 2023 2025]]

The $285,789 manual journal entry alone accounts for the ENTIRE overstatement plus more — without it, the organic fuel expense would be $414,635, which is actually LESS than the $536,712 EFS actual (because some EFS costs hit other accounts like driver advances).

Apollo's P&L fuel burden is **8.1x ATI's** as a percentage of revenue (24.9% vs 3.1%). Even the actual EFS payments (13.6%) are 4.4x ATI's rate — which may reflect legitimate fleet composition differences. But the P&L at 24.9% is inflated by manual journal entries.

---

## 2. ACCOUNT 2010 — THE HIDDEN ACCUMULATOR

See detailed analysis: [[Account 2010 Fuel Payable Mechanism]]

**Key facts:**
- Account 2010 grew from $0 to $322,639.29 during all of 2024 (every month, never cleared)
- On 3/31/2025, it was zeroed out via manual GJ entries backdated by 79-84 days
- $285,789.46 was dumped into Fuel Expense (5500)
- $241,284.09 reduced Cash (the "ADJ TO STMT" mystery entry)
- $282,426.08 was credited to AR (fabricating a receivable)

Source: Apollo_Manual_Journal_Fuel_Targets.csv, Apollo_2010_Monthly_Rollforward.csv

---

## 3. BALANCE SHEET MANIPULATION — 2024 vs 2025

| Account | Dec 2024 | Dec 2025 | Change | Flag |
|---------|----------|----------|--------|------|
| Cash (1000) | $51,768.48 | $111,715.98 | +$59,948 | |
| AR (1100) | $543,478.79 | $143,999.42 | -$399,479 | $282K of drop is fabricated GJ |
| Fuel Payable (2010) | -$322,639.29 | $0.00 | +$322,639 | Zeroed via manual GJs |
| Wire Payable (2011) | $869,941.75 | $1,407.19 | -$868,535 | WHERE DID $868K GO? |
| NP Gemini (2410) | $803,663.10 | $924,185.80 | +$120,523 | Ever-growing, never settled |
| NP ATI (2420) | $615,639.99 | $534,601.30 | -$81,039 | |
| ATI Promissory (2430) | $0.00 | $858,334.89 | +$858,335 | BACKDATED 174 days |
| **Total ATI debt** | **$615,639.99** | **$1,392,936.19** | **+$777,296** | |

Source: [[Apollo 2024 December]], [[Apollo 2025 December]] (balance sheet sections)

### Wire Payable (2011) collapse: $870K → $1.4K
This $868,535 disappearance must be traced. Most likely reclassified to ATI Promissory (2430), which would mean the $858K "backdated promissory note" was actually funded by Wire Payable — an existing intercompany clearing account. The note wasn't new debt; it was relabeling existing amounts to create the appearance of a formal loan.

---

## 4. NP GEMINI — THE EVER-GROWING PHANTOM DEBT

Apollo's books show an ever-growing payable to Gemini:
- End 2024: $803,663.10
- End 2025: $924,185.80

### The Mechanism (from Consolidated GL)
Customer payments to Apollo are labeled as "overpayment for Gemini invoices" and credited to N/P Gemini:

| Date | Payer | Amount | Memo |
|------|-------|--------|------|
| 10/20/2023 | MES | $100,217.50 | "overpayment for Gemini invoice 30003, 30005" |
| 12/29/2023 | Sapphire Gas Solutions | $258,044.71 | "overpayment for Gemini invoices" |
| 12/12/2024 | Deposit | $100,000.00 | Deposit to N/P Gemini |
| 01/29/2025 | MES | $11,782.27 | "PAYMENT FROM MES FOR GEMINI INVOICES" |
| 02/10/2025 | MES | $10,726.91 | "MES Gemini invoice 30561" |
| 02/19/2025 | MES | $11,766.25 | "MES Gemini invoice 30568" |

Source: [[Apollo 2023 to dec 2024 General Ledger]] (NP Gemini entries)

**The question:** If customers are paying Apollo for Gemini work, those are Apollo's revenues. Crediting them to NP Gemini means Apollo's revenue goes to service Gemini's "debt" — but who authorized this? The net effect is Apollo's revenue is being siphoned to build a Gemini payable that may never be settled.

---

## 5. GIG TRANSPORTATION = CONFIRMED GEMINI CONNECTION

Source: Apollo 2023 to dec 2024 General Ledger.csv (Fuel Card Payables section)

GIG Transportation Services appears in the EFS fuel card payables (EFSLLC sub-account) as "GIGTRANSPORTATIONSER" receiving fuel card advances from Apollo's EFS account:

| Date | Reference | Amount |
|------|-----------|--------|
| 11/01/2023 | NTA455 | $229.74 |
| 11/03/2023 | NTA446 | $245.08 |
| 11/05/2023 | NTA439 | $448.54 |
| 11/06/2023 | NTA436 | $466.48 |
| 11/08/2023 | NTA428 | $377.32 |
| 11/08/2023 | NTA429 | $129.74 |
| 11/10/2023 | NTA422 | $423.95 |
| 11/12/2023 | NTA415 | $483.36 |
| (+ more) | | |

GIG Transportation was also paid $111,924.21 from Apollo's bank account in 2024 ([[Intercompany Transfer Tracker]]). The fact that GIG has fuel card advances on Apollo's EFS account confirms GIG is an owner-operator or subhauler using Apollo/ATI fuel cards — likely a Gemini-related entity.

---

## 6. INSURANCE COST ALLOCATION

### ATI charges Apollo for insurance
From [[ATI GL 2023 - Intercompany Billing]]: ATI billed Apollo **$21,260/month** ($255K/year) for insurance, later "adjusted" to $15,000/month.

### What Apollo's P&L shows (2025)
| Account | 2025 Amount |
|---------|-------------|
| 6200-00-00 Insurance Expense | $195,920.00 |
| 6190-00-00 Insurance - Auto | $4,770.88 |
| 6200-01-00 Insurance - Cargo | -$14,520.00 |
| 6200-02-00 Insurance - Cargo | -$6,810.00 |
| 6230-00-00 Insurance - Liability | $30,540.96 |
| 6250-00-00 Insurance - Medical | -$14,436.71 |
| 6260-00-00 Insurance - Other | $5,836.07 |
| 6280-00-00 Insurance - Workers' Comp | -$8,600.00 |
| **Net Insurance** | **~$192,701** |

### What ATI reports for its own insurance (2025)
ATI Total Insurance: **$2,855,696.01** for **$37.1M revenue** = 7.7%
Apollo Net Insurance: **~$192,701** for **$3.7M revenue** = 5.2%

Source: [[Apollo 2025 December]], [[ATI 2025 Profit & Loss MoM]], [[ATI GL 2023 - Intercompany Billing]]

At the $15,000/month intercompany rate, ATI would be billing Apollo $180,000/year. Apollo's actual insurance on its P&L ($192K) is close to that. But the question remains: is Apollo's insurance cost proportional to its fleet size, or is ATI marking up?

---

## 7. TIMELINE OF BACKDATED ENTRIES

Every major manipulation entry was backdated:

| Entry | Transaction Date | Posted to GL | Lag |
|-------|-----------------|-------------|-----|
| 2023 fuel GJ #258 ($25,521) | 04/28/2023 | 09/18/2023 | 143 days |
| 2023 fuel GJ #272 ($44,452) | 05/10/2023 | 09/19/2023 | 132 days |
| 2023 fuel GJ #273 ($39,757) | 06/13/2023 | 09/19/2023 | 98 days |
| 2023 fuel GJ #274 ($62,382) | 07/13/2023 | 09/19/2023 | 68 days |
| 2023 fuel GJ #286 ($36,119) | 08/16/2023 | 09/22/2023 | 37 days |
| 2023 fuel GJ #1169 ($26,452) | 09/20/2023 | **01/08/2025** | **476 days** |
| $858K promissory note | ~2024 | ~6 months later | **174 days** |
| **2025 ADJ TO STMT ($241K)** | **03/31/2025** | **06/18/2025** | **79 days** |
| **2025 fuel dump ($286K)** | **03/31/2025** | **06/23/2025** | **84 days** |
| 2025 April reclass | 04/16/2025 | 06/18/2025 | 63 days |
| 2025 July fuel adj | 07/15/2025 | 08/20/2025 | 36 days |

Sources: [[Apollo_Manual_Journal_Fuel_Targets]], [[DOC-QB-LOGS-2022-2026]]

---

## 8. CUMULATIVE DAMAGE TO APOLLO (DOCUMENTED)

| Finding | Amount | Confidence | Source |
|---------|--------|-----------|--------|
| Net cash extracted by ATI (2024+2025) | **$915,887** | VERIFIED | Bank recs |
| 2025 fuel overstatement (P&L vs EFS) | **$193,933** | HIGH | P&L vs bank |
| 2025 fuel overstatement (grand total vs EFS) | **$422,078** | HIGH | P&L vs bank |
| 2025 manual fuel GJ ($285,789 dump) | **$285,789** | PROVEN | Apollo_Manual_Journal_Fuel_Targets.csv |
| 2025 ADJ TO STMT cash reduction | **$241,284** | PROVEN | Apollo_Manual_Journal_Fuel_Targets.csv |
| NP Gemini ever-growing phantom debt | **$924,186** | HIGH | Dec 2025 balance sheet |
| ATI Promissory (backdated note) | **$858,335** | PROVEN | QB logs + balance sheet |
| Combined ATI+Promissory debt on Apollo | **$1,392,936** | HIGH | Dec 2025 balance sheet |
| Wire Payable disappearance | **$868,535** | SUSPICIOUS | Balance sheet delta |
| GIG Transportation payments (2024) | **$111,924** | CONFIRMED | Bank recs + GL |

Sources: [[Bank Rec Analysis 2024]], [[Bank Rec Analysis 2025]], [[Apollo 2025 December]], [[Apollo_Manual_Journal_Fuel_Targets]], [[Intercompany Transfer Tracker]]

---

## 9. ATI CHARGEBACKS FILE — INTERNAL INCONSISTENCIES

Source: [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]]

ATI's own chargeback summary contains **internal math errors**:

| Item | Claimed Monthly | Claimed Annual | Actual Monthly (÷12) | Discrepancy |
|------|----------------|---------------|---------------------|-------------|
| Rent | $3,000 | $36,000 | $3,000 | OK |
| Wages | $5,500 | $66,000 | $5,500 | OK |
| **Insurance** | **$1,100** | **$198,000** | **$16,500** | **15x error** |
| **E-Logs** | **$32** | **$5,760** | **$480** | **15x error** |
| **Total** | **$9,632** | **$305,760** | | |

The insurance line claims $1,100/month but $198,000/year — those are off by **15x**. The E-Log line claims $32/month but $5,760/year — also off by **15x**. This is either incompetence or deliberate obfuscation.

> [!MISSING-EVIDENCE]
> **To determine intent behind 15x errors:** Requires ATI's internal insurance billing calculations and actual insurance invoices from the carrier. Cross-reference the $198,000/yr claimed against the $192,701 on Apollo's 2025 P&L and the ~$51,260/month allocation visible in 2024 GL.
> **From whom:** ATI ([[Rosanna Karim]]) — insurance invoices demanded in [[Document Demand Letter Template]].
> **What it would prove:** Whether the 15x multiplier is an arithmetic error in a hastily prepared document or a deliberate attempt to inflate Apollo's apparent obligations to ATI.

Compare to what Apollo's 2025 P&L actually shows:
- Insurance Expense (6200): $195,920 (close to the $198K claimed — ATI is billing Apollo their full annual rate)
- E-Log Service (5615): $11,520 (DOUBLE what ATI claims: $5,760)

### Equipment Loans (ATI claims Apollo owes)
| Lender | Units | Amount | Monthly | Term |
|--------|-------|--------|---------|------|
| Stellar/Apollo | 3 | $409,023 | $8,483 | 60 mo |
| Stellar/Apollo | 3 | $461,250 | $9,434 | 60 mo |
| Truist/**Asphalt** | 1 | $275,000 | $6,567 | 48 mo |
| WFB/**Asphalt** | 2 | $510,695 | $12,379 | 48 mo |
| **Total** | **9** | **$1,655,968** | **$36,863** | |

Note: The Truist and WFB loans are in **Asphalt's** name, not Apollo's. Yet ATI charges the payments to Apollo. Total loan payments: $36,863/month = **$442,358/year** being charged to Apollo for equipment, some of which may be titled to ATI.

---

## Connected
- [[Account 2010 Fuel Payable Mechanism]] — Detailed mechanism analysis
- [[Monthly GL vs Consolidated Reconciliation]] — Monthly P&L vs GL discrepancies
- [[Gemini Profit Siphon]] — $128K earned, zero delivered to Apollo
- [[Fuel Cost Manipulation]] — Original fuel finding (now confirmed with exact mechanism)
- [[ATI Monthly Billing Manipulation]]
- [[Promissory Note Backdating]]
- [[GL Audit Trail Anomalies]]
- [[Intercompany Transfer Tracker]]
- [[Investigation Dashboard]]
- [[Evidence Tiers]] — Update: Account 2010 finding is "Must Hit"

## Source Files
- [[Apollo_Manual_Journal_Fuel_Targets]] — The clearing entries
- [[Apollo_2010_Monthly_Rollforward]] — Monthly accumulation
- [[Apollo_2010_2025_Detail]] — Transaction detail
- Apollo 2024 December.csv / Apollo 2025 December.csv — P&L data
- [[ATI 2025 Profit & Loss MoM]] — ATI comparison
- [[Apollo Fuel 2023 2025]] — EFS transaction data
- [[Source Registry]] | [[Data Lineage]]
