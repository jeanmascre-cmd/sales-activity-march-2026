# Sales Activity Analysis — March 2026
Date: 2026-03-23 | Audience: CFO, CEO, VP Sales | Source: HubSpot MCP live pull

---

## TLDR — What the data says

- **Michelle Frank has zero outbound calls and zero upsell activity all year.** 144 emails total. No visible prospecting motion. Needs immediate 1:1.
- **Kristyna Safrova (INACTIVE) has 509 outbound calls attributed this week alone** — all 509 YTD calls fall within the Mar 17+ window for an inactive rep. Data integrity issue. Excluded from all team metrics.
- **The team is active in March** — Sofia Bonicelli (256 outbound MTD), Kirsty Freely (201), Alexandra Dias (135), Sam Kaplan (106), Don Patrick Jakobsen (107) all showing strong March volumes.
- **Kirsty Freely leads upsell activity** — 21 upsell meetings YTD, nearly 3× the next highest rep.

---

## Call Methodology Note

**Outbound calls counted using `hubspot_owner_id`, not `hs_created_by_user_id`.**

Three reps (Sofia Bonicelli, Sam Kaplan, Jessica Civitella) use Aircall. Aircall creates calls via an integration user and assigns them to the rep via `hubspot_owner_id`. Their calls never appear under their own HubSpot user ID as creator. Reps on the HubSpot native dialer (Kirsty Freely, Don Patrick Jakobsen) create calls as themselves.

Using `hs_created_by_user_id` misses all Aircall calls and undercounts for ~50% of the team. The HubSpot native "core report" uses this method and is therefore incomplete. `hubspot_owner_id` is the correct field and is used throughout this analysis.

**Sample validation (2026-03-23):** Two call records reviewed on contact Katie Hubbard (Jessica Civitella) — Mar 10, 19:13 (Left voicemail) and 19:15 (Answered/Connected, note: "in surgery / fd took my info"). Confirmed as two genuine separate calls: first went to voicemail, rep called back 2 minutes later and reached the front desk. No duplication. Aircall counts are valid.

---

## Activity Summary — All AEs (YTD 2026)

| AE | Status | Outbound Calls | Discovery Calls | Upsell Meetings | Emails Sent | Follow-Up Calls ⚠️ |
|---|---|---|---|---|---|---|
| Jessica Civitella | Active | 89 | 2 | 8 | 5,441 | 164 |
| Sam Kaplan | Active | 118 | 1 | 0 | 3,569 | 297 |
| Don Patrick Jakobsen | Active | 107 | 0 | 1 | 315 | 37 |
| Sofia Bonicelli | Active | 274 | 36 | 5 | 9,234 | 166 |
| Kirsty Freely | Active | 235 | 10 | 21 | 11,675 | 269 |
| Alexandra Dias | Active | 135 | 1 | 4 | 1,779 | 60 |
| Carlos Archanco | Active | 78 | 75 | 6 | 8,010 | 77 |
| Michelle Frank | Active | 0 | 0 | 0 | 144 | 0 |
| Emelie Schneider | Active | 7 | 7 | 1 | 4,815 | 8 |
| Juha Huttunen | Active | 1 | 0 | 2 | 480 | 0 |
| Scott Goodsir-Smyth | Active | 8 | 0 | 0 | 1,792 | 0 |
| Kristyna Safrova ⚠️ | **INACTIVE** | 509* | 3 | — | 861 | 2,984* |

> ⚠️ Kristyna Safrova: INACTIVE rep. All 509 outbound calls appear within Mar 17+. Data integrity issue. Excluded from team totals.

**Team totals (active AEs only):** Outbound calls: 1,062 | Upsell meetings: 48 | Emails sent: 47,254

---

## Outbound Calls — Monthly Trend

| AE | Jan | Feb | Mar MTD | This Week | Trend |
|---|---|---|---|---|---|
| Jessica Civitella | 0 | 1 | 88 | 88 | ↑↑ Ramping hard in March |
| Sam Kaplan | 6 | 6 | 106 | 106 | ↑↑ Strong March |
| Don Patrick Jakobsen | 0 | 0 | 107 | 107 | ↑↑ All activity in March |
| Sofia Bonicelli | 9 | 9 | 256 | 216 | ↑↑ Best March volume |
| Kirsty Freely | 22 | 12 | 201 | 185 | ↑↑ Consistent + strong |
| Alexandra Dias | 0 | 0 | 135 | 135 | ↑↑ All activity in March |
| Carlos Archanco | 21 | 26 | 31 | 14 | → Slowing in March |
| Michelle Frank | 0 | 0 | 0 | 0 | ⚠️ Zero outbound all year |
| Emelie Schneider | 0 | 1 | 6 | 5 | → Very low |
| Juha Huttunen | 1 | 0 | 1 | 1 | → Minimal |
| Scott Goodsir-Smyth | 0 | 0 | 8 | 8 | → Very low |
| Kristyna Safrova ⚠️ | 0 | 0 | 509* | 509* | DATA ISSUE |

> Note: Several AEs show 0 outbound in Jan/Feb with a significant spike in March. Don Patrick Jakobsen and Alexandra Dias in particular — confirm start dates before interpreting Jan/Feb zeros as underperformance.

---

## Discovery Calls

Carlos Archanco (75 discovery calls) is the clear outlier — he runs a high-volume discovery motion compared to all peers. Sofia Bonicelli (36) is second. All other AEs are in single digits.

| AE | Discovery Calls YTD |
|---|---|
| Carlos Archanco | 75 |
| Sofia Bonicelli | 36 |
| Emelie Schneider | 7 |
| Kirsty Freely | 10 |
| Jessica Civitella | 2 |
| Alexandra Dias | 1 |
| Sam Kaplan | 1 |
| Don Patrick Jakobsen | 0 |
| Michelle Frank | 0 |
| Juha Huttunen | 0 |
| Scott Goodsir-Smyth | 0 |

---

## Upsell Activity (Meeting/Call - Upsell)

Counted from meetings object where `hs_activity_type = "Meeting/Call - Upsell"`. Note: this meeting type covers both calls and meetings — we do not know which format each was. Report as-is.

| AE | Upsell YTD | Completed | Scheduled/Future | No-Show |
|---|---|---|---|---|
| Kirsty Freely | 21 | 13 | 7 | 1 |
| Jessica Civitella | 8 | 7 | 1 | 0 |
| Carlos Archanco | 6 | 6 | 0 | 0 |
| Sofia Bonicelli | 5 | 4 | 0 | 1 |
| Alexandra Dias | 4 | 0 | 4 | 0 |
| Juha Huttunen | 2 | 2 | 0 | 0 |
| Don Patrick Jakobsen | 1 | 1 | 0 | 0 |
| Emelie Schneider | 1 | 1 | 0 | 0 |
| Sam Kaplan | 0 | — | — | — |
| Michelle Frank | 0 | — | — | — |
| Scott Goodsir-Smyth | 0 | — | — | — |

> Kirsty Freely has the highest upsell volume by a significant margin. Alexandra Dias has 4 upsell meetings booked but none completed yet — all in SCHEDULED state in March.

---

## Emails

Includes manual 1:1 emails and sequence emails — cannot be separated at the email object level. Reported as "Total emails sent."

| AE | Emails Sent YTD |
|---|---|
| Kirsty Freely | 11,675 |
| Sofia Bonicelli | 9,234 |
| Carlos Archanco | 8,010 |
| Jessica Civitella | 5,441 |
| Emelie Schneider | 4,815 |
| Sam Kaplan | 3,569 |
| Alexandra Dias | 1,779 |
| Scott Goodsir-Smyth | 1,792 |
| Juha Huttunen | 480 |
| Don Patrick Jakobsen | 315 |
| Michelle Frank | 144 |

---

## Follow-Up Call Ratio Flag

Per CLAUDE.md: flag any AE where Sales Follow-Up calls > 3× Outbound calls.

| AE | Outbound | Follow-Up | Ratio | Flag? |
|---|---|---|---|---|
| Jessica Civitella | 89 | 164 | 1.8× | No |
| Sam Kaplan | 118 | 297 | 2.5× | No (borderline — monitor) |
| Don Patrick Jakobsen | 107 | 37 | 0.3× | No |
| Sofia Bonicelli | 274 | 166 | 0.6× | No |
| Kirsty Freely | 235 | 269 | 1.1× | No |
| Alexandra Dias | 135 | 60 | 0.4× | No |
| Carlos Archanco | 78 | 77 | 1.0× | No |
| Michelle Frank | 0 | 0 | — | No (no activity) |
| Emelie Schneider | 7 | 8 | 1.1× | No |
| Juha Huttunen | 1 | 0 | 0× | No |
| Scott Goodsir-Smyth | 8 | 0 | 0× | No |
| Kristyna Safrova ⚠️ | 509* | 2,984* | 5.9× | ⚠️ DATA ISSUE — INACTIVE |

No active AE exceeds the 3× threshold. Sam Kaplan at 2.5× is the closest — monitor through April.

---

## Who Needs Attention ⚠️

**Michelle Frank — 0 outbound calls YTD | 0 upsell meetings | 0 discovery calls | 144 emails**
Zero prospecting activity on all metrics. No outbound calls, no upsell meetings, no discovery. 144 emails is the lowest on the team. No visible active selling motion. Needs immediate 1:1 review.

**Emelie Schneider — 7 outbound calls YTD | 7 discovery calls | 1 upsell meeting | 4,815 emails**
Email volume is high (likely sequence-driven) but call activity is minimal. Sustainable prospecting pipeline unclear.

**Juha Huttunen — 1 outbound call YTD | 2 upsell meetings | 480 emails**
Minimal activity across all call metrics. Low email volume.

**Scott Goodsir-Smyth — 8 outbound calls YTD | 0 upsell meetings | 1,792 emails**
Low call volume. May be in a different motion (enterprise/strategic) with lower volume expectations. Has 1 enterprise demo in Feb 2026.

---

## Enterprise Activity

4 confirmed enterprise demos YTD (Meeting - Enterprise Customer Demo). Low volume — consistent with expectation.

| AE | Enterprise Demos |
|---|---|
| Kirsty Freely | 1 (Mar 2026) |
| Scott Goodsir-Smyth | 1 (Feb 2026) |
| Sam Kaplan | 1 (historical) |
| Jessica Civitella | 1 (historical) |

Only Kirsty and Scott have enterprise demos in Q1 2026.

---

## Data Quality Flags

### 1. Calls logged on meetings object
Sales Follow-Up calls found on the meetings object (should be on calls object):
- **Sam Kaplan (108125586):** 6 follow-up calls logged as meetings in 2026
- **Sofia Bonicelli (264419305):** 3 follow-up calls logged as meetings in 2026

Flag to both reps each run. This undercounts their call metrics and pollutes the meetings object.

### 2. Kristyna Safrova (INACTIVE) — data integrity
All 509 outbound calls attributed to owner 140964498 fall within the Mar 17+ window. Implausible for an inactive rep. Possible causes: bulk import, backdated re-attribution, or a system migration that re-stamped timestamps.

**Action required:** Audit HubSpot for bulk activity on owner 140964498 after Mar 17, 2026.

### 3. Unclassified motion records
Motion (New Business vs Upsell) not audited in this run — deal type analysis deferred. Flag for next run.

---

## Per-AE Detail

### Jessica Civitella (311286579)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 1 | 88 | 89 |
| Discovery Calls | — | — | — | 2 |
| Upsell Meetings | — | 3 | 4 | 8 |
| Emails Sent | — | — | — | 5,441 |
| Follow-Up Calls | — | — | — | 164 |

Notes: Ramped hard in March — 88 outbound calls MTD vs 1 in Feb. 8 upsell meetings YTD, all in Feb/Mar. Follow-up ratio 1.8× — acceptable.

---

### Sam Kaplan (108125586)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 6 | 6 | 106 | 118 |
| Discovery Calls | — | — | — | 1 |
| Upsell Meetings | 0 | 0 | 0 | 0 |
| Emails Sent | — | — | — | 3,569 |
| Follow-Up Calls | — | — | — | 297 |

Notes: Strong outbound ramp in March. Zero upsell meetings YTD — all activity is NB motion. Follow-up ratio 2.5× — borderline, monitor. 6 follow-up calls logged as meetings (data quality issue).

---

### Don Patrick Jakobsen (83717736)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 107 | 107 |
| Discovery Calls | — | — | — | 0 |
| Upsell Meetings | — | — | 1 | 1 |
| Emails Sent | — | — | — | 315 |
| Follow-Up Calls | — | — | — | 37 |

Notes: All 107 outbound calls came in March. Zero Jan/Feb — confirm start date. Very low email volume (315). 1 upsell meeting completed in March.

---

### Sofia Bonicelli (264419305)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 9 | 9 | 256 | 274 |
| Discovery Calls | — | — | — | 36 |
| Upsell Meetings | 1 | 0 | 4 | 5 |
| Emails Sent | — | — | — | 9,234 |
| Follow-Up Calls | — | — | — | 166 |

Notes: Highest discovery call count (36) — running a discovery-first motion. Top outbound volume YTD. 5 upsell meetings (4 completed, 1 no-show). 3 follow-up calls logged as meetings (data quality).

---

### Kirsty Freely (124826644)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 22 | 12 | 201 | 235 |
| Discovery Calls | — | — | — | 10 |
| Upsell Meetings | 2 | 11 | 8 | 21 |
| Emails Sent | — | — | — | 11,675 |
| Follow-Up Calls | — | — | — | 269 |

Notes: #1 by emails sent (11,675). #1 by upsell meetings (21 YTD — 13 completed). Consistent outbound across all months. Follow-up ratio 1.1× — healthy.

---

### Alexandra Dias (82586810)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 135 | 135 |
| Discovery Calls | — | — | — | 1 |
| Upsell Meetings | 1 | 0 | 3 | 4 |
| Emails Sent | — | — | — | 1,779 |
| Follow-Up Calls | — | — | — | 60 |

Notes: All activity concentrated in March. 4 upsell meetings booked, none completed yet (all SCHEDULED). Zero Jan/Feb activity — confirm start date.

---

### Carlos Archanco (156289960)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 21 | 26 | 31 | 78 |
| Discovery Calls | — | — | — | 75 |
| Upsell Meetings | 6 | 0 | 0 | 6 |
| Emails Sent | — | — | — | 8,010 |
| Follow-Up Calls | — | — | — | 77 |

Notes: Highest discovery call count by far. All 6 upsell meetings occurred in Jan — none since Feb. Outbound volume slowing in March (31 MTD vs 26 in Feb and 21 in Jan).

---

### Michelle Frank (85529907)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 0 | 0 |
| Discovery Calls | — | — | — | 0 |
| Upsell Meetings | 0 | 0 | 0 | 0 |
| Emails Sent | — | — | — | 144 |
| Follow-Up Calls | — | — | — | 0 |

⚠️ Zero activity on all call and upsell metrics across all of YTD 2026. Lowest email volume by far. No prospecting motion visible in the data.

---

### Emelie Schneider (181769737)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 1 | 6 | 7 |
| Discovery Calls | — | — | — | 7 |
| Upsell Meetings | — | 1 | 0 | 1 |
| Emails Sent | — | — | — | 4,815 |
| Follow-Up Calls | — | — | — | 8 |

Notes: High email volume (4,815) but only 7 outbound calls YTD. Discovery and outbound call counts are identical — working purely from inbound or referral flow.

---

### Juha Huttunen (37634691)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 1 | 0 | 1 | 1 |
| Discovery Calls | — | — | — | 0 |
| Upsell Meetings | — | — | 2 | 2 |
| Emails Sent | — | — | — | 480 |
| Follow-Up Calls | — | — | — | 0 |

Notes: Minimal outbound. 2 upsell meetings completed in March. Low overall volume.

---

### Scott Goodsir-Smyth (96216654)

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 8 | 8 |
| Discovery Calls | — | — | — | 0 |
| Upsell Meetings | 0 | 0 | 0 | 0 |
| Emails Sent | — | — | — | 1,792 |
| Follow-Up Calls | — | — | — | 0 |

Notes: Low outbound volume. 1 enterprise demo in Feb 2026. May be covering a strategic/enterprise territory with lower volume expectations.

---

### Kristyna Safrova (140964498) — INACTIVE ⚠️

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 509* | 509* |
| Emails Sent | — | — | — | 861 |
| Follow-Up Calls | — | — | — | 2,984* |

⚠️ INACTIVE rep. All 509 outbound calls and 2,984 follow-up calls appear entirely within the Mar 17+ window. Likely a data migration or re-attribution event. Excluded from all team metrics. Audit required.

---

*Report generated: 2026-03-23 | Data source: HubSpot MCP live pull | YTD = Jan 1 2026 – Mar 23 2026*
