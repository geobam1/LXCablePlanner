# Codex Collaboration Rules (When Codex Is the Stronger Tool)

This document lists tasks where Codex should take the lead. If a task is not listed here, defer to the other agent.

## 1) Git & Repo Operations
- Use Codex for pulls, status checks, commits, and pushes because it can run local git commands and verify results in the repo.
- Use Codex for applying the commit message format in `clauderules.md` because it can stage, commit, and confirm the exact changes.

## 2) File Edits in This Repo
- Use Codex for direct edits to `💡 3REP Cable Planner_v2.html`, `README.md`, and rules files because it can apply precise patches and keep diffs minimal.
- Use Codex for file moves/renames in the repo because it can execute filesystem commands and confirm the outcome.

## 3) Search & Inspection
- Use Codex for repo-wide searches because it can run fast local queries (`rg`) and report exact matches.
- Use Codex for reviewing local code paths because it can open files directly and cite exact locations.

## 4) Local Verification
- Use Codex for any local checks (lint/tests/scripts) because it can run commands and capture outputs verbatim.
