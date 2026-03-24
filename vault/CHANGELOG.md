---
type: dashboard
tags: [dashboard]
created: 2026-03-24
updated: 2026-03-24
---

# Vault Changelog

> Every structural edit to the vault is logged here. Content edits within existing findings are not tracked here — only structural changes (new files, schema changes, link additions, config changes).

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
