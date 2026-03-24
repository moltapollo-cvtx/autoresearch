---
type: dashboard
status: completed
created: 2026-03-24
updated: 2026-03-24
tags: [dashboard]
---

# Vault Audit Report — 2026-03-24

> Systematic audit of all ~120 files in the Apollo Investigation Vault.

---

## Vault Statistics

| Metric | Count |
|---|---|
| Total markdown files | ~120 |
| Folders | 10 (00–09) + .obsidian + root |
| Dashboard notes | 4 |
| Entity notes (people) | 8 |
| Entity notes (companies) | 4 |
| Evidence notes | 10 |
| Finding notes | 10 |
| Cash flow notes | 2 |
| Chain of custody notes | 3 |
| Strategy notes | 3 |
| Templates | 8 |
| Deliverables | 1 |
| Raw data index notes | ~90 (ATI: 7, Apollo: ~55, Gemini: 24) |
| Root files (README, Untitled) | 2 |

---

## Issues Found

### CRITICAL — Frontmatter Schema Inconsistency
- **No `type:` field** on any note — uses `tags:` array as a proxy
- **No `confidence:` field** as frontmatter property (only in some findings as text)
- **No `related:` or `evidence-refs:` arrays** in frontmatter
- **No `dollar-amount:` numeric field** for Dataview queries
- **Missing `created:` dates** on most notes
- **Missing `updated:` dates** on ~60% of notes

### HIGH — Missing Entity Notes
| Entity | Mentions | Has Note? |
|---|---|---|
| Walker (Apollo owner) | 15+ | NO |
| GIG Transportation Services | 5+ | NO |
| Martha (deleted QB user) | 5+ | NO |
| EFS LLC (fuel card provider) | 20+ | NO |
| McLeod (system user) | 3+ | NO |

### HIGH — Tag Sprawl
**Current tags in use (uncontrolled):**
- `#source-file`, `#ati`, `#apollo`, `#gemini` — entity-specific, not in controlled vocab
- `#document`, `#bank-statement`, `#fuel-card`, `#gl-entry` — sub-types, not standardized
- `#action-needed`, `#strategy`, `#deliverable`, `#chain-of-custody` — outside controlled vocab
- `#cash-flow`, `#action-taken`, `#journal` — inconsistent usage

**Should be normalized to:** `#finding`, `#evidence`, `#entity`, `#source`, `#timeline`, `#person`, `#company`, `#open-question`, `#critical`, `#high`, `#medium`, `#low`

### HIGH — Graph Configuration Empty
- graph.json has basic layout settings but NO saved filter groups
- No color groups for the 6 named narratives
- No CSS snippets directory or vault theme

### MEDIUM — Missing Structural Files
| File | Purpose | Status |
|---|---|---|
| CHANGELOG.md | Track all vault edits | MISSING |
| MOC-Master.md | Map of Content hub | MISSING |
| .obsidian/snippets/vault-theme.css | Visual forensic theme | MISSING |
| Dataview queries in dashboards | Live stats | NOT IMPLEMENTED |

### MEDIUM — Weak/Orphan Notes
| Note | Issue |
|---|---|
| Untitled.md | Empty file — should be deleted |
| Cody.md | Minimal content, only 1 outbound link |
| README.md | References `05_Timeline/` but actual folder is `05_Chain_of_Custody/` |
| James Luhr Jr.md | Only 4 inbound links, minimal content |

### LOW — Dollar Figures Without Inline Source Links
- Investigation Dashboard finding table references amounts but links go to findings, not source evidence (acceptable for dashboard)
- Cash Flow Dashboard `$241,284 "ADJ TO STMT"` and `$84,960 "Ins/Elog"` need source document links
- Some raw data index files have no dollar figures extracted yet

---

## Improvement Plan

| Pass | Priority | Description | Est. Files Affected |
|---|---|---|---|
| 2 | CRITICAL | Frontmatter normalization — add `type`, `confidence`, `created`, `updated`, `related`, `evidence-refs` | ~50 core files |
| 3 | HIGH | Create missing entity notes (Walker, GIG, Martha, EFS, McLeod) | 5 new files |
| 4 | HIGH | Evidence citation pass — inline source links on dollar figures | ~15 findings/evidence |
| 5 | HIGH | Dashboard improvements — add Dataview queries | 4 dashboard files |
| 6 | MEDIUM | Graph layer — graph.json narratives, MOC-Master, bridge notes | ~5 files |
| 7 | MEDIUM | Visual polish — CSS theme, callout styles | 2 files |
| 8 | LOW | Changelog, README fix, cleanup Untitled.md | 3 files |

---

## Positive Findings

- **Excellent link density** — core findings, evidence, and entities are deeply cross-linked
- **Strong chain of custody** — Source Registry, Data Lineage, Duplicate Tracker are comprehensive
- **Consistent templates** — 8 templates cover all note types
- **Dollar figures well-documented** — most amounts have exact values with sources identified
- **Investigation Dashboard is thorough** — 30 findings tracked with status/confidence/links
- **90+ raw data index notes** — every source file has a stub note
