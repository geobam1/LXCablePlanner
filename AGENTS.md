# Project Continuation Rules (Claude + Codex)

Last updated: 2025-12-22

## Scope
This repo should contain **HTML files and sample data only**. Avoid adding non-HTML artifacts unless explicitly requested.

## Primary files
- `💡 3REP Cable Planner_v2.html` (main tool)
- `💡 3REP LX Data Entry_v3.html`
- `versions/` snapshots
- `sample data/` (TSV/TXT/MVR test files)

## Working rules
1. **HTML-only repo**: Keep the repository limited to HTML and sample data. Do not add logs, scripts, chat files, or temporary files unless the user explicitly requests them.
2. **Versioning**: Before any major change, save a timestamped copy in `versions/`:
   - `versions/3REP_Cable_Planner_YYYYMMDD_HHMMSS.html`
3. **Commit discipline**: Commit after each major change or phase. Use short, descriptive messages.
4. **Testing**: UI testing is manual in the browser. If you can’t test, state “NEEDS REVIEW (manual UI test).”
5. **Snapshot priority**: When in doubt, save a snapshot before changing logic.

## Current state / open items
- Project is functional but still pending **visual refresh parity** with older HTML reference files:
  - `/Users/georgebamforth/Downloads/OLD 3REP Cable Planner.html`
  - `/Users/georgebamforth/Downloads/💡 3REP LX Network Builder.html`
- Missing feature analysis already completed and recorded in prior notes.

## Communication rules
- **Claude**: keep approvals short; avoid re-reading files unless necessary.
- **Codex**: do heavy lifting (file reads, analysis, implementation), then report back concisely.
- Reports should include:
  - 2–3 sentence summary
  - line references (no code blocks unless asked)
  - status: DONE / NEEDS REVIEW / BLOCKED

## File hygiene
- Remove `.DS_Store` if it appears.
- Do not add new non-HTML files without explicit request.

## Sample data
Keep `sample data/` tracked in git:
- `3REP_Device_Library_v4.tsv`
- `Snap-On 2026 Lighting 2025 12.05c_EXP.txt`
- `Snap-On Regional Kickoff 2026 v12.10.25a.mvr.zip`

