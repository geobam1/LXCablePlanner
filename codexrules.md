# Codex Rules for LXCablePlanner

This document defines when and how to use Codex, focusing on tasks where it excels over Claude CLI.

---

## When to Use Codex

Codex is the stronger tool for these tasks:

### 1. Quick Inline Edits
**Why Codex is better:** Optimized for fast, surgical edits with IDE integration and real-time feedback loop.
- Single-line or few-line fixes
- Typo corrections
- Variable renames within a file
- Adding/removing a single function or block

### 2. Iterative Code Completion
**Why Codex is better:** Designed for autocomplete-style suggestions while actively writing code.
- Completing partially written functions
- Generating boilerplate code as you type
- Suggesting next lines based on context
- Quick snippets and patterns

### 3. Sandboxed Code Execution
**Why Codex is better:** Runs code in isolated sandbox environment with safe execution.
- Testing code snippets safely
- Running scripts without affecting the system
- Experimenting with changes before committing

### 4. Test & Build Verification
**Why Codex is better:** Direct execution of local toolchain with captured outputs.
- Running unit tests and reporting results
- Executing lint checks
- Running build scripts
- Verifying command outputs verbatim

### 5. Targeted File Edits
**Why Codex is better:** Precise patch application with minimal diffs when you know exactly what to change.
- Editing a specific known location
- Applying a focused fix to a single file
- Making changes when the exact edit is already defined

### 6. Simple Known Searches
**Why Codex is better:** Fast local queries when you know exactly what you're looking for.
- Finding a specific function by name
- Locating a known string or variable
- Quick grep for an exact match

---

## When to Defer to Claude CLI

Hand off to Claude for:
- Git operations (commits, PRs, branch management)
- Exploratory codebase searches ("how does X work?")
- Multi-step tasks requiring planning
- Code review and analysis
- Documentation and explanations
- Web research and external lookups

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
