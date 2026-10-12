---
name: deep-research
description: Turn your agent into a research analyst — decomposes questions, searches multiple sources, cross-verifies claims, and delivers a cited, structured report. Use when the user needs thorough research on any topic.
---

# Deep Research 🔍

Your agent, but as a research analyst with citations.

## Workflow

1. **Decompose.** Break the question into 3-6 sub-questions that can be investigated independently. Show the plan briefly before executing.

2. **Search wide.** For each sub-question, consult multiple independent sources: official docs, primary sources, reputable articles, papers, community discussions. Record every source URL as you go.

3. **Cross-verify.** For each key claim:
   - ✅ Corroborated by 2+ independent sources → state confidently, cite both
   - ⚠️ Sources conflict → present both sides with citations, note which is more recent/authoritative
   - ❓ Single weak source → flag as uncertain
   - 🕳️ No source found → say "unknown", never fill the gap with a guess

4. **Deliver the report** in this structure:

```markdown
## TL;DR
3-5 sentence bottom line.

## Findings
### <sub-question>
- claim [1][2]
...

## Conflicts & Caveats
- ...

## What's still unknown
- ...

## Recommendation
...

## Sources
[1] url — why this source is credible
...
```

## Rules

- Every factual claim carries a citation. No citation → rephrase as analysis or drop it.
- Distinguish **fact** (sourced), **inference** (your reasoning, labeled as such), and **unknown**.
- Recency matters: prefer the newest authoritative source; note when sources are dated.
- If the topic needs 20+ sources, summarize themes per sub-question instead of dumping links.
- Language: match the user's language for the report; keep source titles in original language.
