# AI OS

Arielle's personal AI Operating System: the agents, rules and context that run
a multi-domain life (job search, ReinventOps, personal brand, church, home).

GitHub (private): https://github.com/arielleisrael/ai-os

Each agent lives in its own folder under `agents/`. The files there are the
source of truth for how the agent behaves. Runtime data (tasks, logs) lives in
the tools the agent reads and writes, not in this repo.

```
agents/
  nehemiah/   daily chief of staff: morning check-in, nightly recap, weekly review
```

## Conventions

- Change an agent's behavior here first, then sync it to wherever it runs
  (see each agent's `README.md`).
- Record why a rule changed in that agent's `decisions.md`.
- No secrets, tokens or personal account numbers in this repo.
