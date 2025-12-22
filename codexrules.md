# Codex Rules for LXCablePlanner

This document defines when and how to use Codex, focusing on tasks where it excels over Claude CLI.

---

## When to Use Codex

Codex is the stronger tool for these tasks:

### 1. IDE-Integrated Editing (Copilot)
**Why Codex is better:** Embedded in your editor with cursor-aware context and real-time suggestions.
- Autocomplete while typing in VS Code/IDE
- Context-aware completions based on cursor position
- Inline suggestions without switching tools
- Tab-to-accept workflow

### 2. Sandboxed Code Execution
**Why Codex is better:** Runs code in an isolated environment without affecting your local system.
- Testing experimental code safely
- Running untrusted snippets
- Trying changes before committing locally
- Executing code without side effects

### 3. Real-Time Autocomplete
**Why Codex is better:** Optimized for low-latency, typing-flow completions.
- Completing functions as you write them
- Generating boilerplate without interrupting flow
- Pattern-based suggestions from local context
- Ghost text previews

### 4. Rapid Prototyping in Chat
**Why Codex is better:** ChatGPT code interpreter can execute and iterate on code instantly.
- Quick experiments with immediate output
- Visualizations and data analysis
- Iterating on small scripts
- Testing logic before integrating

---

## When to Defer to Claude CLI

Hand off to Claude for tasks where it is stronger:

- Git operations (commits, PRs, branch management) because it has native workflow integration.
- Exploratory codebase searches ("how does X work?") because it uses specialized search agents.
- Multi-step tasks requiring planning because it has built-in task tracking.
- Code review and analysis because it reasons across large context windows.
- Documentation and explanations because it excels at structured long-form writing.
- Web research and external lookups because it can fetch and summarize external sources.
- Direct file edits on your codebase because both tools edit equally well, but Claude operates directly on your files without sandboxing.
- Local command execution because Claude CLI runs on your actual system with full access.

---

## Handoff Protocol

When finishing a session or handing off to Claude:
1. Export/save any sandboxed work
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
