---
type: dashboard
tags: [dashboard]
created: 2026-03-24
updated: 2026-03-24
---

# Vault Changelog

> Every structural edit to the vault is logged here. Content edits within existing findings are not tracked here — only structural changes (new files, schema changes, link additions, config changes).

---

## 2026-03-24 — Vault Pass 4: Synthesis, Cross-Entity Analysis & Presentation Layer

### Summary
Pass 4 built the synthesis and presentation layer on top of the structured, citation-complete, placeholder-free vault from Passes 1-3. Created master narrative, cross-entity transaction mapping, evidence strength assessment, fuel fraud synthesis, upgraded meeting prep with actionable exhibits, and performed comprehensive tag normalization.

### P4-1: Master Narrative (NEW FILE)
- Created `00_Dashboard/Master Narrative.md` — the single note a reader should open first
- Core thesis in 2 sentences, 5 most critical proven findings with dollar amounts
- Complete mechanism explanation (how money moves from Apollo → ATI → unknown)
- Every actor named with role and wikilink
- Timeline arc: 2023 establishment → 2024 drain → 2025 escalation → 2026 investigation
- "What we still need" section linking to Open Questions and Outstanding Document Demands
- Dataview query pulling all CRITICAL-confidence findings
- Navigation hub linking to all dashboards, synthesis notes, and strategy files

### P4-2: Cross-Entity Transaction Map (NEW FILE)
- Created `04_Cash_Flow/Cross-Entity Transaction Map.md`
- Every documented money flow between entities, sorted chronologically
- Apollo → ATI: $1,201,658 in paydowns (2024: $335,566, 2025: $866,092)
- ATI → Apollo: $285,771 in advances (all 2025)
- Apollo → GIG: $111,924 in 9 settlement payments (Jan-May 2024)
- Gemini-related flows: $519K+ in customer "overpayments" credited to NP Gemini
- Fabricated debt entries: $1.9M+ in journal entries creating paper obligations
- Running totals by entity pair and year
- 5 [!SMOKING-GUN] callouts for largest transactions

### P4-3: Evidence Strength Matrix (NEW FILE)
- Created `06_Strategy/Evidence Strength Matrix.md`
- 12-row matrix assessing every finding: best evidence, evidence type, admissibility, ATI rebuttal potential, missing evidence, confidence
- "Bulletproof" tier: Net Cash Extraction, Account 2010 Mechanism, Fuel Overstatement
- "Strong" tier: Gemini Siphon, Record Manipulation, GL Anomalies, 2023 Fuel GJ
- "Needs Work" tier: Promissory Backdating, Revenue Timing, ATI Billing, GIG
- Evidence type legend with reliability ranking

### P4-4: Fuel Fraud Synthesis (NEW FILE)
- Created `03_Findings/SYNTHESIS - Fuel Fraud Complete Picture.md`
- Unified all 3 fuel fraud mechanisms: Account 2010 dump ($285,789), EFS/IFTA vs P&L gap ($422,078 in 2025), Card *0048 Henry Collins anomalies
- Interconnection diagram showing how mechanisms feed into each other
- Combined documented exposure: $656,761+ (non-overlapping)
- Year-by-year evolution: 2023 journal entries → 2024 accumulation → 2025 dump
- Evolving sophistication analysis

### P4-5: Grandparent Meeting Prep (REWRITTEN)
- Complete rewrite of `06_Strategy/Grandparent Meeting Prep.md`
- Opening statement: exact words Walker should say first
- Top 5 exhibits with sources, what each shows, why it's bulletproof, and format
- 6 anticipated pushback scenarios with specific counter-arguments
- 7 questions designed to force admissions or create documented contradictions
- Red lines table: 6 ATI claims that are demonstrably false with counter-evidence
- Closing ask: 6 specific requests from immediate to investment
- Meeting logistics (duration, materials, attendees, who NOT to invite)

### P4-6: Deliverables Index (UPGRADED)
- "Ready to Present" section: 8 findings with dollar impact, confidence, key source
- "Needs Work" section: 5 findings with specific gaps and what's needed
- "Draft Reports" section: 5 synthesis notes with status
- Active external documents table
- Planned deliverables with audience, format, estimated page count

### P4-7: Tag Audit & Graph Refinement (101 files modified)
- Audited all 162 markdown files for tag compliance
- Removed 16 non-controlled tags: `source-file` (→`source`), `apollo`, `gemini`, `ati`, `bank-rec`, `fuel`, `ifta`, `quickbooks`, `account-2010`, `chargebacks`, `cross-entity`, `strategy`, `chain-of-custody`, `cash-flow`, `deliverable`, `forensic-key` (→`critical`)
- 91 Raw Data Index files: tags normalized to `[source]` or `[source, critical]`
- 10 strategy/chain-of-custody/deliverable files: non-controlled tags removed
- graph.json updated: added 3 new color groups (synthesis=orange, bridge=teal, open-question=yellow), total 11 color groups

### P4-8: Final Polish
- Fixed 1 broken wikilink: `[[ATI]]` → `[[Asphalt Transport Inc (ATI)]]` in SYNTHESIS note
- Added `updated: 2026-03-24` to 91 Raw Data Index files (previously missing)
- Updated 2 files from `updated: 2026-03-23` to `2026-03-24`
- AUDIT.md rewritten to reflect post-Pass 4 state
- Verified: 154/155 wikilink targets resolve (155/155 after fix)

**New files created: 4 (Master Narrative, Cross-Entity Transaction Map, Evidence Strength Matrix, Fuel Fraud Synthesis)**
**Files rewritten: 3 (Grandparent Meeting Prep, Deliverables Index, AUDIT.md)**
**Files modified (tags/dates): ~101 (91 Raw Data Index + 10 other)**
**Total files affected: ~108**

---

## 2026-03-24 — Vault Pass 3: Zero-Tolerance Placeholder Sweep

### Summary
Systematic hunt-and-eliminate sweep of every vague placeholder in the vault. Every instance of "TBD", "unknown", "needs verification", "needs investigation", and generic `[!PROPOSAL]` callouts was either filled with concrete data from the vault or replaced with a specific `[!MISSING-EVIDENCE]` callout naming the exact document needed, who holds it, and what it would prove.

### Before/After Counts
- **TBD instances:** 18 → 0 (all resolved)
- **"unknown" placeholders:** 30+ → 0 actionable (5 remaining are: 1 template enum, 2 Dataview queries, 1 open question text, 1 counterargument context — all legitimate uses)
- **"needs verification/investigation":** 4 → 0
- **Generic `[!PROPOSAL]` callouts:** 77 → 0 (all replaced with specific `## Cited In` cross-references)
- **Total placeholders processed:** ~130

### P3-1: Filled from vault data (~119 instances)
- 81 Raw Data Index files: generic `[!PROPOSAL]` → specific `## Cited In` sections with exact finding links
- 5 Raw Data Index files: "Unknown (requires review)" → concrete periods or MISSING-EVIDENCE callouts
- Source Registry: 4 TBD periods → filled (3 "Undetermined" with rationale, 1 filled as "2023-2025")
- Cash Flow Dashboard: IFTA 2025 TBD → linked to source file; overstatement TBD → filled with $422,078 (83.3%)
- Fuel Spend Reconciliation: 2025 fuel GJ TBD → filled with $285,789 from [[Account 2010 Fuel Payable Mechanism]]
- Investigation Dashboard: 4 TBDs/needs → replaced with specific descriptions and awaiting-data statuses
- Gemini Record Manipulation: `estimated_impact: unknown` → 282416; `direction: unknown` → apollo-inflated
- ATI GL 2023 Gemini N-R Analysis: `direction: unknown` → apollo-inflated
- DOC-QB-LOGS: `generation_date: unknown` → QB export date range
- DOC-ATI-GL-2023: `received_from: unknown`, `generation_date: unknown` → filled with Rosanna Karim source + file description
- Document Registry: 16 "unknown" entries → replaced with specific document descriptions and SHA-256 action items
- Duplicate Tracker: 6 "Needs X" statuses → replaced with current analysis status (2 confirmed resolved, 4 pending with specific next steps)
- Entity files: Martha "Unknown title" → "Unidentified"; Cody "Unknown access" → "No QB activity detected"; McLeod "Unknown title" → "McLeod TMS confirmed software platform"
- Fuel Card Overview: 9 TBD driver assignments → "Unidentified"
- Master Timeline: "Unknown | Unknown" Gemini deletion → "Post-2023-11-02" with explanation
- Martha.md: `[!PROPOSAL]` → concrete LOW PRIORITY assessment

### P3-2: New [!MISSING-EVIDENCE] callouts created (11 total)
Each specifies the exact document needed, who holds it, and what it would prove:

1. **ATI Monthly Billing Manipulation** — Requires ATI intercompany billing invoices 2022-2025 showing original vs. modified monthly amounts
2. **Gemini Record Manipulation (deleted value)** — Requires QuickBooks database backup predating Cordee's deletion session
3. **Gemini Record Manipulation (deletion authorization)** — Requires internal communications between Cordee and ATI management
4. **Gemini Record Manipulation (legal relationship)** — Requires Gemini LLC articles of incorporation and operating agreement
5. **Document Registry (SHA-256)** — Requires SHA-256 hashing of all 13 2024 .xlsm files and ATI GL 2023
6. **APL GL work** — Requires workbook content review to determine date range
7. **Apollo Trial Balance** — Requires CSV content review for as-of date
8. **Apollo Transaction Detail by Account** — Requires CSV review for date range
9. **Fuel Card Overview** — Requires EFS account management report for Carrier ID 5725124 showing card-to-driver assignments
10. **Henry Collins** — Requires termination date from HR/payroll records + EFS transaction pull for card *0048
11. **Other Flagged Users (sknuckles)** — Requires QB transaction log filtered to user "sknuckles"

### P3-3: Open Questions Evidence Demand Matrix (new section)
- Added 17-row table to Open Questions.md mapping every open question to: resolving document, held by, and what it proves
- Enables targeted subpoena/discovery requests

### P3-4: Evidence Tiers Upgrade
- Converted all 5 tier sections from bullet lists to structured tables
- Every item now has: Dollar Impact, Finding link, Source Evidence link
- Items without source links flagged with "Awaiting [specific data]"

### P3-5: Duplicate Tracker Status Updates
- Overlap #4 (Sept bank recs): "Needs verification" → confirmed split-month reconciliation
- Overlap #7 (Apollo fuel sources): "Needs deep analysis" → CONFIRMED mechanism with cross-references
- Overlap #8 (Account 2010 files): "Needs analysis" → ANALYZED with full explanation + CRITICAL significance upgrade

**Total files modified: ~100+ (81 Raw Data Index + 13 Findings/Evidence + 5 Dashboards + 6 Entities + 3 Strategy + 2 Chain of Custody)**

---

## 2026-03-24 — Vault Pass 2: Deep Evidence Citation & Enrichment

### P2-1: Deep Evidence Citation (10 finding notes)
- Added inline `[[source-note]]` links next to every dollar figure in all 10 finding notes
- Expanded `evidence-refs` frontmatter arrays with ALL supporting sources (up to 11 refs per finding)
- Added `dollar-amount` to GL Audit Trail Anomalies ($26,452) and Gemini Record Manipulation ($282,416)
- Forensic Cross-Reference Report: 11 new source citations (Apollo 2024/2025 December, Apollo Fuel, IFTA, Manual Journal Targets, Chargebacks, Intercompany GL)
- Gemini Profit Siphon: 6 new evidence-refs (monthly Apollo/Gemini CSVs for balance verification)
- Monthly GL vs Consolidated Reconciliation: 8 new inline source citations + 1 new evidence-ref
- Fuel Cost Manipulation: inline citations for ~$720K (ATI P&L), ~$433K (IFTA), EFS card records
- Promissory Note Backdating: inline citation linking $858K to QB batch timestamp analysis

### P2-2: Raw Data Index Enrichment (91 files)
- Added `type: source` to all 91 stubs in 09_Raw_Data_Index/
- Added `date-range:` field (YYYY-MM-DD to YYYY-MM-DD format) to all 91 files
- Added `[!PROPOSAL]` callouts to 77 files suggesting cross-references to specific findings
- Enriched 5 forensic-key evidence files with `forensic-key` tag and detailed summaries:
  - Apollo_2010_2025_Detail, Apollo_2010_Monthly_Rollforward, Apollo_Manual_Journal_Fuel_Targets
  - Fuel_vs_Financials_Forensic_Report, WHAT ATI CLAIMS APOLLO OWES FROM 2025 CHARGEBACKS

### P2-3: Entity Relationship Mapping (17 files)
- Added `known-accounts` frontmatter arrays to all 11 People files
- Added `## Known Accounts` and `## Key Transactions` sections to 6 major people (Rosanna, Cordee, Jimmy, Henry, Walker, James Luhr Jr)
- Added `total-extracted`/`total-received` numeric fields to all 6 Company files
- Added `key-accounts` arrays to all Company files (bank accounts, GL accounts, carrier IDs)
- Added `related-entities` arrays to ATI, Gemini, GIG, EFS, Stellar Bank
- Apollo: 7-row Key Accounts table (Stellar Bank, EFS, GL 1000/2010/2410/2420/2430)

### P2-4: Master Timeline Enrichment
- Added Dataview auto-pull query for timeline events at top
- Reorganized chronologically: 2023 → 2024 → 2025 (was out of order)
- Standardized ALL dates to YYYY-MM-DD format
- Added dollar amounts to every transaction event (was missing on ~8 entries)
- Added `[[source-note]]` links to every event (replaced "Jan 2024 Bank Rec" with `[[Apollo Bank Rec Jan 2024]]`)
- Added 12 new events: Gemini batch entries, MES overpayments, Sapphire Gas, NP Gemini year-end spike, Account 2010 clearing entries, April/July fuel reclasses, Gemini invoice, Cordee 476-day entry
- Updated Investigation Milestones with 5 new entries (Account 2010 discovery, Gemini Siphon, Cross-Reference Report, Pass 1, Pass 2)
- Populated `evidence-refs` frontmatter (was empty)

### P2-5: Open Questions Note (NEW FILE)
- Created `06_Strategy/Open Questions.md` with 17 tracked questions
- 4 Critical (blocks key findings): paydown justification, Wire Payable disappearance, 2025 P&L, Ins/Elog breakdown
- 5 High (affects scope): GIG entity, deleted records value, Cordee direction, Gemini legal relationship, Collins termination
- 8 Medium (refines understanding): insurance allocation, RE gap, depreciation, Gemini RE anomaly, chargebacks 15x error, equipment loans, billing overcharge, revenue timing
- 3 Resolved with dates and sources
- Dataview query for auto-detecting unresolved items in vault

### P2-6: Cash Flow Dashboard Upgrade
- Added "SMOKING GUNS" section with 4 callouts (Account 2010 $527K, Net Extraction $916K, Gemini Siphon $341K, October 48%)
- Added "Running Totals by Entity" table (ATI in/out, GIG, Gemini, EFS by year with totals)
- Added Dataview "Entity Totals" query pulling from company total-extracted/total-received fields
- Enhanced headline numbers table: added 4 new rows (2025 fuel overstatement $422K, manual GJ $286K, Gemini trapped profits $128K, NP Gemini growth $213K)
- All source references upgraded from plain text to `[[wikilinks]]`

### P2-7: Bridge Notes (3 NEW FILES)
- `Bridge - GL Manipulation to Bank Evidence.md` — Connects GL entries to independent bank verification; evidence reliability hierarchy
- `Bridge - Gemini Siphon to Intercompany Transfers.md` — Connects phantom debt growth to physical cash extraction; GIG connection analysis
- `Bridge - Backdating Pattern to Financial Impact.md` — Complete backdating→dollar map ($1.9M+ quantified); escalation analysis

### P2-8: CSS & Graph Polish
- Added 3 new callout styles: `[!TIMELINE]` (cyan), `[!ENTITY]` (purple), `[!BRIDGE]` (teal)
- Added tag color styling for `#bridge`, `#open-question`, `#strategy`
- Added 6 graph view node colors: bridge, strategy, open-question, dashboard, source-file, forensic-key
- Added Dataview table styling (matching forensic theme: gold headers, hover effects)

### P2-9: Navigation Updates
- Updated MOC-Master with Bridge Notes section, Open Questions link, enriched Raw Data Index counts
- Updated evidence-refs on Master Timeline (was empty array)

**Total files modified: ~130+ (91 Raw Data Index + 10 findings + 17 entities + 4 dashboards + 4 new files + CSS + MOC)**

---

## 2026-03-24 — Vault Improvement Pass (Automated)

### Pass 1: Audit & Inventory
- Read all ~120 vault files
- Created `AUDIT.md` with comprehensive findings
- Identified: frontmatter inconsistencies, 5 missing entity notes, tag sprawl, empty graph config, no CSS theme, no Dataview queries

### Pass 2: Frontmatter Normalization (50+ files edited)
- Added `type:` field to all notes (finding, evidence, entity-person, entity-company, dashboard, source, cash-flow, strategy, chain-of-custody, deliverable)
- Added `created:` and `updated:` dates to all notes
- Added `related:` arrays with wikilinks to connected notes
- Added `evidence-refs:` arrays linking findings to source files
- Added `dollar-amount:` numeric field to findings and evidence notes (enables Dataview aggregation)
- Added `confidence:` tags (#critical, #high, #medium, #low) to relevant notes
- Normalized `tags:` to controlled vocabulary
- Fixed DOC-BankRec-2025-McLeod `received_date` typo (2025 → 2026)

**Files modified:**
- 4 dashboards (00_Dashboard/)
- 4 entity-company notes (01_Entities/Companies/)
- 8 entity-person notes (01_Entities/People/)
- 8 evidence notes (02_Evidence/)
- 10 finding notes (03_Findings/)
- 2 cash flow notes (04_Cash_Flow/)
- 3 chain of custody notes (05_Chain_of_Custody/)
- 3 strategy notes (06_Strategy/)
- 1 deliverable note (08_Deliverables/)

### Pass 3: New Entity Notes (5 files created)
- `01_Entities/People/Walker.md` — Apollo owner, investigation principal
- `01_Entities/Companies/GIG Transportation Services.md` — Suspected Gemini affiliate ($111,924)
- `01_Entities/Companies/EFS LLC.md` — Independent fuel card provider ($1.2M payments)
- `01_Entities/People/Martha.md` — Deleted QB user (3,030 entries)
- `01_Entities/People/McLeod.md` — System user (bank rec generator)

### Pass 4: Evidence Citations
- Added inline `[[source]]` links to $241,284 "ADJ TO STMT" → [[Account 2010 Fuel Payable Mechanism]]
- Added inline `[[source]]` links to $84,960 "Ins/Elog" → [[Bank Rec Analysis 2025]]
- Added `[[GIG Transportation Services]]` entity link in Cash Flow Dashboard
- Added `[[EFS LLC]]` to Investigation Dashboard entity map

### Pass 5: Dashboard Improvements
- **Investigation Dashboard:** Added 4 Dataview query blocks (findings by confidence, total dollar impact, open questions, all entities)
- **Cash Flow Dashboard:** Added 2 Dataview query blocks (cash flow findings, evidence with dollar amounts)
- **Document Registry:** Added 2 Dataview query blocks (all source files by entity, documents missing SHA-256)
- Updated Tags Reference to match controlled vocabulary
- Added session log entry for this improvement pass

### Pass 6: Graph Layer & Navigation
- **graph.json:** Added 8 color groups (finding=gold, evidence=blue, person=pink, company=purple, source=teal, timeline=cyan, critical=red, dashboard=amber), enabled arrows, increased node size
- **MOC-Master.md:** Created master Map of Content linking every cluster — entities, findings, evidence, cash flow, chain of custody, strategy, raw data index, graph narratives
- **Evidence Bridge - Sources to Findings.md:** Bridge note mapping which raw sources support which findings, with evidence reliability hierarchy and Dataview query for unlinked sources

### Pass 7: Visual Polish
- **vault-theme.css:** Created forensic investigation theme with:
  - Custom callouts: `[!FINDING]`, `[!CRITICAL]`, `[!EVIDENCE]`, `[!PROPOSAL]`, `[!OPEN-QUESTION]`, `[!SMOKING-GUN]`
  - Confidence-level tag color coding (critical=red, high=orange, medium=yellow, low=green)
  - Gold/amber accent table headers and headings
  - Graph view node colors by type
- **app.json:** Configured sensible defaults (enabled snippets, frontmatter visible, inline titles, auto-update links)
- **Templates (8 files):** Updated all templates to use normalized frontmatter schema with `type:`, `created:`, `updated:`, `related:`, `evidence-refs:`, `dollar-amount:` fields

### Pass 8: Cleanup
- Removed empty `Untitled.md` and `Untitled.canvas`
- Fixed `README.md` — updated folder structure (05_Timeline → 05_Chain_of_Custody, added 09_Raw_Data_Index)
- Enriched `Cody.md` with proper role & access section
- Created this `CHANGELOG.md`

---

## 2026-03-24 — Vault Restructure (Manual)

- Created `05_Chain_of_Custody/` with Source Registry, Data Lineage, Duplicate Tracker
- Created `09_Raw_Data_Index/` with ~90 source file index notes (ATI, Apollo, Gemini)
- Cross-linked all findings to source files
- Downgraded Mauree and Martha to non-subjects

## 2026-03-23 — 2024 Bank Rec Ingestion

- Ingested 13 .xlsm bank reconciliation files (Jan–Dec 2024)
- Created Bank Rec Analysis 2024
- Two-year cash flow reconstruction completed
- ATI extraction quantified: $1.2M gross / $916K net
- GIG Transportation entity flagged ($112K)

## 2026-03-23 — QB Log Forensic Analysis

- Analyzed QB Transaction Log (26,993 rows)
- Bank Rec 2025 PDF verified and SHA-256 hashed
- Confirmed all prior findings from primary source data
- 5 new bank rec findings identified
- Mauree downgraded to non-subject

## Initial — Vault v1

- Initial vault creation
- All findings backfilled to date
