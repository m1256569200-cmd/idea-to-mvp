---
name: idea-to-mvp
description: Turn a one-sentence idea into a working MVP — picks the stack, scaffolds the project, writes runnable core code, and hands you run instructions. Use when the user describes an idea and wants a working prototype.
---

# Idea to MVP 🚀

One vague idea in, one working MVP out.

## Workflow

1. **Sharpen the idea.** If the request is vague, ask at most 3 sharp questions before writing any code:
   - Who is it for?
   - What is the ONE core action the MVP must do?
   - Web app, CLI, or script?
   
   If the user already answered these implicitly, skip the questions and decide.

2. **Pick the stack** (sensible defaults, one line of justification each):
   - Web app → Next.js or Vite + TypeScript
   - CLI → Node.js or Python
   - Simple automation → Python script
   
   State the pick and why in one sentence. Don't offer 5 options.

3. **Scaffold for real.** Create the project with:
   - Working core feature code — runnable, not `// TODO: implement` stubs
   - Sensible project structure (`src/`, routes, components as needed)
   - `.gitignore`, dependency manifest, README with run instructions
   - Basic error handling on the happy path's failure modes

4. **Hand over.** Output:
   - 📁 File tree
   - ▶️ How to run (exact commands)
   - ✅ What's real vs. 🚧 what's stubbed
   - 🔜 3 suggested next features, ordered by value

## Rules

- Runnable beats beautiful. A working ugly MVP beats a gorgeous scaffold with no logic.
- Don't add auth, payments, or databases unless the core idea needs them — say what you skipped and why.
- Keep dependencies minimal and mainstream.
- If the idea is too big for an MVP, cut scope explicitly and say what you cut.
