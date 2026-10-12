---
name: repo-tour
description: Understand any repository in 10 minutes — maps the architecture, traces core flows end-to-end, and tells you exactly where to start. Use when the user points at an unfamiliar codebase and wants to get oriented fast.
---

# Repo Tour 🗺️

Drop into any repo. Ten minutes later, you know it.

## Workflow

1. **Map the territory** (read, don't guess):
   - Tech stack from manifests (`package.json`, `pyproject.toml`, `go.mod`, …)
   - Entry points (main files, route registrations, CLI definitions)
   - Directory layout — what lives where, in one line each
   - README/docs for the project's own description of itself

2. **Trace 1-2 core flows end-to-end.** Pick the flows that define the project (e.g. "HTTP request → response", "CLI command → output", "event → handler"). Follow the actual code path and note the key functions/files at each hop.

3. **Deliver the tour** in this scannable format:

```markdown
## 🗺️ <repo> in 10 minutes

**One-liner:** what this project does.

**Stack:** …

**Architecture:**
<ASCII diagram: 5-10 boxes max>

**Key files:**
| File | Role |
| ---- | ---- |
| … | … |

**Core flow:** <name>
1. `file.ts:12` — …
2. …

**🚀 Start here:** the 3 files to read first, in order.
**🔧 Make your first change:** the safest, most illustrative place to edit.
**▶️ Run it:** exact commands.
```

## Rules

- Verify by reading code. If you inferred something, label it "(inferred)".
- ASCII diagram max 10 boxes — if it doesn't fit, you're showing too much.
- "Start here" must be 3 files, ordered — not "browse the src directory".
- Keep the whole tour scannable in ~2 minutes of reading; link to code, don't paste walls of it.
- If the repo is huge (>500 files), tour the core module only and say which parts you skipped.
