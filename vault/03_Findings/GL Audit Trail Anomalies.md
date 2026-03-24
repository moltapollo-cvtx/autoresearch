---
tags: [finding]
status: documented
confidence: high
estimated_impact: varies
direction: both
---

# GL Audit Trail Anomalies

## Summary
Multiple anomalies in the general ledger point to systematic retroactive manipulation of Apollo's financial records.

## Key Anomalies

### 1. The 476-Day Retroactive Journal Entry
A journal entry was created that backdates an accounting event by **476 days** — over 15 months. This is not a timing difference or clerical error; it is a fundamental rewriting of historical financial records.

### 2. Bulk Same-Session Entry Pattern
[[Rosanna Karim]] is identified as the primary user making suspicious journal entries and bulk data modifications. The pattern of entering large batches of records in single sessions (see also [[Gemini Record Manipulation]]) indicates retrospective record construction rather than contemporaneous bookkeeping.

### 3. Other Flagged Users
System users **sknuckles**, **mcleod**, and **Martha** have been flagged for suspicious or anomalous activity in the audit trail. See [[Other Flagged Users]].

## The No-Audit-Trail Problem
The accounting system has **no audit trail enabled**. This means:
- Changes to journal entries leave no record
- The current data snapshot is the **only available audit record**
- Evidence preservation is urgent — any further modifications will overwrite the current state

## Recommended Protocols
- [x] SHA-256 hash all current data exports immediately — **DONE 03/23/2026**
  - Bank Rec PDF: `50f8c8bd63ff6f48dc71a0b0e4f6d01b1c8efde68759803584f03e3683908923`
  - QB Logs XLSM: `d918f3c9134d06e26fd2724abd8806c22090e5d8a3976f5f64e9a503ef9a0a82`
- [ ] Store copies in off-site encrypted storage
- [ ] Request that audit trail be enabled going forward (though this may alert subjects)
- [ ] Document the current state as the baseline for all future comparisons

---

## QB Transaction Log Confirmation (Added 03/23/2026)

Source: [[DOC-QB-LOGS-2022-2026]] — 26,993 transactions, Feb 2023–Apr 2025

### 476-Day Entry — CONFIRMED
Trans #1169: $26,451.77 "co driver fuel" — transaction date 09/20/2023, entered **01/08/2025 14:33** by **Cordee**. Credits NP ATI, debits Fuel Expense - Company. Simultaneously inflates Apollo's fuel cost AND increases Apollo's debt to ATI.

### Systematic Backdating by User
| User | Entries >30d lag | % of their entries | Avg lag | Max lag |
|---|---|---|---|---|
| Rosanna | 1,942 | 39.4% | 36 days | 300 days |
| Cordee | 1,417 | 12.1% | 18 days | 476 days |
| Admin | 159 | 5.6% | 18 days | 157 days |
| Mauree | 109 | 2.5% | 12 days | 117 days |
| Martha | 90 | 3.0% | 12 days | 82 days |
| Rikki | 79 | 71.2% | 57 days | 96 days |

**Rosanna** has the worst backdating profile: nearly 40% of all her entries were made more than 30 days after the supposed transaction date.

### General Journal Dominance
Rosanna controls **47.5%** of all General Journal entries (2,651 of 5,580). GJ entries bypass the normal AP/AR cycle and are the highest-manipulation-risk transaction type in the system.

### NEW: "Martha [Deleted User]" — 3,030 Entries
Martha's user account has been **deleted from the system** but 3,030 transactions remain attributed to them. Deleting a user account is itself a form of audit trail destruction — the person cannot be questioned about their entries through system-level identification.

### "Mauree" — 4,379 Entries (Not a Subject)
See [[Mauree]]. Third most active user in the system. **Assessment: incompetent, not malicious.** Entry pattern is routine fuel card settlements for named owner-operators. Does not touch intercompany accounts (NP ATI, NR Apollo) used in the manipulation mechanism.

## Source Files
- [[Apollo QuickBooks LOGS 2022-2026]] — Primary source (26,993 transactions, SHA: `d918f3c9...ef9a0a82`)
- [[Apollo Quickbooks Audit Trail 2023 to dec 2024]] — Supplementary audit trail
- [[Source Registry]] | [[Data Lineage]]
