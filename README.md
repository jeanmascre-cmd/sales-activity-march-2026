# Sales Activity Analysis — March 2026

Weekly + monthly sales activity analysis for CFO, CEO, and VP Sales.
Validates actual rep activity (outbound calls, demos, emails) against stated workload.
Split: SME vs Enterprise | NB vs Upsell

---

## What it does

Fetches HubSpot activity data (calls, meetings, emails) across all AEs,
aggregates by rep and period, flags low performers and data quality issues,
and produces a report showing the reality of sales team activity.

Output: Notion page + Slack summary to #rev_ops

---

## Key metrics

| Metric | HubSpot object | Filter |
|---|---|---|
| Outbound calls | calls | hs_activity_type = "Call - Outbound" |
| Discovery calls | calls | hs_activity_type = "Call - Discovery" |
| Demo Scheduled (DS) | meetings | type = 1st Demo + outcome SCHEDULED/RESCHEDULED |
| Demo Done (DD) | meetings | type = 1st Demo + outcome COMPLETED |
| No-show | meetings | type = 1st Demo + outcome NO_SHOW |
| Emails sent | emails | direction = EMAIL, status = SENT |
| Follow-Up calls ⚠️ | calls | hs_activity_type = "Call - Sales Follow-Up" (flag only) |

**Important:** Outbound = hs_activity_type = "Call - Outbound". Never use hs_call_direction.

---

## Files

| File | Description |
|---|---|
| `CLAUDE.md` | Project rules, AE owner IDs, known data quality issues — read before any analysis |
| `README.md` | This file |
| `requirements.txt` | Python dependencies (requests, pytz) |
| `data/by-ae-calls.csv` | Outbound, discovery, follow-up calls per AE × period |
| `data/by-ae-demos.csv` | DS, DD, no-show, cancel per AE × period |
| `data/by-ae-emails.csv` | Emails sent per AE YTD |
| `data/data-quality.csv` | Mislogged activities per AE |
| `output/sales-activity-march-2026.md` | Full analysis report — 2026-03-23 |
| `scripts/` | Automation scripts (to be added) |
| `.github/workflows/` | GitHub Actions scheduler (to be added) |

---

## Active AEs

| Name | Owner ID |
|---|---|
| Jessica Civitella | 311286579 |
| Sam Kaplan | 108125586 |
| Don Patrick Jakobsen | 83717736 |
| Sofia Bonicelli | 264419305 |
| Kirsty Freely | 124826644 |
| Alexandra Dias | 82586810 |
| Carlos Archanco | 156289960 |
| Michelle Frank | 85529907 |
| Emelie Schneider | 181769737 |
| Juha Huttunen | 37634691 |
| Scott Goodsir-Smyth | 96216654 |

---

## Key findings — first run (2026-03-23)

- **Michelle Frank:** Zero outbound calls all year. Zero completed demos. Needs immediate 1:1.
- **Carlos Archanco:** 67% no-show rate (163/244 demos). Booking quality problem.
- **Kristyna Safrova (INACTIVE):** 509 outbound calls all appearing in one week — data integrity issue, exclude from team metrics.
- **Team strong performers in March:** Sofia Bonicelli, Kirsty Freely, Sam Kaplan, Don Patrick Jakobsen

---

## Related projects

- [pipeline-analysis-march-2026](https://github.com/jeanmascre-cmd/pipeline-analysis-march-2026) — daily pipeline report
- [20260318-outbound-calls-meetings-report](https://github.com/jeanmascre-cmd/20260318-outbound-calls-meetings-report) — outbound call audit (methodology reference)

---

*Built by Jean Mascré, RevOps — March 2026*
