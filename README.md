# Building Agents Workshop

Free Claude skills from the *Building Agents to Automate Routine Tasks* workshop. Install one, run it on your own work, and keep what it makes. Each works on the free plan.

A **skill** is a saved play. You teach the AI the steps once, and it runs them the same way every time.

## What's in here

| Skill | What it does |
|-------|--------------|
| [weekly-dashboard](weekly-dashboard/) | Turn a messy brain-dump or a photo of your calendar into a clean, prioritized weekly dashboard. |
| [clipify](clipify/) | Turn one long video into short, social-ready 9:16 clips with burned-in captions. Runs fully on your machine. |
| [fanout](fanout/) | Fan-out research. Spawns several researchers in parallel to explore a question from different angles, then synthesizes one answer. |
| [stochastic](stochastic/) | Ask many agents the same question independently, then see where they agree, where they split, and what only one or two noticed. |
| [autoresearch](autoresearch/) | Autonomous hill-climb on any numeric metric — bundle size, build time, a score. Generates changes, measures each one, keeps what wins. |
| [crucible](crucible/) | Pressure-test a cold email, headline, or pitch before it ships. Generates variants, judges them from the recipient's point of view, kills the weak ones. |

## How to load a skill in Claude

1. Download or clone this repo.
2. On the **free plan**, turn on **Code execution and file creation** in Settings.
3. Point Claude at the skill folder (or copy its `SKILL.md` into your skills directory), then run it on your own real input.

Clipify needs a few local tools (ffmpeg, Whisper, Python). See [clipify/README.md](clipify/README.md) for setup. Autoresearch needs Node. Fanout, stochastic, autoresearch, and crucible spawn subagents, so they work best in Claude Code.

## Use them as a starting point

Free to use as-is or to fork into your own. Start with one, run it on something real this week, then make it yours.

All of these are mine except clipify, which is adapted from [Louise de Sadeleer](https://github.com/louisedesadeleer) and keeps its own license and credit.

— Celine Krzan
