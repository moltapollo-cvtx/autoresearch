---
type: entity-company
tags: [entity, company]
status: confirmed
created: 2026-03-24
updated: 2026-03-24
related: ["[[Apollo Energy Resources LLC]]", "[[Fuel Cost Manipulation]]", "[[Fuel Spend Reconciliation]]", "[[Fuel Card Overview]]"]
---

# EFS LLC — Fuel Card Provider

## Role & Access
- **Type:** Third-party fuel card provider (independent of ATI)
- **Carrier ID served:** Apollo Energy Resources LLC (Carrier ID 5725124)
- **Cards managed:** 10 masked cards (*0040 through *0049) — see [[Fuel Card Overview]]
- **Data reliability:** HIGH — EFS records cannot be altered by ATI

## Evidentiary Significance

EFS LLC is a **critical independent data source** in this investigation. Because ATI has no audit trail on its accounting system, EFS fuel card records and the corresponding Stellar Bank payments to EFS provide the only independently verifiable fuel cost data.

### Key Data Points
| Period | Apollo Bank Payments to EFS | Source |
|---|---|---|
| 2024 (full year) | $705,265.28 | [[Bank Rec Analysis 2024]] |
| 2025 (Mar–Dec) | $506,491.82 | [[Bank Rec Analysis 2025]] |
| **Two-year total** | **$1,211,757.10** | [[Fuel Spend Reconciliation]] |

### The Fuel Overstatement
- ATI-prepared P&L reports Apollo's fuel cost at ~$720K (2024 est.) and $928,570 (2025 grand total)
- Actual cash paid to EFS: $705,265 (2024), $506,492 (2025)
- The 2025 discrepancy is **83.3% overstatement** — see [[Forensic Cross-Reference Report]]
- The mechanism: ATI posts fake "fuel" journal entries → inflates Apollo's debt → collects via "paydowns"

## Connected Findings
- [[Fuel Cost Manipulation]] — The $287K fuel gap finding
- [[Fuel Spend Reconciliation]] — Bank-level EFS payment reconciliation
- [[Account 2010 Fuel Payable Mechanism]] — How fuel overstatement is mechanized
- [[Forensic Cross-Reference Report]] — 83.3% overstatement quantified

## Connected Entities
- [[Apollo Energy Resources LLC]] — Customer account
- [[Stellar Bank]] — Payments flow from Apollo's Stellar Bank account to EFS

## Source Files
- [[Apollo Fuel 2023 2025]] — EFS fuel card data
- [[ATI Fuel 2023 2025]] | [[ATI FUEL 2024]] — ATI fuel records (for comparison)
- [[Source Registry]] | [[Data Lineage]]
