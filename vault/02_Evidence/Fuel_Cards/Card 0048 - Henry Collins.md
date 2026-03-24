---
type: evidence
tags: [evidence, critical]
card_number: "*0048"
assigned_driver: "[[Henry Collins]]"
priority: critical
status: needs-verification
confidence: high
created: 2026-03-23
updated: 2026-03-24
related: ["[[Fuel Card Overview]]", "[[Henry Collins]]", "[[Fuel Cost Manipulation]]"]
---

# Card *0048 — Henry Collins

## Why This Card Matters
*0048 has the **highest spend** of all 10 masked fuel cards under Apollo's Carrier ID. It is assigned to [[Henry Collins]], a **terminated driver**. His termination date is the critical threshold: every dollar charged to this card after his departure is direct, unambiguous evidence of fraud.

## Status
- [ ] **CRITICAL:** Obtain Henry Collins' exact termination date
- [ ] Pull full transaction history from EFS
- [ ] Isolate all post-termination charges
- [ ] Identify all cash advance transactions
- [ ] Determine physical card custody chain after termination

## Analysis Framework
Once we have the termination date and transaction history:
1. Total charges before termination (baseline — legitimate use)
2. Total charges after termination (fraud indicator)
3. Cash advances (high fraud signal regardless of date)
4. Geographic analysis — where were charges made vs. where was the truck?
5. Frequency/pattern analysis — does usage pattern change after termination?

## Connected
- [[Fuel Card Overview]]
- [[Henry Collins]]
- [[Fuel Cost Manipulation]]
