---
tags: [dashboard, document]
updated: 2026-03-23
---

# Document Registry
> Every document received is logged here. This IS the audit trail that ATI's system doesn't provide.

---

## Why This Matters

ATI's accounting system has **no audit trail**. The only way to detect retroactive manipulation is to compare documents received at different points in time. If a YTD figure for a completed period changes between two submittals, that is **proof of retroactive journal entry manipulation**.

---

## Document Integrity Protocol

1. **Log every document immediately upon receipt** using [[Template - Document Receipt]]
2. **SHA-256 hash** the file upon receipt
3. **Store originals off-site** in encrypted storage
4. **Never overwrite** — new versions get new entries linked to prior version

### How to SHA-256 Hash a File
```bash
# macOS / Linux
shasum -a 256 filename.xlsx

# Windows PowerShell
Get-FileHash filename.xlsx -Algorithm SHA256
```

---

## Registry

| Doc ID | Document Name | Received | From | Generation Date | Hash (first 16) | Link |
|---|---|---|---|---|---|---|
| DOC-ATI-GL-2023 | ATI General Ledger 2023 | 2026-03-23 | unknown | unknown | PENDING | [[DOC-ATI-GL-2023]] |
| DOC-BANKREC-2025 | Bank Rec History (McLeod) | 2026-03-23 | McLeod (system) | 2026-03-22 13:17 | `50f8c8bd63ff6f48` | [[DOC-BankRec-2025-McLeod]] |
| DOC-QB-LOGS | Apollo QB Transaction Log 2022-2026 | 2026-03-23 | Walker (uploaded) | unknown | `d918f3c9134d06e2` | [[DOC-QB-LOGS-2022-2026]] |
| DOC-BANKREC-2024-JAN | Apollo Bank Rec Jan 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-FEB | Apollo Bank Rec Feb 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-MAR | Apollo Bank Rec Mar 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-APR | Apollo Bank Rec Apr 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-MAY | Apollo Bank Rec May 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-JUN | Apollo Bank Rec Jun 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-JUL | Apollo Bank Rec Jul 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-AUG | Apollo Bank Rec Aug 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-SEP1 | Apollo Bank Rec Sept 1 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-SEP30 | Apollo Bank Rec Sept 30 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-OCT | Apollo Bank Rec Oct 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-NOV | Apollo Bank Rec Nov 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |
| DOC-BANKREC-2024-DEC | Apollo Bank Rec Dec 2024 | 2026-03-23 | Walker (uploaded) | unknown | PENDING | [[Bank Rec Analysis 2024]] |

---

## File Inventory — 2024 Bank Recs

| Filename | Period | Format | Sheets |
|---|---|---|---|
| Apollo_Bank_Rec_Jan_2024.xlsm | Jan 2024 | .xlsm | JAN 2024 |
| Apollo_Bank_Rec_FEB_2024.xlsm | Feb 2024 | .xlsm | FEB 2024 |
| Apollo_Bank_Rec_MAR_2024.xlsm | Mar 2024 | .xlsm | MAR 2024 |
| Apollo_Bank_Rec_APR_2024.xlsm | Apr 2024 | .xlsm | APR 2024 |
| Apollo_Bank_Rec_MAY_2024.xlsm | May 2024 | .xlsm | MAY 2024 |
| Apollo_Bank_Rec_JUNE_2024.xlsm | Jun 2024 | .xlsm | JUNE 2024 |
| Apollo_Bank_Rec_JULY_2024.xlsm | Jul 2024 | .xlsm | JULY 2024 |
| Apollo_Bnak_Rec_AUG_2024.xlsm | Aug 2024 | .xlsm | Sheet1 |
| Apollo_Bank_Rec_Sept_1_2024.xlsm | Sep 1 2024 | .xlsm | SEPT 1 2024 |
| Apollo_Bank_Rec_SEPT_30-2024.xlsm | Sep 30 2024 | .xlsm | SEPT 30 2024 |
| Apollo_Bank_Rec_OCT_2024.xlsm | Oct 2024 | .xlsm | OCT 2024 |
| Apollo_Bank_Rec_NOV_2024.xlsm | Nov 2024 | .xlsm | NOV 2024 |
| Apollo_Bank_Rec_DEC_2024.xlsm | Dec 2024 | .xlsm | DEC 2024 |

**Note on format difference:** The 2024 files are QuickBooks-exported bank reconciliation reports (.xlsm with macros). The 2025 data is a McLeod-generated Bank Reconciliation History Report (PDF). Different format, same underlying account.

**Note on August filename:** "Apollo_B**n**ak_Rec_AUG_2024.xlsm" — typo in filename ("Bnak" instead of "Bank"). Evidence of hasty/careless file handling.

---

## Action Items
- [ ] SHA-256 hash all 13 2024 .xlsm files — **PENDING**
- [ ] Store all files in off-site encrypted storage
- [ ] Compare 2024 QB-exported bank recs against 2025 McLeod-generated report for any overlapping period discrepancies

---

## Red Flags Already Observed
- All 12 ATI monthly statements batch-printed on the same date
- Documents with generation timestamps inconsistent with events described
- Rosanna has provided only partial ATI financials despite repeated requests
- 2025 Q1 bank recs batch-reconciled retroactively (June 18-19, 2025)
- McLeod (flagged user) generated the 2025 bank rec report

---

## Pending
See: [[Outstanding Document Demands]]
