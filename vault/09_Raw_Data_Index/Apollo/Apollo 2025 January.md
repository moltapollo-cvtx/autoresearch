---
tags: [source-file, apollo]
type: source
doc_id: SRC-APL-013
file_path: "../../Apollo 2025 January.csv"
file_type: csv
entity: Apollo Energy Resources LLC
period: 2025-01
date-range: 2025-01-01 to 2025-01-31
received_date:
sha256:
status: indexed
---

# Apollo Energy GL - January 2025

## File Details
- **Original filename:** `Apollo 2025 January.csv`
- **File path:** `../../Apollo 2025 January.csv`
- **Type:** csv
- **Entity:** [[Apollo Energy Resources LLC]]
- **Period covered:** January 2025

## Contents Summary
Monthly general ledger export for Apollo Energy, January 2025. Contains all journal entries, debits/credits, and account activity for the month.

## Related Evidence
- [[GL Audit Trail Anomalies]]

## Related Findings
- [[ATI Monthly Billing Manipulation]]

> [!PROPOSAL] Potential evidence for additional findings
> This source file may contain transaction-level detail supporting [[Account 2010 Fuel Payable Mechanism]] (clearing entries in 2025 that attempted to settle the inflated Account 2010 balance) or [[Forensic Cross-Reference Report]] (monthly verification of intercompany charges). Cross-reference recommended.

## Chain of Custody
- **Indexed:** 2026-03-24
- **Analyzed in:** [[Bank Rec Analysis 2025]]
- **Supports finding:** [[ATI Monthly Billing Manipulation]]
