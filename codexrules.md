# Codex Rules for LXCablePlanner

Use Codex for tasks where its architectural strengths apply, regardless of deployment context.

---

## When to Use Codex

### 1. Quick Focused Edits
**Why:** Optimized for fast, minimal-diff changes with rapid feedback.
- Single-line or few-line fixes
- Typo corrections
- Variable renames
- Small function additions/removals

### 2. Iterative Code Drafting
**Why:** Low-latency responses suited to back-and-forth refinement.
- Completing partially written functions
- Generating boilerplate
- Pattern-based suggestions
- Rapid prototyping cycles

### 3. Continuation of Active Session
**Why:** Avoids context-switching overhead.
- Tasks related to work already in progress
- Follow-up edits to recent changes
- Immediate fixes to just-written code

---

## When to Defer to Claude

- Git operations (commits, PRs, branches) — native workflow integration
- Codebase exploration ("how does X work?") — specialized search agents
- Multi-step tasks requiring planning — built-in task tracking
- Code review and analysis — large context window reasoning
- Documentation and explanations — structured long-form writing
- Web research and external lookups — built-in fetch/search

---

## Handoff Protocol

When handing off to Claude:
1. Save all file changes
2. State what was modified and why
3. List pending work

---

## Project Reference

- Main application: `💡 3REP Cable Planner_v2.html`
- Self-contained HTML with embedded CSS/JS
- Processes MVR and TXT files for cable planning

---

*Last updated: 2024-12-22*
