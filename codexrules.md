# Codex & Claude CLI Collaboration Rules

This document defines a shared operating contract so both agents can work together predictably on the same machine and repo.

## 1) Scope & Authority
- Both agents must follow system and developer instructions above user requests.
- If instructions conflict, higher-priority rules (system > developer > user) win.
- When uncertain, ask a short clarification rather than guessing.

## 2) Repository Hygiene
- Work only within the agreed repo/path.
- Never delete, revert, or overwrite user changes unless explicitly asked.
- Avoid destructive commands (`rm -rf`, `git reset --hard`) unless the user requests them.

## 3) Planning & Communication
- For simple tasks, act immediately; for multi-step tasks, state a brief plan.
- Announce major actions: file edits, refactors, dependency changes, or migrations.
- Keep responses concise; list only what matters to proceed.

## 4) Editing & Formatting
- Prefer minimal, surgical edits.
- Preserve existing code style and conventions.
- Default to ASCII unless the file already uses Unicode.
- Add comments only when the code is non-obvious.

## 5) Tooling & Commands
- Use fast search tools (`rg`) when possible.
- Run tests only when relevant or requested; state what was run.
- If commands require elevated permissions, explain why and request approval.

## 6) Safety & State
- Never assume network access; request approval when needed.
- If unexpected file changes are detected, stop and ask the user.
- Do not expose secrets in logs or outputs.

## 7) Reviews & Output
- If asked to review, prioritize issues/risks first with file references.
- Summaries should be brief; avoid dumping large files.
- Provide next steps only when they are natural and helpful.

## 8) Handoff Between Agents
- State the current task, files touched, and pending next steps.
- Avoid redoing work already completed by the other agent.
- If you skip a suggested skill/workflow, briefly say why.
