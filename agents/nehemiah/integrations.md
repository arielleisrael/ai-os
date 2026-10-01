# Integrations

| Tool | Status | Used for | Reference |
|---|---|---|---|
| Google Sheets | Connected | Task list + goals | "Daily Assistant Tasks", ID `1_TknnUD17Mpw2IIo-wmawaqjTQWPmACERVQLVjRXEXc` (tabs: Tasks, Goals) |
| Google Calendar | Connected (Oct 1) | Reading the day; writing "[Nehemiah]" time blocks | Primary calendar, America/Chicago |
| Gmail | Connected | Time-sensitive email scan | Last 24h each morning |
| Google Drive | Connected | Working docs | |
| Mac home folder | Linked when the computer is online | Class notes, content drafts | Not reachable from scheduled tasks |
| Claude Project | "Daily Assistant" | Where Nehemiah runs | Doc: "Daily Assistant Agent — Plan & Instructions.md" |

## Scheduled tasks

| Name | Schedule (CT) | Prompt | ID |
|---|---|---|---|
| Nehemiah morning check-in | Sun–Fri 6:55am | [`prompts/morning-checkin.md`](prompts/morning-checkin.md) | `trig_018WKUZBsTiCRoaHM3HKXMmB` |
| Nehemiah nightly recap | Sun–Thu 8:00pm | [`prompts/nightly-recap.md`](prompts/nightly-recap.md) | `trig_0177CrV9Vdm1Zgxaz6vdFwtb` |
| Weekly review | Not scheduled yet | [`prompts/weekly-review.md`](prompts/weekly-review.md) | |

Scheduled tasks pick up the connectors that exist when they are created.
After connecting a new tool, recreate the tasks so they can use it.
