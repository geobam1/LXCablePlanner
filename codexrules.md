# Codex Rules for LXCablePlanner

This document defines when and how to use Codex, focusing on tasks where it excels over Claude CLI.

---

## When to Use Codex

Codex is the stronger tool for these tasks:

### 1. Quick Inline Edits
**Why Codex is better:** Optimized for fast, surgical edits with immediate local diffs.
- Single-line or few-line fixes
- Typo corrections
- Variable renames within a file
- Adding/removing a single function or block

### 2. Iterative Code Completion
**Why Codex is better:** Suited to autocomplete-style drafting while writing code.
- Completing partially written functions
- Generating boilerplate as you type
- Suggesting next lines based on local context
- Quick snippets and patterns

### 3. Local Execution & Verification
**Why Codex is better:** Can run local commands in the repo and capture verbatim output.
- Running unit tests and reporting results
- Executing lint checks
- Running build scripts
- Verifying command outputs exactly

### 4. Targeted File Changes
**Why Codex is better:** Precise patch application when the exact edit is already defined.
- Editing a specific known location
- Applying a focused fix to a single file
- Making changes with minimal diffs

---

## When to Defer to Claude CLI

Hand off to Claude for tasks where it is stronger:

- Git operations (commits, PRs, branch management) because its workflow integrates commit formatting and PR tooling.
- Exploratory codebase searches ("how does X work?") because it uses broader search agents and cross-file reasoning.
- Multi-step tasks requiring planning because it has built-in task planning and progress tracking.
- Code review and analysis because it can reason across large context windows.
- Documentation and explanations because it excels at long-form, structured writing.
- Web research and external lookups because it can fetch and summarize external sources.

---

## Handoff Protocol

When finishing a session or handing off to Claude:
1. Save all file changes
2. State what was modified and why
3. Note any tests run and their results
4. List pending work or known issues

---

## Project Reference

- Main application: `💡 3REP Cable Planner_v2.html`
- Self-contained HTML with embedded CSS/JS
- Processes MVR and TXT files for cable planning

---

*Last updated: 2024-12-22*
