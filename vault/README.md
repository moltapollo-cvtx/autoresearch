# Apollo Investigation Vault — Setup Guide

## Quick Start
1. Unzip this folder anywhere on your machine
2. Open Obsidian → "Open folder as vault" → select the unzipped folder
3. Start with **00_Dashboard/Investigation Dashboard.md** — that's your home base

## Recommended Obsidian Plugins
Install these from Settings → Community Plugins:

- **Dataview** — Enables dynamic queries across notes (e.g., auto-generate tables of all `#finding` notes with their confidence levels)
- **Calendar** — Visual timeline navigation
- **Templater** — Use the templates in `07_Templates/` when creating new notes
- **Graph Analysis** — Enhanced graph view for mapping entity relationships
- **Kanban** — Optional: turn the Outstanding Document Demands into a visual board

## Vault Structure

```
00_Dashboard/       ← Start here. MOC pages that link to everything.
01_Entities/        ← People and companies involved
02_Evidence/        ← Source evidence organized by type
03_Findings/        ← Documented investigative conclusions
04_Cash_Flow/       ← Money movement tracking
05_Chain_of_Custody/ ← Source registry, data lineage, duplicate tracking
06_Strategy/         ← Meeting prep, evidence tiers, document demands
07_Templates/        ← Reusable note templates for new entries
08_Deliverables/     ← Index of formal documents produced
09_Raw_Data_Index/   ← Index notes for every raw source file (~90 files)
```

## How to Use Going Forward

### When you receive a new document:
1. SHA-256 hash it immediately
2. Create a new note from `Template - Document Receipt`
3. Add it to the Document Registry
4. Compare against prior versions of the same document

### When you identify a new finding:
1. Create a new note from `Template - Finding`
2. Link it to relevant entities, evidence, and timeline entries
3. Add it to the Investigation Dashboard summary table
4. Assess its evidence tier for the meeting

### When you have a Claude session:
1. Add a row to the Session Log in Investigation Dashboard
2. Update any affected findings, evidence, or entity notes
3. Add any new documents to the registry
4. Update the timeline if new dated events were identified

## Security Notes
- This vault contains sensitive investigation materials
- Store on an encrypted drive or use Obsidian's built-in encryption
- Back up regularly to off-site encrypted storage
- Do NOT sync to cloud services that ATI personnel could access
