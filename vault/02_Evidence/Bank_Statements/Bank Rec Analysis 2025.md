---
tags: [evidence, finding, bank-statement, cash-flow]
status: in-progress
confidence: high
---

# Bank Reconciliation Analysis — 2025

## Source
[[DOC-BankRec-2025-McLeod]] — 54-page detailed bank rec history, Stellar Bank account 1000-00-00, Feb–Dec 2025.

---

## Monthly Balance Trajectory

| Period | Stmt Balance | Adjusted Bank | GL Ending | Deposits | Payments | Adjustments |
|---|---|---|---|---|---|---|
| 03/31/2025 | $27,813 | $26,579 | $26,579 | $384,536 | $70,880 | ($338,844) |
| 04/30/2025 | $50,029 | ($42,904) | ($42,904) | $235,545 | $193,735 | ($111,293) |
| 05/31/2025 | ($21,197) | ($74,963) | ($74,963) | $215,677 | $175,324 | ($72,412) |
| 06/30/2025 | $69,911 | $65,080 | $65,080 | $309,077 | $133,550 | ($35,484) |
| 07/31/2025 | $45,156 | $27,508 | $27,508 | $356,119 | $248,769 | ($144,921) |
| 08/29/2025 | $71,317 | $29,302 | $29,302 | $298,251 | $188,343 | ($108,114) |
| 09/30/2025 | $104,706 | $55,393 | $55,393 | $353,087 | $230,754 | ($96,242) |
| 10/31/2025 | $125,095 | $100,770 | $100,770 | $738,528 | $199,404 | ($493,747) |
| 11/30/2025 | $136,439 | $106,946 | $106,946 | $266,197 | $153,008 | ($107,012) |
| 12/31/2025 | $108,490 | $86,472 | $86,472 | $420,203 | $218,657 | ($222,021) |

**Note:** Adjusted bank = GL ending in every period ($0.00 variance). This means the books are "reconciled" — but the question is whether the entries used to reconcile are legitimate.

---

## Critical Finding #1: Massive "Adjustments" Column

The "Plus adjustments" line in each reconciliation absorbs enormous sums. These are **not** normal bank reconciliation items:

| Period | Adjustments | Notes |
|---|---|---|
| March 2025 | ($338,844) | Includes "$241,284 ADJ TO STMT" — single journal entry |
| October 2025 | ($493,747) | Largest adjustment month — includes $230K ATI paydown + $125K loan paydown |
| December 2025 | ($222,021) | Includes $84,960 "Ins/Elog" + $50K ATI paydown |

The March 2025 **"ADJ TO STMT"** entry for **-$241,284.09** is particularly alarming. This is a single general journal adjustment on 03/31/2025 with no further description. It's the largest single non-payroll, non-intercompany entry in the entire report.

---

## Critical Finding #2: Intercompany Cash Flows

### Money IN to Apollo from ATI/Gemini
| Date | Description | Amount |
|---|---|---|
| 05/19/2025 | ADVANCE | $60,000 |
| 05/23/2025 | advance ATI | $45,000 |
| 06/03/2025 | advance gemini | $40,000 |
| 06/05/2025 | adv Gemini for Applied | $17,639 |
| 06/11/2025 | advance ATI for OD | $50,000 |
| 07/03/2025 | Gemini payment inv 0001160 | $4,789 |
| 07/03/2025 | ATI inv. paid to Apollo | $7,148 |
| 07/09/2025 | gemini invoices | $14,367 |
| 07/25/2025 | Gemini invoces | $19,803 |
| 07/28/2025 | payment for gemini invoice | $3,156 |
| 07/29/2025 | pament for ati invoices | $2,926 |
| 08/01/2025 | reversal overage ATI | $18,000 |
| 08/27/2025 | ATI inv. paid to Apollo | $1,472 |
| 08/28/2025 | ATI CHR INVOICE | $1,472 |
| **Total IN** | | **$285,771.49** |

### Money OUT from Apollo to ATI
| Date | Description | Amount |
|---|---|---|
| 06/17/2025 | ati paydown | ($90,000) |
| 06/30/2025 | paydown | ($60,000) |
| 08/01/2025 | Chr to Ati | ($18,000) |
| 08/06/2025 | paydown | ($33,000) |
| 08/15/2025 | note paydown | ($70,000) |
| 09/16/2025 | Payron ATI NP | ($40,000) |
| 09/22/2025 | paydown NP ATI | ($50,000) |
| 10/16/2025 | ATI paydown | ($230,000) |
| 10/31/2025 | loan paydown | ($125,000) |
| 11/19/2025 | paydown of NP ATI Auto | ($15,132) |
| 11/30/2025 | Ins/Elog | ($84,960) |
| 12/08/2025 | paydown ATI note | ($50,000) |
| **Total OUT** | | **$-866,091.76** |

### Net Flow
**$-580,320.27** — Apollo sent **$580,320.27 MORE to ATI than ATI sent to Apollo** during this period.

This is a critical number. Apollo is generating cash and ATI is extracting it as "note paydowns" and "paydowns." The underlying notes/loans that justify these paydowns need to be verified against the $858K backdated promissory note.

---

## Critical Finding #3: Duplicate Entry Patterns

Multiple instances of entries followed by immediate reversals and re-entries on the same date:
- 03/03/2025: Deposit $32,285.62 → Reverse → Re-enter same amount
- 04/01/2025: Two deposits voided and re-entered same day
- 04/02/2025: $4,695 deposit/reverse/re-enter
- 05/07/2025: $5,917.50 deposit/reverse/re-enter
- 05/23/2025: Multiple "DUPLICATE REMOVAL" entries (wages, fees, taxes)
- 06/01/2025: Payroll entered, reversed, re-entered, reversed again with "payroll reversal" entries
- 06/03/2025: $12,085 deposit/reverse/re-enter twice
- Multiple months show this pattern

This could be legitimate correction of data entry errors, **or** it could be a technique for obscuring the actual cash flow by creating noise in the transaction record.

---

## Critical Finding #4: EFS Fuel Payments — Actual Cash Outflow

Total EFS LLC payments from checks section (what Apollo *actually paid* for fuel):

| Month | EFS Payments |
|---|---|
| Mar 2025 | $35,890.90 |
| Apr 2025 | $33,354.26 |
| May 2025 | $38,045.84 |
| Jun 2025 | $54,578.12 |
| Jul 2025 | $60,295.85 |
| Aug 2025 | $71,078.01 |
| Sep 2025 | $62,538.87 |
| Oct 2025 | $65,552.52 |
| Nov 2025 | $41,392.27 |
| Dec 2025 | $43,765.18 |
| **Total** | **$506,491.82** |

**This is what Apollo actually paid EFS according to the bank.** Compare this to the ATI-prepared P&L fuel figure to quantify the overstatement for the 2025 period. The 2024 comparison showed a ~$287K gap — this data lets us extend that analysis.

---

## Critical Finding #5: Settlement Checks to Owner-Operators

Regular biweekly settlement checks to subcontractors. Key payees appearing throughout:
- **Anthony Coleman (ACOLEMAN)** — Every period, often 2 checks per period
- **Courtney Willams TRKG, LLC (CWILLAMS)** — Every period
- **Big Kat Trans LLC / JJOHNSON** — Every period (this is Jermaine Johnson — flagged for fuel card fraud-to-new-card pattern)
- **Remus Muresan (RMURESAN)** — Mar–Aug
- **Henson Fastrac Transport LLC (GHENSON)** — Jul–Nov
- **Espree Johnson Enterprises (PJOHNSON)** — Sep–Dec
- **John Ngugi (JNGUGI)** — Single appearance Aug

**Note on JJOHNSON:** Jermaine Johnson (Big Kat Trans LLC) was flagged in the fuel card investigation for being issued a new card after fraud was flagged on an old card. He receives settlement checks in every single month of this report.

---

## Critical Finding #6: Post Date Clustering

| Statement Date | Post Date | Lag (days) |
|---|---|---|
| 03/31/2025 | 06/18/2025 | 79 |
| 04/30/2025 | 06/18/2025 | 49 |
| 05/31/2025 | 06/19/2025 | 19 |
| 06/30/2025 | 07/15/2025 | 15 |
| 07/31/2025 | 08/20/2025 | 20 |
| 08/29/2025 | 09/18/2025 | 20 |
| 09/30/2025 | 10/14/2025 | 14 |
| 10/31/2025 | 11/20/2025 | 20 |
| 11/30/2025 | 12/08/2025 | 8 |
| 12/31/2025 | 01/15/2026 | 15 |

**March, April, and May 2025 were all reconciled within a 2-day window (June 18-19).** This is the same batch-processing pattern we've seen with the 12 monthly statements. The first quarter of bank recs was done retroactively in a batch.

---

## Action Items
- [ ] SHA-256 hash the source PDF immediately
- [ ] Cross-reference EFS check totals ($506,491.82) against ATI-reported fuel P&L for 2025
- [ ] Investigate the $241,284 "ADJ TO STMT" entry — what is this adjusting?
- [ ] Verify the underlying notes/loans that justify $866,091.76 in ATI paydowns
- [ ] Match Gemini transfers to [[Gemini Record Manipulation]] findings
- [ ] Request supporting documentation for the $84,960 "Ins/Elog" charge on 11/30/2025
- [ ] Cross-reference JJOHNSON settlement checks with fuel card activity

## Connected Findings
- [[Fuel Cost Manipulation]] — Now have actual bank-level EFS payment data for 2025
- [[Promissory Note Backdating]] — ATI paydowns reference "NP" (note payable)
- [[Gemini Record Manipulation]] — Gemini transfers visible in bank data
- [[Fuel Card Overview]] — EFS is the fuel card vendor; all fuel card payments flow through these checks
- [[Intercompany Transfer Tracker]] — Detailed breakdown

---

## Critical Finding #7: November Settlement Check Void/Re-Issue Pattern (Added 03/23/2026)

On 11/03/2025, settlement checks D0000295–D0000298 (ACOLEMAN $20,750.81, CWILLAMS $22,799.50, JJOHNSON $11,329.00, PJOHNSON $6,479.38) were all **voided the same day they were issued**, then re-issued as D0000299–D0000302 for identical or near-identical amounts.

**Total voided on that date: $61,458.69**

This void-and-reissue pattern creates offsetting credits that can be redirected. Need to trace whether the voided checks' GL credits were properly reversed or were used to absorb other charges.

---

## Critical Finding #8: December $0.00 Settlement Checks (Added 03/23/2026)

Four settlement checks on 12/15/2025 were issued for $0.00 or voided:
- D0000364 — ACOLEMAN — $0.00 (voided 12/15)
- D0000367 — PJOHNSON — $0.00 (voided 12/15)
- D0000368 — ACOLEMAN — $0.00
- D0000371 — PJOHNSON — $0.00

These drivers were supposedly settled but received nothing. If they hauled loads during this period, where did the settlement money go?

---

## Critical Finding #9: UCNG Gemini Transaction — $20,879.82 (Added 03/23/2026)

On 11/12/2025 (reconciled in December):
- DEP: (blank description) — **-$20,879.82** (reversal)
- DEP: "UCNG Gemini Invs" — **+$20,879.82**

This is Gemini revenue flowing through Apollo's bank account. "UCNG" likely references a specific customer or contract. Confirms Gemini-as-pass-through pattern. Cross-reference with the 23 mass-deleted Gemini records.

---

## Critical Finding #10: October 2025 Peak Extraction Month (Added 03/23/2026)

| Date | Description | Amount |
|---|---|---|
| 10/16/2025 | ATI paydown | -$230,000.00 |
| 10/31/2025 | loan paydown | -$125,000.00 |
| **Total Oct extraction** | | **-$355,000.00** |

October deposits totaled $738,528. ATI extracted **48% of all cash inflows** in a single month. This is the most aggressive extraction month in the dataset.

---

## Critical Finding #11: $84,960 "Ins/Elog" Charge — 11/30/2025 (Added 03/23/2026)

Single withdrawal labeled "Ins/Elog" for **$84,960.00**. This is the largest single non-paydown charge in the entire year. No breakdown between insurance and ELD services. No supporting invoices identified. This bundles two distinct cost categories into a single opaque charge — same obfuscation technique as intercompany billing.

**ACTION: Demand itemized breakdown with supporting invoices immediately.**
