# HIVE

[![Support me on Patreon](https://img.shields.io/badge/Patreon-Support%20my%20work-FF424D?style=flat&logo=patreon&logoColor=white)](https://www.patreon.com/AndersBjarby)

An experimental Claude Code setup that treats an agent team as a collective intelligence rather than a hierarchy. Instead of fixed roles, HIVE manifests "capabilities" that spawn, merge, split, mutate, and dissolve based on what the work actually needs.

## Concept

- No CEO, no titles, no careers — capabilities are temporary crystallizations of competence.
- Each capability has an energy level (0–100) that rises when used and decays when idle; below the threshold it dissolves back into the "void" (archived in `.claude/dissolved/`), ready to be resurrected later.
- Organization emerges from the work, not from up-front planning.

## Commands

| Command | Purpose |
|---------|---------|
| `/spawn` | Manifest a new capability |
| `/status` | View active capabilities and their energy |
| `/evolve` | Trigger self-analysis and evolution |
| `/dissolve` | Return a capability to the void |

## Usage

Open the project in Claude Code and use the slash commands above. The coordinating agent lives in `.claude/agents/hive.md`, command definitions in `.claude/commands/`, and spawned capabilities are written to `.claude/capabilities/`.

```bash
claude
/spawn
> Describe needed capability: "Handle database operations with Postgres"
```

## Tech

Claude Code (Markdown agents, slash commands, and capability files under `.claude/`).
