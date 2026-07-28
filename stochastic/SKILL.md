---
name: stochastic
description: "Stochastic multi-agent consensus. Spawns N agents with identical prompts to independently analyze a problem. Aggregates by consensus (mode), divergences (splits), and outliers (unique ideas)."
allowed-tools:
  - Read
  - Agent
  - Grep
  - Glob
  - Bash
---

# /stochastic — Multi-Agent Consensus

Spawn N agents (default 10) with identical context and near-identical prompts. Each independently analyzes and produces a structured response. Aggregate by finding consensus (mode), divergences (splits), and outliers (unique ideas).

$ARGUMENTS — the problem, question, or decision to distribute across agents.

Optional: `n=X` — number of agents (default 10)

## Why this works

Exploits stochastic variation in LLM outputs. Repeated independent runs make stable conclusions, divergences, and outliers visible instead of hiding them inside one confident answer.

Agreement is a stability signal, not proof. Repetition can reduce idiosyncratic errors, but every run can still share the same false premise. Evidence and human review remain required.

## How it works

1. Parse the problem into a clear question
2. Spawn N agents in parallel with identical prompts
3. Collect all responses
4. Aggregate: mode, splits, outliers

## Agent prompt template

```
Analyze this problem:
[QUESTION]

Give your conclusion with reasoning. Rate confidence (high/medium/low). Flag anything uncertain.

Under 300 words. Lead with conclusion.
```

## Aggregation

- **Consensus (mode)** — what most agents agree on
- **Divergences (splits)** — where agents disagree, revealing genuine judgment calls
- **Outliers** — unique ideas only 1-2 agents surfaced

## Output

Report directly:
- Agents polled: N
- Deduplicated ideas with frequency counts
- Total raw ideas
