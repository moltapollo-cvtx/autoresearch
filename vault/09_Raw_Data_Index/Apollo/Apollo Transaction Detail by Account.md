---
tags: [source]
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
updated: 2026-03-24
---

# Apollo Energy Transaction Detail by Account

## File Details
- **Original filename:** `Apollo Transaction Detail by Account.csv`
- **File path:** `../../Apollo Transaction Detail by Account.csv`
- **Type:** csv
- **Entity:** [[Apollo Energy Resources LLC]]
- **Period covered:** Undetermined — see MISSING-EVIDENCE below

> [!MISSING-EVIDENCE] Period cannot be determined from filename
> Requires review of CSV headers or content to determine date range. Without date range, cannot determine which findings this transaction detail supports.

## Contents Summary
Detailed transaction listing organized by account for Apollo Energy. Provides granular transaction-level data for each GL account, useful for drilling into specific expense categories and identifying individual intercompany charges from ATI.

## Related Evidence
- [[GL Audit Trail Anomalies]]
- [[ATI GL 2023 - Intercompany Billing]]

## Related Findings
- [[ATI Monthly Billing Manipulation]]

## Cited In
- [[Monthly GL vs Consolidated Reconciliation]] — transaction-level detail used to verify individual account balances
- [[Account 2010 Fuel Payable Mechanism]] — Account 2010 activity drilled into at transaction level (undated; see MISSING-EVIDENCE note above)

## Chain of Custody
- **Indexed:** 2026-03-24
- **Analyzed in:** Pending analysis
- **Supports finding:** Pending
