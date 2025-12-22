# Codex Rules for LXCablePlanner

This document defines when and how to use Codex, focusing on task suitability rather than deployment details.

---

## When to Use Codex

Codex is the stronger tool for these tasks:

### 1. Quick Inline Edits
**Why Codex is better:** Optimized for fast, surgical edits with minimal diffs.
- Single-line or few-line fixes
- Typo corrections
- Variable renames within a file
- Adding/removing a single function or block

### 2. Iterative Drafting
**Why Codex is better:** Low-latency completions while actively writing code.
- Completing partially written functions
- Generating boilerplate as you type
- Suggesting next lines based on local context

### 3. Targeted File Changes
**Why Codex is better:** Precise patch application when the exact edit is already defined.
- Editing a specific known location
- Applying a focused fix to a single file
- Making changes with minimal diffs

### 4. Simple Known Searches
**Why Codex is better:** Fast exact-match queries when you already know the identifier or string.
- Locating a specific function or variable by name
- Finding a known string or UI label
- Quick exact-match grep with `rg`

---

## When to Defer to Claude CLI

Hand off to Claude for tasks where it is stronger:

- Git operations and PRs because of workflow integration and commit formatting.
- Exploratory codebase searches because it excels at cross-file reasoning.
- Multi-step tasks requiring planning because it provides structured task tracking.
- Code review and analysis because it reasons across large contexts.
- Documentation and explanations because it produces strong long-form output.
- Web research and external lookups because it can fetch and summarize sources.
- Interactive problem solving because it adapts through clarifying questions.

Note: Local command execution follows the active tool and is not the deciding factor.

---

## Handoff Protocol

When finishing a session or handing off to Claude:
1. Commit all changes with clear messages
2. State what was modified and why
3. Note any tests run or issues encountered
4. List pending work for Claude to continue

---

## Project Reference

- Main application: `💡 3REP Cable Planner_v2.html`
- Self-contained HTML with embedded CSS/JS
- Processes MVR and TXT files for cable planning

---

*Last updated: 2024-12-22*
