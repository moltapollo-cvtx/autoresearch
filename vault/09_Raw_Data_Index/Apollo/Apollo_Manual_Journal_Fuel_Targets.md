---
tags: [source-file, apollo, fuel, forensic-key]
type: source
doc_id: SRC-APL-057
file_path: "../../Apollo_Manual_Journal_Fuel_Targets.csv"
file_type: csv
entity: Apollo Energy Resources LLC
period: 2023 to 2025
date-range: 2023-01-01 to 2025-12-31
received_date:
sha256:
status: indexed
---

# Apollo Energy Manual Journal Entries - Fuel Targets

## File Details
- **Original filename:** `Apollo_Manual_Journal_Fuel_Targets.csv`
- **File path:** `../../Apollo_Manual_Journal_Fuel_Targets.csv`
- **Type:** csv
- **Entity:** [[Apollo Energy Resources LLC]]
- **Period covered:** Unknown (requires review)

## Contents Summary
**KEY EVIDENCE FILE.** Listing of manual journal entries targeting fuel-related accounts in Apollo Energy's books. This file documents deliberate manipulation of fuel cost allocations through manual journal entries rather than system-generated transactions. Each entry represents a conscious override of the normal accounting process, where someone manually debited fuel expense accounts and credited intercompany payable (Account 2010). The pattern of manual entries -- rather than automated fuel card imports -- is a primary indicator that fuel costs charged to Apollo were fabricated or inflated. Cross-reference against actual fuel card data to quantify the discrepancy between real fuel purchases and booked fuel expenses.

## Related Evidence
- [[Fuel Cost Manipulation]]
- [[Fuel Card Overview]]
- [[Fuel Spend Reconciliation]]
- [[GL Audit Trail Anomalies]]

## Related Findings
- [[Fuel Cost Manipulation]]
- [[ATI Monthly Billing Manipulation]]
- [[Account 2010 Fuel Payable Mechanism]]
- [[GL Audit Trail Anomalies]]

## Chain of Custody
- **Indexed:** 2026-03-24
- **Analyzed in:** [[Fuel Spend Reconciliation]]
- **Supports finding:** [[Fuel Cost Manipulation]]
