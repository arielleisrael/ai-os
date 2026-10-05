# Communication and handoffs

How Arielle, or any other work, reaches Nehemiah.

| Need | Channel | When Nehemiah acts |
|---|---|---|
| Talk it through, re-plan now | Chat in the **Nehemiah - Daily Assistant** Project (desktop or phone), starting with "Nehemiah: …" | Immediately |
| Hand off something to plan | Add a row to the **Inbox** tab of the task sheet | Next routine (7 AM, 8 PM or Sunday plan) |
| Hand off a file (draft, notes, doc to review) | Put it in the **Nehemiah** Google Drive folder; optionally add an Inbox row linking it | Next routine (unlisted new files get an Inbox row automatically) |
| Something urgent from other work | Inbox row with Urgency = Urgent, then open a Project chat | Immediately in chat; listed first at the next routine |
| Reply to a routine | Answer the routine's message in its own session | Immediately |

## Inbox tab

Sheet "Daily Assistant Tasks" (ID `1_TknnUD17Mpw2IIo-wmawaqjTQWPmACERVQLVjRXEXc`), tab **Inbox**.

| Column | Values |
|---|---|
| Timestamp | YYYY-MM-DD HH:MM CT |
| From | "Arielle", "Claude Code: <repo>", "chat: <topic>" |
| Ask | One sentence: what's needed and why |
| Track | Job search, ReinventOps, Brand, Software factory, Church, Home, Planning |
| Urgency | Urgent, Today, This week, Whenever |
| Status | New, Scheduled, Done, Dropped |
| Resolution | Filled in by Nehemiah |

Triage rules: [`prompts/_inbox-rules.md`](prompts/_inbox-rules.md).

## Nehemiah Drive folder

Google Drive folder **Nehemiah** (ID `1M4Cpxl7ZtSDEmmuXeAry7bIc753E_6jF`, https://drive.google.com/drive/folders/1M4Cpxl7ZtSDEmmuXeAry7bIc753E_6jF). Working drafts and notes Nehemiah should see, and drafts Nehemiah makes for Arielle. Scheduled routines can read Drive but not the Mac, so files for Nehemiah go here, not in a local folder or this repo. Class notes and content drafts stay where they already live; connect that Mac folder to a live chat only when a task needs it.

## Snippet for repos and other agents

Paste into each repo's `CLAUDE.md` (already in the ai-os root `CLAUDE.md`):

```markdown
## Handoffs to Nehemiah (Arielle's chief of staff)
When work here produces something Arielle needs to schedule, decide, or
follow up on (a blocker, a finished milestone, a promise to someone, a
deadline), append one row to the Inbox tab of the "Daily Assistant Tasks"
Google Sheet (ID 1_TknnUD17Mpw2IIo-wmawaqjTQWPmACERVQLVjRXEXc):
Timestamp (YYYY-MM-DD HH:MM CT) | From ("Claude Code: <repo>") | Ask (one
sentence, what's needed and why) | Track | Urgency | Status = New | Resolution
blank. Don't edit other tabs. If the Sheets connector isn't available,
tell Arielle the one-line Ask so she can add it.
```

## Later

- Cairn replaces the Inbox tab at cutover (see [`task-schema.md`](task-schema.md)).
- Slack or Discord only if other people (Uzziah, clients) need to reach Nehemiah. Revisit after Nov 15.
