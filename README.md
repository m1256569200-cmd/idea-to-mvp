# 🤖 agent-team

**One task, a team of agents. 大任务自动拆分、多 agent 并行 — *agent-team is all you need.***

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Skill](https://img.shields.io/badge/skill-Claude%20Code%20%7C%20Cursor%20%7C%20Copilot-blue)

## ✨ What it does

Hand your agent a task that's too big for one straight shot. It decomposes it into **truly independent** subtasks, assigns roles (`researcher`, `implementer`, `reviewer`…), dispatches them **in parallel**, then synthesizes everything into one coherent result — conflicts resolved, final review pass included.

```
you: "research 3 competitors, summarize each, and compare pricing"
agent: ✂️ 4 subtasks → 🤖 parallel dispatch → 🧩 synthesis + review
```

## 📦 Install

```bash
# Claude Code
mkdir -p ~/.claude/skills/agent-team && cp SKILL.md ~/.claude/skills/agent-team/

# Cursor (project-level)
mkdir -p .cursor/skills/agent-team && cp SKILL.md .cursor/skills/agent-team/
```

## 🎯 How it works

1. **✂️ Decomposes** — 2-5 independent subtasks, each with inputs + done-criteria
2. **🎭 Assigns roles** — researcher / implementer / reviewer / writer / tester
3. **🚀 Dispatches in parallel** — partitioned by file/directory, scope-guarded
4. **🧩 Synthesizes** — merges, resolves conflicts explicitly, one final review pass

## 🧭 Ground rules

- Independence is non-negotiable — dependent work becomes phases, not subtasks
- Max 5 parallel agents; done-criteria in writing before dispatch
- Never ships 5 disconnected outputs — synthesis is the whole point

---

## 🇨🇳 中文介绍

**一个任务，一支 agent 小队。** 大任务自动拆成真正独立的子任务，分配角色并行开干，最后汇总成一份连贯的结果。

- ✂️ 拆：2-5 个独立子任务，每个写明输入和完成标准
- 🎭 分角色：researcher / implementer / reviewer / writer / tester
- 🚀 并行派发：按文件/目录分区，互不踩脚
- 🧩 汇总：合并结果、显式解决冲突、最后再过一遍 reviewer

适合：竞品调研、技术选型、多模块开发、任何"一个人干太慢"的大任务。

## 📄 License

MIT
