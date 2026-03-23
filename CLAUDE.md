# Sales Activity Analysis — CLAUDE.md

## HOW TO ANSWER ANY ACTIVITY QUESTION — READ THIS FIRST

**NEVER use hs_call_direction to identify outbound calls.**
Outbound = the motion, identified by hs_activity_type = "Call - Outbound" on the calls object.

**NEVER mix SME and Enterprise.**
SME = corporate_deal = false OR no associated deal.
Enterprise = corporate_deal = true only.

---

## What this project is

Weekly + monthly sales activity analysis for CFO, CEO, VP Sales.
Purpose: validate or disprove rep claims about workload using actual HubSpot activity data.
Reference project: jeanmascre-cmd/pipeline-analysis-march-2026 (same HubSpot account, same patterns).

---

## SME vs Enterprise

| Segment | Filter |
|---|---|
| SME | corporate_deal = false on associated deal, OR activity has no associated deal |
| Enterprise | corporate_deal = true on associated deal only |

Activities with no associated deal are included in SME. Never shown separately.

---

## Motion (NB vs Upsell)

Motion property does not yet exist in HubSpot. Use dealtype as proxy:

| Motion | Deal types |
|---|---|
| New Business | newbusiness, New Business - NH Pay |
| Upsell | existingbusiness, Upsell - NH Pay, Upsell - Cubex, Upsell - Support |
| Unclassified | No associated deal or other deal type |

Unclassified should not exist. If any records are unclassified, flag them explicitly by AE —
this is a data quality issue that needs to be resolved.

Update this file when the Motion property goes live.

---

## Activity Definitions

### PRIMARY METRICS (what we measure and report)

#### 1. Outbound Calls
**Object:** calls
**Filter:** hs_activity_type = "Call - Outbound"
**2026 YTD volume (as of 2026-03-23):** 3,836

This is the outbound prospecting motion. Do not use hs_call_direction.

**Call outcome (hs_call_disposition):**
| Value | Label |
|---|---|
| 47680b13-b839-45df-b882-12d353b02553 | Answered/Connected |
| 73a0d17f-1163-4015-bdd5-ec830791da20 | No answer |
| b2cf5968-551e-4856-9783-52b3da59a7d0 | Left voicemail |
| 1ae4f6e7-2ff7-4397-a00d-94eaaaa87c3f | Booked Demo |
| 4816fadb-7556-4334-bbd9-5d7e3bdd366c | Conversation with Prospect |
| f240bbac-87c9-4f6e-bf70-924b57d47db7 | Connected |

#### 2. Discovery Calls
**Object:** calls
**Filter:** hs_activity_type = "Call - Discovery"
**2026 YTD volume:** 984

Reported separately from demos. Discovery ≠ Demo Scheduled.
A discovery call precedes a demo — it is its own activity type and must not be counted
in the DS/DD funnel.

#### 3. Demos — SME New Business (the core funnel)
**Object:** meetings
**Types:** Meeting - 1st Sales Demo Online | Meeting - 1st Sales Demo On-Site
**2026 YTD volume:** 1,579 combined

| Metric | Filter |
|---|---|
| DS (Demo Scheduled) | hs_meeting_outcome IN (SCHEDULED, RESCHEDULED) |
| DD (Demo Done) | hs_meeting_outcome = COMPLETED |
| No-show | hs_meeting_outcome = NO_SHOW — flag per AE |
| Cancelled | hs_meeting_outcome = CANCELED — flag per AE |

#### 4. Emails Sent
**Object:** emails
**Filter:** hs_email_direction = EMAIL AND hs_email_status = SENT
**2026 YTD volume:** 83,879
Includes manual 1:1 emails and sequence emails — cannot be separated at the email object level.
Label as "Total emails sent" in all outputs.

#### 5. Sequences Running
Query HubSpot sequence enrollments API.
Count enrollments where status = ACTIVE at time of analysis, grouped by AE (enrolled_by).

---

### SECONDARY METRICS (flagged, not counted in main totals)

#### Sales Follow-Up Calls
**Object:** calls
**Filter:** hs_activity_type = "Call - Sales Follow-Up"
**2026 YTD volume:** 7,514

Not a primary activity metric. A high volume of follow-up calls relative to outbound calls
indicates a broken sales process — rep is chasing rather than prospecting.
**Flag any AE where Sales Follow-Up calls > 3× their Outbound calls in a given period.**

#### Follow-Up Demos
**Object:** meetings
**Types:** Meeting - Follow-Up Sales Demo Online | Meeting - Follow-Up Sales Meet On-Site
**2026 YTD volume:** 514

Not counted in the DS/DD funnel. A high volume of follow-up demos relative to 1st demos
may indicate deals are stalling. Flag per AE if disproportionate.

#### Upsell Calls/Meetings
**Object:** meetings
**Filter:** hs_activity_type = "Meeting/Call - Upsell"
**2026 YTD volume:** 140
Tracked separately. Not mixed into NB funnel.

#### Enterprise Demos
**Object:** meetings
**Type:** Meeting - Enterprise Customer Demo
**2026 YTD volume:** 4
Tracked in the Enterprise section. Very low volume — keep separate, never mix with SME.

---

### DATA QUALITY FLAGS (always run, always show per AE)

**Calls logged as meetings:**
Query meetings object where hs_activity_type = "Call - Outbound".
Per March 2026 audit: zero after the fix. Flag immediately if any recur.

**Sales Follow-Up logged as meetings:**
Query meetings object where hs_activity_type = "Call - Sales Follow-Up".
2026 YTD: 168 records. Flag per AE — these should be logged on the calls object.

---

## AE Attribution
Use hubspot_owner_id on each activity object.
This is the rep the activity is assigned to.

### Active AEs (SME sales team — confirmed 2026-03-23)
| Owner ID | Name | Status |
|---|---|---|
| 311286579 | Jessica Civitella | Active |
| 108125586 | Sam Kaplan | Active |
| 83717736 | Don Patrick Jakobsen | Active |
| 264419305 | Sofia Bonicelli | Active |
| 124826644 | Kirsty Freely | Active |
| 82586810 | Alexandra Dias | Active |
| 156289960 | Carlos Archanco | Active |
| 85529907 | Michelle Frank | Active |
| 181769737 | Emelie Schneider | Active |
| 37634691 | Juha Huttunen | Active |
| 96216654 | Scott Goodsir-Smyth | Active |
| 140964498 | Kristyna Safrova | **INACTIVE — exclude from team metrics** |

Refresh this list at the start of each run to catch new hires or departures.

---

## Comparison Periods

| Period | Definition |
|---|---|
| This week | Mon–Sun, vs prior week (WoW) |
| This month | MTD vs prior month same period, vs same month last year |
| QTD | vs prior quarter |
| YTD | Jan 1 current year to analysis date |

---

## Output Structure (same pattern as pipeline-analysis-march-2026)

### Main page sections:
1. **Activity summary table** — all AEs × primary metrics × current week + MTD
2. **Outbound calls** — volume by AE, weekly trend, outcome breakdown
3. **Discovery calls** — volume by AE, trend
4. **Demo funnel** — DS / DD / no-show / cancel by AE (SME only in main view)
5. **Emails + sequences** — total sent + active sequences per AE
6. **Enterprise section** — separate block, same metrics, clearly labelled
7. **Flags** — Sales Follow-Up high volume | Follow-Up demo high volume |
   mislogged activities | unclassified motion records
8. **Who needs attention** — reps with low activity vs stated position
   Format: "[Rep] — [N] DD | [N] outbound calls | [N] sequences running | [N] follow-up calls"

### Per-AE toggles (bottom of page):
One toggle per AE with full activity detail. Same structure as pipeline project.

---

## Output Destination
- Notion: Claude Code Automations — Company Catalogue
  https://www.notion.so/nordhealth/Claude-Code-Automations-Company-Catalogue-32757ba3e0ba817eb3fcc889c6634a3d
  New row in catalogue table + new linked Notion page with analysis.
- Slack: #rev_ops — summary alert on completion (same format as pipeline)

---

## Known Data Quality Issues (from first run 2026-03-23)

**Kristyna Safrova (140964498) — INACTIVE:**
All 509 outbound calls and 2,984 follow-up calls appear within the Mar 17+ window for an
inactive rep. Likely a bulk re-attribution or data migration event. Always exclude from
team metrics. HubSpot audit required on this owner ID.

**Calls logged as meetings — 2026 YTD:**
- Sam Kaplan: 6 follow-up calls logged on meetings object
- Sofia Bonicelli: 3 follow-up calls logged on meetings object
These should be on the calls object. Flag to the reps each run.

**Carlos Archanco no-show rate:**
67% no-show rate (163/244 demos) as of 2026-03-23. This is a known anomaly.
Track this metric every run — if it persists, escalate.

**Several AEs show zero Jan/Feb activity:**
Don Patrick Jakobsen, Alexandra Dias, Jessica Civitella — confirm start dates before
interpreting Jan/Feb zeros as underperformance.

---

## Validation Rules
1. total_outbound_calls > 0
2. total_demos > 0
3. SME + Enterprise = total (no records excluded)
4. Any unclassified motion records → alert and list by AE
5. If checks 1 or 2 fail: do not update Notion, send failure alert to #rev_ops

---

## Files

```
data/               — raw HubSpot extracts (JSON, CSV) by activity type
output/             — analysis reports (markdown)
scripts/            — main analysis script
.github/workflows/  — weekly + monthly scheduler
CLAUDE.md           — this file
README.md           — project overview
requirements.txt    — requests, pytz
```
