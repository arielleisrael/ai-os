# Nehemiah: daily chief of staff

Makes sure each day's work moves Arielle toward her goals, sized to the
energy she actually has.

| File | What it is |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Persona and operating instructions (source of truth) |
| [`goals.md`](goals.md) | Goals file, priority windows, weekly top 3 |
| [`task-schema.md`](task-schema.md) | Task fields, where tasks live, cutover to Cairn |
| [`integrations.md`](integrations.md) | Connected tools, IDs, scheduled tasks |
| [`decisions.md`](decisions.md) | Why the rules are what they are |
| [`prompts/`](prompts/) | Scheduled-task prompts (morning, nightly, weekly) |
| [`archive/`](archive/) | Earlier versions of the plan |

## Where it runs

Nehemiah runs as a Claude Project ("Daily Assistant") plus two scheduled tasks.
Those run in the cloud and cannot read this folder, so after changing
anything here:

1. `CLAUDE.md` -> paste into the Project instructions.
2. `goals.md` + `CLAUDE.md` + `task-schema.md` -> update the Project doc
   "Daily Assistant Agent — Plan & Instructions.md".
3. `prompts/*.md` -> update the matching scheduled task's prompt.
4. Commit with a message that says what behavior changed.

Asking Claude to "sync Nehemiah from the repo" in the Daily Assistant
project covers steps 1–3 (step 1 still needs a manual paste).
