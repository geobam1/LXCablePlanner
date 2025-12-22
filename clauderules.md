# Claude CLI Rules for LXCablePlanner

Use Claude for tasks where its architectural strengths apply, regardless of deployment context.

---

## When to Use Claude

### 1. Git Operations
**Why:** Native `gh` CLI integration with automatic commit formatting and PR workflows.
- Commits, pushes, pulls, branch management
- Creating well-formatted commit messages
- Pull request creation and management
- Merge conflict resolution with full context

### 2. Codebase Exploration
**Why:** Specialized search agents with parallel file reading and cross-file reasoning.
- Finding where functionality is implemented
- Understanding code flow across files
- Answering "how does X work?" questions
- Tracing dependencies and imports

### 3. Multi-Step Planning
**Why:** Built-in task tracking (TodoWrite) and ability to break down complex work.
- Feature implementations spanning multiple files
- Refactoring with interdependent changes
- Debugging across components

### 4. Code Review & Analysis
**Why:** Large context window enables reviewing entire files with deep reasoning.
- Reviewing changes for bugs or issues
- Security analysis
- Architectural improvements
- Edge case identification

### 5. Documentation
**Why:** Strong natural language generation for structured long-form writing.
- README files
- Code explanations
- Technical documentation

### 6. Interactive Problem Solving
**Why:** Can ask clarifying questions and adapt approach mid-task.
- Ambiguous requirements
- User preference decisions
- Exploratory debugging

### 7. Web Research
**Why:** Built-in web search and URL fetching.
- API documentation lookup
- Error solutions
- Best practices research

---

## When to Defer to Codex

- Quick focused edits (single-line fixes, typos)
- Iterative code drafting with rapid feedback
- Tasks already in progress in Codex session

---

## Handoff Protocol

When handing off to Codex:
1. Commit all changes with clear messages
2. State what was modified and why
3. List pending work

---

## Project Reference

- Main application: `💡 3REP Cable Planner_v2.html`
- Self-contained HTML with embedded CSS/JS
- Processes MVR and TXT files for cable planning

---

*Last updated: 2024-12-22*
