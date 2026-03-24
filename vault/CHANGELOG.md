---
type: dashboard
tags: [dashboard]
created: 2026-03-24
updated: 2026-03-24
---

# Vault Changelog

> Every structural edit to the vault is logged here. Content edits within existing findings are not tracked here — only structural changes (new files, schema changes, link additions, config changes).

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
