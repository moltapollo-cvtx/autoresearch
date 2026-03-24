---
tags: [finding, evidence, gl-entry, cash-flow]
status: documented
confidence: high
estimated_impact: "$510K+ claimed receivable"
direction: apollo-inflated
---

# ATI GL 2023 — N/R Apollo Energy Analysis

## Source: [[DOC-ATI-GL-2023]]

## Summary
ATI's "N/R Apollo Energy" account is the mechanism through which ATI builds a receivable against Apollo. In 2023, ATI debited $1,119,801 to this account (charges TO Apollo) and credited $609,729 (income applied FROM Apollo), leaving a year-end balance of **$510,072** that ATI claims Apollo owes.

---

## The Fuel Charging Mechanism — SMOKING GUN

ATI periodically debits "fuel" charges directly to Apollo's N/R account — NOT through the normal AP/AR cycle. These are journal entries, not invoices:

| Date | Description | Amount Charged |
|---|---|---|
| 04/28/2023 | fuel | $25,521 |
| 05/10/2023 | fuel | $44,452 |
| 06/13/2023 | fuel | $39,757 |
| 07/13/2023 | fuel | $62,382 |
| 08/16/2023 | fuel | $36,119 |
| 09/19/2023 | fuel | $26,452 |
| **Total** | | **$234,683** |

**This is the direct evidence of HOW the fuel overstatement works.** ATI takes a lump sum labeled "fuel" and debits it to Apollo's N/R. There are no invoices, no supporting detail, no breakdown of what fuel purchases these represent. Each entry is a single line, a single number, no reference to specific EFS transactions or IFTA data.

These entries stop after September 2023. Why? Possibly because the reporting structure changed or because 2024 uses a different mechanism — which we've already documented (the ~$287K gap between IFTA and P&L).

## Income Credits Applied

ATI also credits "income" to Apollo's N/R, reducing the receivable:

| Date | Amount |
|---|---|
| 02/28/2023 | $16,400 |
| 03/31/2023 | $36,984 |
| 04/28/2023 | $30,404 |
| 05/10/2023 | $85,861 |
| 06/13/2023 | $50,201 |
| 07/13/2023 | $159,247 |
| 08/16/2023 | $104,758 |
| **Total** | **$483,854** |

The income credits also stop in August 2023 — same timing as the fuel charges stopping.

## Net Fuel Impact
ATI charged $234,683 in fuel and credited $483,854 in income. But on the **same dates** as the fuel charges, ATI also debited numerous other items — payroll advances ($35K, $25K, $32K, $40K, $75K, $120K), equipment down payments ($140K, $153K), legal fees, 401k, etc. The net of ALL charges vs. ALL income credits left Apollo owing $510,072.

## The $293,750 in Equipment Loans
Two large entries stand out:
- 04/12/2023: "loan to Apollo for equip dwn pymt" — **$140,000**
- 04/27/2023: "advance to Apollo loan 2 dwn pymt" — **$153,750**

Total: $293,750 in equipment down payments. These are the likely foundation for the promissory note. See [[Promissory Note Backdating]].

## The $195,000 in "Advances"
- 06/13/2023: "payroll advance" — $32,000
- 06/23/2023: "payroll adv" — $25,000
- 07/01/2023: "payroll" — $35,000
- 07/19/2023: "advance bills and payroll" — $35,000
- 07/19/2023: "advance" — $22,500
- 08/09/2023: "advance" — $40,000
- 09/26/2023: "Apollo advance" — $75,000
- 09/28/2023: "Apollo advance OO settlement" — $120,000

Total advances: ~$384,500. These are labeled as ATI lending Apollo money. But Apollo was generating revenue (the income credits prove this). The question is whether these advances were necessary, or whether ATI was deliberately under-distributing Apollo's own revenue to create the appearance of indebtedness.

## Apollo Promissory Account — EMPTY
The "Apollo Promissory" account exists in the chart of accounts but has **ZERO transactions** in 2023. If the $858K promissory note was executed during 2023, it should have entries here. Its absence corroborates the backdating finding.

## Connected Findings
- [[Fuel Cost Manipulation]] — This GL data shows the EXACT mechanism: undocumented "fuel" journal entries
- [[Promissory Note Backdating]] — $293K in equipment loans likely underlie the note; Promissory account empty
- [[ATI GL 2023 - Intercompany Billing]] — Separate billing channel for services
- [[Intercompany Transfer Tracker]] — These 2023 charges became the "paydowns" extracted in 2024-2025
- [[GL Audit Trail Anomalies]] — Backdating pattern

## Source Files
- [[ATI GeneralLedger Report 2023]] — Raw data source (266,513 rows)
- [[Apollo QuickBooks LOGS 2022-2026]] — Apollo-side confirmation
- [[Source Registry]] | [[Data Lineage]]

## Entities
- [[Asphalt Transport Inc (ATI)]] | [[Apollo Energy Resources LLC]]
- [[Rosanna Karim]] — Posted 2 of 6 fuel entries | [[Cordee]] — Entry #1169
