---
type: strategy
status: active
tags: [open-question]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Investigation Dashboard]]"
  - "[[Evidence Tiers]]"
  - "[[Outstanding Document Demands]]"
---

# Open Questions — Investigation Tracker

> Every unresolved question in the vault, organized by status and linked to findings. Use `[!OPEN-QUESTION]` callouts in other notes to feed this list.

## Dataview: All Open Questions from Vault

```dataview
LIST
FROM ""
WHERE contains(text, "needs investigation") OR contains(text, "TBD") OR contains(text, "unknown") OR contains(text, "unconfirmed")
SORT file.name ASC
```

---

## Critical — Blocks Key Findings

| # | Question | Status | Related Finding | Related Demand |
|---|----------|--------|----------------|----------------|
| Q1 | What documents/notes justify $1,201,658 in cumulative ATI "paydowns" from Apollo? Only documented basis is the $858K promissory note, which is proven backdated. | open | [[Intercompany Transfer Tracker]], [[Promissory Note Backdating]] | [[Outstanding Document Demands]] |
| Q2 | Where did the $868,535 in Wire Payable (account 2011) go? Collapsed from $870K to $1.4K between Dec 2024 and Dec 2025. Most likely reclassified to ATI Promissory (2430). | open | [[Forensic Cross-Reference Report]] | — |
| Q3 | What is the 2025 ATI-prepared P&L fuel line for Apollo? Without this, the 2025 fuel gap cannot be calculated against ATI's own numbers. | open | [[Fuel Cost Manipulation]], [[Fuel Spend Reconciliation]] | [[Outstanding Document Demands]] |
| Q4 | What is the itemized breakdown of the $84,960 "Ins/Elog" charge on 2025-11-30? No supporting invoices exist. | open | [[Bank Rec Analysis 2025]], [[Cash Flow Dashboard]] | [[Outstanding Document Demands]] |

---

## High — Affects Investigation Scope

| # | Question | Status | Related Finding |
|---|----------|--------|----------------|
| Q5 | Is GIG Transportation Services a Gemini affiliate? $111,924 paid from Apollo in biweekly patterns (Jan–May 2024), and GIG appears in EFS fuel card payables as "GIGTRANSPORTATIONSER." | investigating | [[GIG Transportation Services]], [[Forensic Cross-Reference Report]] |
| Q6 | What was the total dollar value of the 23 Gemini records mass-deleted by Cordee? The records were created by Rosanna and then destroyed — content unknown. | open | [[Gemini Record Manipulation]] |
| Q7 | Was Cordee directed to delete the 23 Gemini records, and if so, by whom? | open | [[Gemini Record Manipulation]], [[Cordee]] |
| Q8 | What is Gemini's formal legal relationship to ATI? Subsidiary? Affiliate? Joint venture? | open | [[Gemini Logistics USA LLC]], [[Gemini Profit Siphon]] |
| Q9 | What is the exact termination date for Henry Collins? Post-termination fuel card charges on *0048 cannot be quantified without this. | open | [[Henry Collins]], [[Card 0048 - Henry Collins]] |

---

## Medium — Refines Understanding

| # | Question | Status | Related Finding |
|---|----------|--------|----------------|
| Q10 | Why did insurance allocation (account 6200) stop abruptly in Nov–Dec 2024 after 10 months at exactly $51,260.09/month? | open | [[Monthly GL vs Consolidated Reconciliation]] |
| Q11 | Why does the GL show $8,669 more in losses than the P&L computes for FY2024? (Retained Earnings gap) | open | [[Monthly GL vs Consolidated Reconciliation]] |
| Q12 | Why is December 2024 depreciation ($20,999) absent from GL Accumulated Depreciation but present in P&L? | open | [[Monthly GL vs Consolidated Reconciliation]] |
| Q13 | How were Gemini's retained earnings reduced by $55,460 despite $127,964 in net income? ~$183K removed via unidentified adjustments. | open | [[Gemini Profit Siphon]] |
| Q14 | What explains ATI's own $198K insurance claim vs $1,100/month (15x error) in the chargebacks document? Incompetence or obfuscation? | open | [[Forensic Cross-Reference Report]], [[WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS]] |
| Q15 | Are the Truist and WFB equipment loans ($785K) in ATI's name being charged to Apollo? Total: $36,863/month = $442K/year. | open | [[Forensic Cross-Reference Report]] |
| Q16 | What is the total overcharge from ATI's variable-to-fixed billing modification? Needs quantification across all months. | open | [[ATI Monthly Billing Manipulation]] |
| Q17 | Does the revenue timing shift pattern hold across all 12 months of 2024? APL_GL_Comparison_Report.xlsx was interrupted. | open | [[Revenue Timing Shift]] |

---

## Resolved

| # | Question | Resolution | Date | Source |
|---|----------|-----------|------|--------|
| R1 | What is the "$241,284 ADJ TO STMT" entry? | Part of Account 2010 clearing — reduced cash while zeroing fuel payable. 79-day backdated. | 2026-03-24 | [[Account 2010 Fuel Payable Mechanism]] |
| R2 | How does the fuel overstatement mechanism work in 2025? | Account 2010 accumulated $323K in 2024, then dumped $286K into Fuel Expense on 2025-03-31 via manual GJ. | 2026-03-24 | [[Account 2010 Fuel Payable Mechanism]] |
| R3 | Do Gemini profits flow to Apollo? | No. $127,964 earned over 24 months, zero distributed. NR Apollo grew by $213K — more than Gemini earned. | 2026-03-24 | [[Gemini Profit Siphon]] |

---

## Evidence Demand Matrix — What Document Resolves Each Question

| Question | Resolving Document | Held By | Proves |
|----------|--------------------|---------|--------|
| Q1 (paydown justification) | Intercompany loan agreements, promissory notes, board resolutions for all ATI-Apollo transfers 2024-2025 | ATI (Rosanna Karim / James Luhr Jr) | Whether $1.2M in "paydowns" had legal basis beyond the backdated $858K note |
| Q2 (Wire Payable $868K) | Apollo GL journal entry detail for account 2011 covering Dec 2024–Dec 2025, showing reclassification entries | ATI (controls Apollo's QB) | Where $868,535 was reclassified — likely to ATI Promissory (2430) |
| Q3 (2025 P&L fuel line) | ATI-prepared Apollo Energy P&L for FY2025, showing 5500/5310/5520 account detail | ATI (Rosanna Karim) | 2025 fuel overstatement calculated against ATI's own numbers |
| Q4 ($84,960 Ins/Elog) | Itemized invoices comprising the $84,960 "Ins/Elog" charge posted 2025-11-30 | ATI (Rosanna Karim) | Whether the charge is legitimate insurance + e-log costs or fabricated |
| Q5 (GIG = Gemini?) | GIG Transportation Services LLC articles of incorporation and ownership records; EFS carrier management records for GIG | Texas Secretary of State; EFS LLC | Whether GIG shares ownership with Gemini/ATI — if yes, $112K is additional siphon |
| Q6 (deleted Gemini value) | QuickBooks database backup predating Cordee's deletion session | ATI (controls QB system) | Total dollar value of 23 deleted Gemini records |
| Q7 (deletion authorization) | Internal communications (email/Slack/text) between Cordee and ATI management re: Gemini records | ATI (subpoena/discovery) | Whether Cordee acted on ATI direction to destroy evidence |
| Q8 (Gemini legal status) | Gemini Logistics USA LLC operating agreement, articles of incorporation, ownership records | Texas Secretary of State | ATI's control relationship — determines if Gemini debt is self-dealing |
| Q9 (Collins termination date) | Apollo Energy HR/payroll records showing Henry Collins' last day of employment | Walker (Apollo) or ATI payroll | Enables calculation of post-termination fraud on card *0048 |
| Q10 (insurance stop) | Insurance allocation policy and Nov/Dec 2024 GL entries for account 6200 | ATI (Rosanna Karim) | Whether ~$102,520 in missing insurance allocation was diverted |
| Q11 (RE gap $8,669) | December 2024 closing journal entries and prior-year adjustments | ATI (controls QB) | Whether the $8,669 gap is a closing error or intentional manipulation |
| Q12 (Dec depreciation) | December 2024 depreciation journal entry (or absence thereof) in GL | ATI (controls QB) | Whether $20,999 was intentionally omitted from GL |
| Q13 (Gemini RE decrease) | Gemini 2024-2025 adjusting journal entries affecting retained earnings | ATI (controls Gemini books) | Where ~$183K in Gemini equity went — potential distribution to ATI |
| Q14 (15x chargeback error) | ATI internal insurance billing calculations; actual insurance invoices | ATI (Rosanna Karim) | Whether 15x multiplier is arithmetic error or intentional inflation |
| Q15 (equipment loans) | Truist and WFB loan agreements for 3 equipment units ($785K) | ATI (James Luhr Jr / Rosanna Karim) | Whether loans in ATI's name are being passed through to Apollo at markup |
| Q16 (billing overcharge) | ATI monthly intercompany billing invoices to Apollo 2022-2025 | ATI (Rosanna Karim) | Total overcharge from variable-to-fixed billing modification |
| Q17 (revenue timing) | Completed APL_GL_Comparison_Report.xlsx — monthly revenue comparison across all 12 months 2024 | Investigation team (in progress) | Whether revenue timing shift is systematic or isolated |

---

## Source Files
- [[Investigation Dashboard]] — Master finding list
- [[Evidence Tiers]] — Presentation priority
- [[Outstanding Document Demands]] — Documents needed to resolve open questions
