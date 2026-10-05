# Task schema and cutover

Tasks live in the **Daily Assistant Tasks** Google Sheet now (Notion hit its
free block limit) and move to Cairn, the software factory to-do app, once it
meets the cutover criteria. Same schema in both, so the migration is a
connection change.

| Field | Values |
|---|---|
| Title | Free text |
| Status | Not started / In progress / Done |
| Due date | Date (or "Daily" for standing blocks) |
| Domain | Job Search, ReinventOps, Brand, Church, Home |
| Linked goal | A goal from `goals.md` |
| Priority | High / Medium / Low |
| Track | Short-term / Long-term |
| Source | Email, meeting, self, Inbox: <From> |

Other tabs: **Inbox** (handoffs; see [`communication.md`](communication.md)), **Goals**, **Log**, **Weekly**.

## Cutover to Cairn when it:

- [ ] Supports create, update and status changes
- [ ] Has the domain and priority fields
- [ ] Exposes an API or MCP the agent can call
- [ ] Has run alongside the Google Sheet for one clean week
