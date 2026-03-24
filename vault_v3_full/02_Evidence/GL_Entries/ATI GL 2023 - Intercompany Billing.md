---
tags: [finding, evidence, gl-entry]
status: documented
confidence: high
estimated_impact: "$311K invoiced"
direction: apollo-inflated
---

# ATI GL 2023 — Intercompany Billing Analysis

## Source: [[DOC-ATI-GL-2023]]

## Summary
ATI invoiced Apollo $311,173 through the Intercompany account in 2023. The billing was **batch-entered retroactively** — all entries carry a 09/01/2023 date, with a second batch on 09/22/2023 that covers "March - August" retroactively.

---

## The Billing Structure

### Monthly Services (from 09/01/2023 entries)
| Service | Monthly Rate |
|---|---|
| Prophesy (dispatch software) | $450 |
| QuickBooks | $118 |
| Back office services | $4,000 |
| Corp office services | $1,250 → $10,250 |
| Rent | $3,000 |
| Cell phone | $50 |
| ELD services | $4,784 |
| ELD monthly services | $192 |
| Insurance (GL, cargo, property) | $21,260 → adjusted to $15,000 |

### The Retroactive Batch (09/22/2023)
These entries cover months that had already passed:
- Telephone Feb–Aug: $350 ($50/mo × 7)
- Rent Mar–Aug: $18,000 ($3,000/mo × 6)
- Insurance Mar–Aug: **$127,561** ($21,260/mo × 6)
- Corp office Apr–Aug: $6,250 ($1,250/mo × 5)
- Back office services: $16,000 ($4,000/mo × 4)
- Prophesy: $1,350 ($450/mo × 3)

## Red Flags

### 1. Batch Entry Pattern
All intercompany invoices were entered on two dates: 09/01/2023 and 09/22/2023. No monthly billing was entered contemporaneously from January through August. This is the same retrospective record creation pattern seen in [[Gemini Record Manipulation]] and [[GL Audit Trail Anomalies]].

### 2. Corp Office Services Tripled
Corp office services started at $1,250/month, then jumped to $10,250/month with no explanation — an 8x increase. The September entries show both the original $1,250 AND a separate $9,000 entry, plus the retroactive $6,250 for Apr-Aug at the original rate.

### 3. Insurance Rate
$21,260/month ($255K/year) for GL, cargo, and property insurance. Then "adjusted per unit increase" to $15,000/month. The retroactive batch charges $127,561 for Mar-Aug at the original rate. Is this the actual insurance cost, or is ATI marking up the premium?

### 4. Interest Charge
On 11/30/2023: "Interest as of 11/30" — $1,932. ATI is charging Apollo **interest** on the intercompany balance. This means ATI inflates Apollo's costs, then charges interest on the resulting balance.

## Connected
- [[ATI Monthly Billing Manipulation]] — 2024 billing modifications follow this same pattern
- [[ATI GL 2023 - Apollo N-R Analysis]] — This billing is separate from the N/R fuel charges
