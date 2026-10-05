# Integrations

| Tool | Status | Used for | Reference |
|---|---|---|---|
| Google Sheets | Connected | Task list + goals | "Daily Assistant Tasks", ID `1_TknnUD17Mpw2IIo-wmawaqjTQWPmACERVQLVjRXEXc` (tabs: Tasks, Inbox, Goals, Log, Weekly) |
| Google Calendar | Connected (Oct 1) | Reading the week; writing "🧱 <task>" blocks tagged "Scheduled by Nehemiah" | Primary calendar + Family, High Holy Days (`truespiritofchrist.com_be306n876qji74i6hid6c0vmsg@group.calendar.google.com`), Church Master; America/Chicago |
| Gmail | Connected | Time-sensitive email scan | Last 24h each morning |
| Google Drive | Connected | Working docs; Nehemiah folder for handoff files and drafts | Folder "Nehemiah", ID `1M4Cpxl7ZtSDEmmuXeAry7bIc753E_6jF` |
| Mac folders | Connected per live chat when the computer is online | ai-os repo; class notes or drafts only when a task needs them | Not reachable from scheduled tasks |
| GitHub | Private repo (backup) | Version history for this folder | https://github.com/arielleisrael/ai-os |
| Claude Project | "Nehemiah - Daily Assistant" | Where Nehemiah runs | Doc: "Daily Assistant Agent — Plan & Instructions.md" |

## Scheduled tasks

| Name | Schedule (CT) | Prompt | ID |
|---|---|---|---|
| Nehemiah morning check-in | Sun–Fri 6:55am | [`prompts/morning-checkin.md`](prompts/morning-checkin.md) | `trig_018WKUZBsTiCRoaHM3HKXMmB` |
| Nehemiah nightly recap | Sun–Thu 8:00pm | [`prompts/nightly-recap.md`](prompts/nightly-recap.md) | `trig_0177CrV9Vdm1Zgxaz6vdFwtb` |
| Nehemiah weekly plan | Sun 8:50am | [`prompts/weekly-plan.md`](prompts/weekly-plan.md) | `trig_01HnDRokgnoN49EJrZDJunTC` |
| Daily briefing (paused Oct 5) | Daily 9:00am | Older read-only brief, superseded by the morning check-in | `trig_015oZqQYPbJLBkjAVdpBN5bY` |

Scheduled tasks pick up the connectors that exist when they are created.
After connecting a new tool, recreate the tasks so they can use it.

Prompts in the scheduled tasks = the prompt file with `<<CALENDAR RULES>>` replaced by [`prompts/_calendar-rules.md`](prompts/_calendar-rules.md) and `<<INBOX RULES>>` replaced by [`prompts/_inbox-rules.md`](prompts/_inbox-rules.md).
