---
name: agent-team
description: Turn one big task into a coordinated team of agents — decomposes work, assigns roles, runs subtasks in parallel, then synthesizes the results. Use when a task is too big for one straight shot and splits into independent parts.
---

# Agent Team 🤖

One task in. A team of agents on it. One synthesized result out.

## Workflow

1. **Decompose.** Break the task into subtasks that are genuinely independent — each needs clear inputs, a definition of done, and no dependency on another subtask's output. If everything depends on everything, say so and don't force parallelism. Aim for 2-5 subtasks.

2. **Assign roles.** Give each subtask a role that fits: `researcher` (gather facts), `implementer` (write code), `reviewer` (critique), `writer` (docs), `tester` (verify). One role per subtask, stated up front.

3. **Dispatch in parallel.** Launch all subtasks together with:
   - The exact slice of work (not "help with the project")
   - Its inputs and done-criteria
   - What NOT to touch (scope guard)
   
   Subagents must not step on each other's files — partition the work by file/directory.

4. **Synthesize.** When all return:
   - Merge the outputs into one coherent result
   - Resolve conflicts explicitly (state what conflicted and which resolution you picked)
   - Run one final `reviewer` pass over the combined result
   - Report: what each agent did (1 line each) + the unified outcome

## Rules

- Independence is non-negotiable. A subtask that needs another's output is not a subtask — it's a phase. Sequence phases, parallelize within them.
- Cap at 5 parallel agents. More than that and coordination costs exceed the gains.
- Every subtask gets done-criteria in writing before dispatch. "Do your best" is not a criterion.
- If a subtask fails, retry it once with narrower scope before giving up on it — and say so in the report.
- Never present 5 disconnected outputs as the final answer. Synthesis is the job.
