# 🚀 idea-to-mvp

**Turn one sentence into a working MVP. 一句话想法 → 可运行的 MVP — *idea-to-mvp is all you need.***

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Skill](https://img.shields.io/badge/skill-Claude%20Code%20%7C%20Cursor%20%7C%20Copilot-blue)

## ✨ What it does

You describe an idea in one sentence. Your agent picks the stack, scaffolds the project, writes **runnable** core code, and hands you exact run instructions. No `// TODO` stubs, no 5-option questionnaires.

```
you: "a habit tracker with streaks"
agent: 📁 file tree + ▶️ npm run dev + ✅ what's real + 🔜 next features
```

## 📦 Install

Copy `SKILL.md` into your skills folder:

```bash
# Claude Code
mkdir -p ~/.claude/skills/idea-to-mvp && cp SKILL.md ~/.claude/skills/idea-to-mvp/

# Cursor (project-level)
mkdir -p .cursor/skills/idea-to-mvp && cp SKILL.md .cursor/skills/idea-to-mvp/
```

Then just say: *"build me an MVP for …"*

## 🎯 How it works

1. **🔪 Sharpens** the idea — at most 3 questions (who / core action / platform)
2. **🧱 Picks** a mainstream stack with one line of justification
3. **⚙️ Scaffolds** real working code — happy path fully runnable
4. **📋 Hands over** — file tree, run commands, real-vs-stubbed, next 3 features

## 🧭 Scope discipline

Won't silently add auth, payments, or databases. If your idea needs cutting down to MVP size, it tells you exactly what got cut.

---

## 🇨🇳 中文介绍

**一句话想法 → 可运行的 MVP。** 把想法丢给 agent，它帮你选技术栈、搭项目结构、写出**真正能跑**的核心代码，最后给你运行命令和后续规划。

- 🔪 最多问 3 个关键问题，不啰嗦
- 🧱 技术栈只选主流的，并一句话说明理由
- ⚙️ 核心功能是真代码，不是 TODO 占位
- 📋 交付：文件树、运行命令、已实现/未实现清单、下一步建议

适合：想快速验证想法的独立开发者、黑客松选手、产品经理。

## 📄 License

MIT
