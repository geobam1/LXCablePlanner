# Claude CLI Rules for LXCablePlanner

This document defines when and how to use Claude CLI, focusing on tasks where it excels over Codex.

---

## When to Use Claude CLI

Claude is the stronger tool for these tasks:

### 1. Git Operations
**Why Claude is better:** Native git integration with automatic commit formatting, branch management, and PR creation built-in.
- Commit, push, pull, and branch operations
- Creating well-formatted commit messages
- Managing pull requests via `gh` CLI
- Resolving merge conflicts with full context

### 2. Codebase Exploration & Understanding
**Why Claude is better:** Specialized search agents, parallel file reading, and pattern matching across large codebases.
- Finding where functionality is implemented
- Understanding code flow across multiple files
- Answering "how does X work?" questions
- Tracing dependencies and imports

### 3. Complex Multi-Step Tasks
**Why Claude is better:** Built-in task planning (TodoWrite), progress tracking, and ability to break down complex work.
- Feature implementations requiring multiple files
- Refactoring with many interdependent changes
- Debugging issues that span multiple components

### 4. Code Review & Analysis
**Why Claude is better:** Long context window allows reviewing entire files/features at once with deep reasoning.
- Reviewing changes for bugs or issues
- Security analysis
- Suggesting architectural improvements
- Identifying edge cases

### 5. Documentation & Explanations
**Why Claude is better:** Strong natural language generation and ability to understand context deeply.
- Writing or updating README files
- Explaining complex code sections
- Creating technical documentation

### 6. Interactive Problem Solving
**Why Claude is better:** Can ask clarifying questions mid-task and adapt approach based on answers.
- Ambiguous requirements that need clarification
- Tasks where user preferences matter
- Exploratory debugging

### 7. Web Research & External Resources
**Why Claude is better:** Built-in web search and URL fetching capabilities.
- Looking up API documentation
- Finding solutions to errors
- Researching best practices

---

## When to Defer to Codex

Hand off to Codex for tasks where it is stronger:

- Quick inline edits (single-line fixes, typos) because it provides immediate local diffs.
- Iterative code completion because it excels at autocomplete-style drafting while typing.
- Local execution and verification because it can run commands and capture verbatim output.
- Targeted file changes because it applies precise patches with minimal diffs.

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
