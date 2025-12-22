# Claude CLI Rules for LXCablePlanner

This document defines when and how to use Claude CLI, focusing on task suitability rather than deployment details.

---

## When to Use Claude CLI

Claude is the stronger tool for these tasks:

### 1. Git Workflow & PRs
**Why Claude is better:** Native workflow integration with commit formatting and PR tooling.
- Commit, push, pull, and branch operations
- Creating well-formatted commit messages
- Managing pull requests via `gh` CLI
- Resolving merge conflicts with full context

### 2. Codebase Exploration & Understanding
**Why Claude is better:** Strong cross-file reasoning for “how does X work?” questions.
- Finding where functionality is implemented
- Understanding code flow across multiple files
- Tracing dependencies and imports

### 3. Complex Multi-Step Tasks
**Why Claude is better:** Built-in task planning and progress tracking.
- Feature implementations requiring multiple files
- Refactors with interdependent changes
- Debugging issues that span components

### 4. Code Review & Analysis
**Why Claude is better:** Long-context reasoning across entire features.
- Reviewing changes for bugs or issues
- Security analysis
- Identifying edge cases

### 5. Documentation & Explanations
**Why Claude is better:** Strong long-form, structured writing.
- Writing or updating README files
- Explaining complex code sections
- Creating technical documentation

### 6. Interactive Problem Solving
**Why Claude is better:** Iterative clarifications and adaptive approach.
- Ambiguous requirements that need clarification
- Tasks where user preferences matter

### 7. Web Research & External Resources
**Why Claude is better:** Can fetch and summarize external sources.
- Looking up API documentation
- Finding solutions to errors
- Researching best practices

---

## When to Defer to Codex

Hand off to Codex for tasks where it is stronger:

- Quick inline edits (single-line fixes, typos) because it excels at fast, minimal diffs.
- Iterative drafting because it is optimized for low-latency completions.
- Targeted file changes because it applies precise patches when the edit is already defined.
- Simple known searches because it can run fast exact-match queries locally.

Note: Local command execution follows the active tool and is not the deciding factor.

---

## Handoff Protocol

When finishing a session or handing off to Codex:
1. Commit all changes with clear messages
2. State what was modified and why
3. Note any tests run or issues encountered
4. List pending work for Codex to continue

---

## Project Reference

- Main application: `💡 3REP Cable Planner_v2.html`
- Self-contained HTML with embedded CSS/JS
- Processes MVR and TXT files for cable planning

---

*Last updated: 2024-12-22*
