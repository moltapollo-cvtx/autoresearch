---
tags: [dashboard, cash-flow]
status: active
updated: 2026-03-24
---

# Cash Flow Dashboard
> Track every dollar from source to destination. The core question: **Where did Apollo's money go?**

---

## The Headline Numbers

| Metric | Amount | Source |
|---|---|---|
| Net cash extracted by ATI (2024+2025) | **-$915,887** | Bank recs, verified |
| Gross cash sent to ATI (2024+2025) | **-$1,201,658** | Bank recs, verified |
| ATI/Gemini advances returned (2025 only) | +$285,771 | Bank recs, verified |
| GIG Transportation (suspected Gemini, 2024) | **-$111,924** | Bank recs, unconfirmed entity |
| Fuel overstatement (identified mechanism) | **-$287,000** est. | IFTA vs P&L cross-reference |
| Undocumented journal entries (2023 GL) | **-$234,683** | QB logs, confirmed |
| Unexplained "ADJ TO STMT" (Mar 2025) | **-$241,284** | Bank rec, unexplained |
| Undocumented "Ins/Elog" (Nov 2025) | **-$84,960** | Bank rec, no invoices |

---

## Balance Trajectory — The Drain

```
Jan 2024: $364,745  ████████████████████████████████████
Feb 2024: $230,501  ███████████████████████
Mar 2024: $214,427  █████████████████████
Apr 2024: $199,669  ████████████████████
May 2024: $126,015  █████████████
Jun 2024:  $50,921  █████
Jul 2024:   $8,903  █
Aug 2024:  $28,029  ███
Sep 2024:  $15,689  ██
Oct 2024:  $36,443  ████
Nov 2024: -$44,470  ████ NEGATIVE
Dec 2024:  $61,743  ██████
                    ... system transition ...
Mar 2025:  $27,813  ███
Apr 2025:  $50,029  █████
May 2025: -$21,197  ██ NEGATIVE
Jun 2025:  $69,911  ███████
Jul 2025:  $45,156  █████
Aug 2025:  $71,317  ███████
Sep 2025: $104,706  ███████████
Oct 2025: $125,095  █████████████
Nov 2025: $136,439  ██████████████
Dec 2025: $108,490  ███████████
```

**2024 pattern:** Steady drain from $365K to negative in 10 months.
**2025 pattern:** Oscillating with ATI advances propping it up, then massive extractions ($355K in October alone).

---

## The Fuel Gap

| Source                         | 2024             | 2025             | Can ATI Alter?        |
| ------------------------------ | ---------------- | ---------------- | --------------------- |
| EFS at bank (actual cash paid) | $705,265         | $506,492         | No — bank verified    |
| ATI-prepared P&L fuel          | ~$720K (est.)    | **NOT PROVIDED** | Yes — no audit trail  |
| IFTA filing                    | ~$433K (partial) | TBD              | No — government-sworn |
| **Implied overstatement**      | **~$287K**       | **TBD**          |                       |

The mechanism: ATI posts fake "fuel" journal entries → inflates Apollo's recorded debt → collects via "paydowns." See [[Fuel Cost Manipulation]], [[Fuel Spend Reconciliation]].

---

## Key Accounts

### Apollo — Stellar Bank (Acct 21920400 / GL 1000-00-00)
- **Controlled by:** [[Rosanna Karim]] — sole authorizer of all bank transfers out
- **Apollo's access:** None. Walker has no direct access to Apollo's own bank account.
- **2024 beginning balance:** $364,745 → ended year at $61,743 (83% decline)
- **2025 ending balance:** $108,490 (GL: $86,472 after adjustments)

### EFS Fuel Cards (Carrier ID 5725124)
- 10 masked cards: `*0040` through `*0049`
- See: [[Fuel Card Overview]]

---

## Cash Flow Categories Under Investigation

### 1. Direct ATI Extraction
- [[Intercompany Transfer Tracker]] — $1.2M gross, $916K net over two years
- [[Promissory Note Backdating]] — $858K note underlying the "paydowns" was backdated

### 2. Fuel Cost Inflation
- [[Fuel Cost Manipulation]] — The $287K gap
- [[Fuel Spend Reconciliation]] — Bank-level data now available for both years
- [[Fuel Card Overview]] — Card-level investigation

### 3. Undocumented Charges
- $241,284 "ADJ TO STMT" (03/31/2025) — unexplained
- $84,960 "Ins/Elog" (11/30/2025) — no supporting invoices
- [[ATI Monthly Billing Manipulation]] — Monthly charges modified upward

### 4. Revenue Manipulation
- [[Revenue Timing Shift]] — Systematic 1-month forward shift in 2024 data

### 5. Gemini Logistics
- [[Gemini Record Manipulation]] — 23 records mass-deleted
- GIG Transportation (2024): $112K — entity confirmation needed
- UCNG Gemini (2025): $20,880 pass-through confirmed

---

## Outstanding Items
- [ ] **URGENT:** 2025 ATI-prepared P&L (fuel line) — demand immediately
- [ ] **URGENT:** Itemized breakdown of $84,960 "Ins/Elog" charge
- [ ] **URGENT:** Documentation for $241,284 "ADJ TO STMT"
- [ ] **URGENT:** Loan/note docs justifying $866K in 2025 "paydowns"
- [ ] Confirm GIG Transportation Services entity identity (Gemini?)
- [ ] Obtain unaltered EFS portal exports
- [ ] Pull transaction reports for prioritized fuel cards (*0048, *0042)
- [ ] Obtain Henry Collins exact termination date
- [ ] Full-year ATI financials (2024 and 2025)
- [ ] Stellar Bank raw statements
- [ ] Volume discount agreements
- [ ] Insurance invoices, equipment lease agreements

---

## Source Files & Chain of Custody
- Bank Recs: [[Apollo Bank Rec Jan 2024]] through [[Apollo Bank Rec DEC 2024]], [[Apollo Bank Rec JAN 2025]], [[Apollo Bank Rec FEB 2025-QB]]
- [[Apollo Bank Recs 2025-TMS SYSTEM REPORT]] | [[Apollo bank transfers 2025]]
- [[Apollo QuickBooks LOGS 2022-2026]] | [[Apollo Fuel 2023 2025]]
- [[Apollo_Manual_Journal_Fuel_Targets]] — Suspicious: manual journal fuel targets
- See [[Source Registry]] | [[Data Lineage]] | [[Duplicate Tracker]]
