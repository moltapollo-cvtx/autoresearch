---
tags: [source-file, apollo]
type: source
doc_id: SRC-APL-051
file_path: "../../Apollo Transaction Detail by Account.csv"
file_type: csv
entity: Apollo Energy Resources LLC
period:
date-range:
received_date:
sha256:
status: indexed
---

# Apollo Energy Transaction Detail by Account

## File Details
- **Original filename:** `Apollo Transaction Detail by Account.csv`
- **File path:** `../../Apollo Transaction Detail by Account.csv`
- **Type:** csv
- **Entity:** [[Apollo Energy Resources LLC]]
- **Period covered:** Unknown (requires review)

## Contents Summary
Detailed transaction listing organized by account for Apollo Energy. Provides granular transaction-level data for each GL account, useful for drilling into specific expense categories and identifying individual intercompany charges from ATI.

## Related Evidence
- [[GL Audit Trail Anomalies]]
- [[ATI GL 2023 - Intercompany Billing]]

## Related Findings
- [[ATI Monthly Billing Manipulation]]

> [!PROPOSAL] Potential evidence for additional findings
> This account-level transaction detail may support [[Account 2010 Fuel Payable Mechanism]] (drill into Account 2010 activity), [[Monthly GL vs Consolidated Reconciliation]] (verify individual account balances), and [[Revenue Timing Shift]] (identify timing of revenue recognition entries). Cross-reference recommended.

## Chain of Custody
- **Indexed:** 2026-03-24
- **Analyzed in:** Pending analysis
- **Supports finding:** Pending
