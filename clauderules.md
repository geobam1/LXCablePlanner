# AI Assistant Rules for LXCablePlanner

## Project Overview
This is a Cable Planning Tool for Live Events that processes MVR and TXT files to create cable lists. The main application is a single-page HTML application.

---

## General Rules

### 1. Code Consistency
- Maintain the existing code style and structure
- Do not refactor working code unless explicitly requested
- Keep changes minimal and focused on the task at hand

### 2. File Structure
- Main application: `💡 3REP Cable Planner_v2.html`
- This is a self-contained HTML file with embedded CSS and JavaScript
- Do not split into separate files unless requested

### 3. Before Making Changes
- Always read the relevant code sections before modifying
- Understand the existing implementation before suggesting changes
- Test changes mentally or describe expected behavior

---

## Git Workflow

### Commit Messages
- Use clear, descriptive commit messages
- Format: `<type>: <description>`
- Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`

### Branches
- Work on `main` unless otherwise specified
- Pull latest changes before starting work
- Commit frequently with atomic changes

---

## Collaboration Rules (Claude CLI & ChatGPT/Codex)

### Handoff Protocol
1. **Document your changes**: When finishing a session, summarize what was done
2. **Note pending tasks**: List any incomplete work or known issues
3. **Avoid conflicts**: Don't leave uncommitted changes when possible

### Communication
- Use comments in code only when logic is complex
- Update this document if new conventions are established
- Keep README.md updated with significant feature changes

### Conflict Resolution
- If encountering merge conflicts, preserve both sets of changes when possible
- When in doubt, ask the user before overwriting changes
- Check git status before starting new work

---

## Code Standards

### HTML
- Use semantic HTML5 elements
- Maintain accessibility attributes where present
- Keep inline styles minimal; prefer embedded CSS

### CSS
- Use consistent naming conventions
- Group related styles together
- Comment sections for clarity

### JavaScript
- Use clear variable and function names
- Handle errors gracefully with user feedback
- Preserve existing event handlers and logic patterns

---

## Prohibited Actions
- Do not delete or overwrite files without explicit permission
- Do not introduce external dependencies without approval
- Do not commit sensitive data or credentials
- Do not make breaking changes to file import/export functionality

---

## Quick Reference

| Action | Command |
|--------|---------|
| Pull latest | `git pull` |
| Check status | `git status` |
| Stage all | `git add .` |
| Commit | `git commit -m "type: message"` |
| Push | `git push` |

---

*Last updated: 2024-12-22*
