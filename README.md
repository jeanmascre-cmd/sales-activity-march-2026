# Sales Activity Analysis — March 2026

Weekly + monthly sales activity analysis for CFO, CEO, and VP Sales.
Validates actual rep activity (outbound calls, demos, emails) against stated workload.

---

## What it does

Fetches HubSpot activity data (calls, meetings, emails), aggregates by AE,
and produces a weekly/monthly report split by SME vs Enterprise and NB vs Upsell.
Flags reps with low activity, mislogged records, and process red flags
(e.g. too many follow-up calls relative to outbound calls).

Output: Notion page updated in-place + Slack summary to #rev_ops.

---

## Folder structure

| Folder/File | Purpose |
|---|---|
| `data/` | Raw HubSpot extracts (JSON, CSV) by activity type |
| `output/` | Analysis reports in markdown |
| `scripts/` | Main analysis script |
| `.github/workflows/` | Weekly + monthly scheduler (GitHub Actions) |
| `CLAUDE.md` | Project rules — read this before any analysis |
| `README.md` | This file |
| `requirements.txt` | Python dependencies |

---

## Key metrics

| Metric | HubSpot object | Filter |
|---|---|---|
| Outbound calls | calls | hs_activity_type = "Call - Outbound" |
| Discovery calls | calls | hs_activity_type = "Call - Discovery" |
| Demo Scheduled (DS) | meetings | type = 1st Demo + outcome SCHEDULED |
| Demo Done (DD) | meetings | type = 1st Demo + outcome COMPLETED |
| Emails sent | emails | direction = EMAIL, status = SENT |
| Sequences running | sequence enrollments | status = ACTIVE |

---

## GitHub repo

`jeanmascre-cmd/sales-activity-march-2026`

---

## Related projects

- [pipeline-analysis-march-2026](https://github.com/jeanmascre-cmd/pipeline-analysis-march-2026) — daily pipeline report (same HubSpot account)
- [20260318-outbound-calls-meetings-report](https://github.com/jeanmascre-cmd/20260318-outbound-calls-meetings-report) — outbound call audit (methodology reference)

---

*Built by Jean Mascré, RevOps — March 2026*
