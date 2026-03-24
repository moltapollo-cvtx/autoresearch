---
type: finding
status: documented
confidence: high
tags: [finding, high]
created: 2026-03-23
updated: 2026-03-24
related:
  - "[[Gemini Profit Siphon]]"
  - "[[Gemini Logistics USA LLC]]"
  - "[[GL Audit Trail Anomalies]]"
evidence-refs:
  - "[[DOC-QB-LOGS-2022-2026]]"
  - "[[ATI GL 2023 - Gemini N-R Analysis]]"
  - "[[Bank Rec Analysis 2025]]"
dollar-amount: 282416
estimated_impact: 282416
direction: apollo-inflated
---

# Gemini Record Manipulation

## Summary
Two distinct acts of record manipulation involving [[Gemini Logistics USA LLC]]:

1. **Batch creation:** [[Rosanna Karim]] entered ALL Gemini liability records in a single session — not organically over time as transactions occurred. This means the entire Gemini intercompany ledger was constructed retrospectively.

2. **Mass deletion:** [[Cordee]] deleted 23 Gemini-related records in approximately 25 minutes. This is evidence destruction.

## Evidence
- Accounting system session logs show Rosanna's batch entry
- Same logs show Cordee's mass deletion within a narrow time window
- The combination — bulk creation followed by bulk deletion — suggests the records were created to serve a purpose and then removed when that purpose was fulfilled (or when discovery became a risk)

## Open Questions

> [!MISSING-EVIDENCE]
> **To determine value of 23 deleted Gemini records:** Requires QuickBooks database backup or transaction-level audit log from before the deletion event, covering [[Gemini Logistics USA LLC]] N/P entries. The backup must predate Cordee's ~25-minute deletion session. Without this, the total dollar value of the 23 deleted records cannot be determined. Confidence on deletion impact remains **low**.

> [!MISSING-EVIDENCE]
> **To determine who directed the deletion:** Requires internal communications (email, Slack, text) between [[Cordee]] and ATI management ([[Rosanna Karim]], [[Jimmy]]) in the period surrounding the deletion event. Subpoena or discovery request to ATI for all communications referencing "Gemini" records. Without this, the question of authorization remains open.

> [!MISSING-EVIDENCE]
> **To confirm Gemini's legal relationship to ATI:** Requires Gemini Logistics USA LLC articles of incorporation, operating agreement, and ownership records from the Texas Secretary of State (or state of formation). Cross-reference against ATI's corporate filings. Without this, the formal relationship cannot be established. Confidence remains **medium**.

## Connected
- [[Rosanna Karim]] — Created the records
- [[Cordee]] — Deleted the records
- [[Gemini Logistics USA LLC]]

---

## QB Log Confirmation (Added 03/23/2026)

Source: [[DOC-QB-LOGS-2022-2026]]

### N/P Gemini Batch Entries — Exact Amounts Confirmed
Rosanna entered three "reconciliation adj for brokered drivers and revenue" entries to N/P Gemini, all on **11/02/2023** in a single session:

| Trans# | Tx Date | Amount | Memo |
|---|---|---|---|
| 760 | 07/31/2023 | $17,974.00 | reconciliation adj for brokered drivers and revenue |
| 761 | 08/31/2023 | $122,751.66 | reconciliation adj for brokered drivers and revenue |
| 762 | 09/30/2023 | $141,690.72 | reconciliation adj for brokered drivers and revenue |
| **Total** | | **$282,416.38** | |

All three month-end dates, all entered in a single session on 11/02/2023. This is textbook retrospective record construction.

## Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — QB-side confirmation of batch entries + deletions
- Gemini monthly GL files: [[Gemini January 2024]] through [[Gemini December 2024]], [[Gemini 2025 January]] through [[Gemini 2025 December]]
- [[ATI GL 2023 - Gemini N-R Analysis]] — ATI-side Gemini intercompany analysis
- [[Source Registry]] | [[Data Lineage]]

### Bank Rec: UCNG Gemini Transaction — 11/12/2025
$20,879.82 labeled "UCNG Gemini Invs" flowed through Apollo's bank account in December 2025 reconciliation. Confirms Gemini continues to use Apollo as a pass-through for cash flows.

### Bank Rec: Gemini Invoice — 12/15/2025
$6,163.71 deposit labeled "Gemini Invoice" — money IN to Apollo from Gemini. Without the deleted records, the basis for this amount cannot be verified.
