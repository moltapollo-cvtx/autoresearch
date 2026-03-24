---
type: finding
status: documented
confidence: critical
tags: [finding, critical, bridge]
created: 2026-03-24
updated: 2026-03-24
related:
  - "[[Account 2010 Fuel Payable Mechanism]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[Bank Rec Analysis 2024]]"
  - "[[GL Audit Trail Anomalies]]"
evidence-refs:
  - "[[Apollo_Manual_Journal_Fuel_Targets]]"
  - "[[Apollo_2010_Monthly_Rollforward]]"
  - "[[Bank Rec Analysis 2024]]"
  - "[[Bank Rec Analysis 2025]]"
  - "[[DOC-QB-LOGS-2022-2026]]"
---

# Bridge: GL Manipulation → Bank Statement Evidence

> This note connects the **internal GL manipulation findings** (Account 2010, audit trail anomalies, backdated entries) to the **external bank statement evidence** (bank reconciliations, EFS payments, cash flow reconstruction).

---

## The Connection

The investigation has two independent evidence streams that converge on the same conclusion:

### Stream 1: Internal GL Evidence (ATI-controlled, manipulable)
- [[Account 2010 Fuel Payable Mechanism]] — $322,639 accumulated in 2024, then dumped as $285,789 fuel expense + $241,284 cash reduction on 2025-03-31
- [[GL Audit Trail Anomalies]] — 476-day backdated entry, 39.4% of Rosanna's entries backdated >30 days
- [[Fuel Cost Manipulation]] — $234,683 in 2023 fuel GJ entries with no supporting invoices
- [[Apollo_Manual_Journal_Fuel_Targets]] — The specific journal entries that executed the manipulation

### Stream 2: External Bank Evidence (independent, verified)
- [[Bank Rec Analysis 2024]] — $335,566 extracted, $0 returned, balance dropped from $365K to $62K
- [[Bank Rec Analysis 2025]] — $866,092 extracted, $285,771 returned, $241,284 "ADJ TO STMT" confirmed
- EFS bank payments: $705,265 (2024) + $506,492 (2025) = $1,211,757 actual fuel spend ([[Apollo Fuel 2023 2025]])

### Where They Meet

| GL Claim | Bank Reality | Match? |
|----------|-------------|--------|
| $241,284 "ADJ TO STMT" reduces cash (GL: 2025-03-31, posted 2025-06-18) | $241,284 appears as unexplained reduction in bank rec | YES — exact penny match |
| P&L fuel expense: $700,425 (2025) | EFS actual fuel: $506,492 (2025) | NO — $193,933 overstatement (38.3%) |
| P&L grand total fuel: $928,570 (2025) | EFS actual fuel: $506,492 (2025) | NO — $422,078 overstatement (83.3%) |
| $285,789 manual GJ labeled "fuel" | No corresponding EFS transaction | FABRICATED — no cash moved for this "fuel" |
| $335,566 ATI transfers out (2024 GL) | $335,566 confirmed in bank statements | YES — amounts match but no loan docs justify them |

---

## Why This Matters

The GL manipulation is **not just an accounting anomaly** — it has **real cash consequences** visible in bank statements that ATI cannot alter:

1. The $285,789 fuel dump inflates Apollo's recorded expenses, making Apollo appear less profitable
2. The $241,284 "ADJ TO STMT" actually reduced Apollo's bank balance — real money disappeared
3. The $1.2M in "paydowns" extracted from Apollo's bank account match GL transfer records
4. The bank evidence is **independent verification** — Stellar Bank records cannot be retroactively altered by ATI

**The internal manipulation creates the JUSTIFICATION for the external cash extraction.**

---

## Evidence Reliability Hierarchy
1. **Bank statements** (Stellar Bank) — independent, cannot be altered by ATI
2. **EFS fuel card records** — third-party, held by EFS
3. **IFTA government filings** — government-sworn, filed with state authorities
4. **QuickBooks transaction logs** — ATI-controlled but with timestamps that reveal backdating
5. **ATI-prepared P&L** — ATI-controlled, no audit trail, lowest reliability

See: [[Evidence Tiers]], [[Source Registry]]
