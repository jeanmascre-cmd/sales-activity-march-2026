# Sales Activity Analysis — March 2026
Date: 2026-03-23 | Audience: CFO, CEO, VP Sales | Source: HubSpot MCP live pull

---

## TLDR — What the data says

- **Michelle Frank: zero outbound calls, zero upsell activity, 144 emails — all in March.** No prospecting motion visible on any metric. Needs immediate 1:1.
- **The team is active in March** — Sofia Bonicelli (256 outbound MTD), Kirsty Freely (201), Alexandra Dias (135), Sam Kaplan (106), Don Patrick Jakobsen (107).
- **Kirsty Freely leads upsell** — 21 Meeting/Call - Upsell YTD vs 8 for the next rep (Jessica).
- **Call - Sales Legacy flag** — Sofia Bonicelli has 52 legacy call logs YTD. This type should not be in active use. Flag for cleanup.
- **No dedicated call type for NB inbound calls** — see methodology note below. Follow-Up call volumes may include inbound NB activity.

---

## Call Methodology Note

**Outbound calls counted using `hubspot_owner_id`, not `hs_created_by_user_id`.**

Sofia Bonicelli, Sam Kaplan, and Jessica Civitella use Aircall. Aircall creates calls via an integration user and assigns them to the rep via `hubspot_owner_id`. Using `hs_created_by_user_id` misses all Aircall calls and undercounts for ~50% of the team. The HubSpot native "core report" uses this method and is therefore incomplete.

**Sample validation (2026-03-23):** Two call records on contact Katie Hubbard (Jessica Civitella) — Mar 10, 19:13 (Left voicemail) and 19:15 (Answered/Connected, note: "in surgery / fd took my info"). Two genuine separate calls confirmed. Aircall counts are valid.

**No dedicated call type for NB inbound calls.** There is no `Call - NB Inbound` or equivalent type in HubSpot. Inbound NB prospect calls are either not logged, captured under `Call - Sales Follow-Up`, or occasionally mislabelled as outbound. When reviewing follow-up call volumes, some of that count may reflect inbound NB activity, not chasing.

---

## Activity Summary — All AEs (YTD 2026, sorted by outbound call volume)

| AE | Outbound Calls | Discovery Calls | Meeting/Call - Upsell | Emails Sent | Follow-Up Calls ⚠️ |
|---|---|---|---|---|---|
| Sofia Bonicelli | 274 | 36 | 5 | 9,234 | 166 |
| Kirsty Freely | 235 | 10 | 21 | 11,675 | 269 |
| Alexandra Dias | 135 | 1 | 4 | 1,779 | 60 |
| Sam Kaplan | 118 | 1 | 0 | 3,569 | 297 |
| Don Patrick Jakobsen | 107 | 0 | 1 | 315 | 37 |
| Jessica Civitella | 89 | 2 | 8 | 5,441 | 164 |
| Carlos Archanco | 78 | 75 | 6 | 8,010 | 77 |
| Scott Goodsir-Smyth | 8 | 0 | 0 | 1,792 | 0 |
| Emelie Schneider | 7 | 7 | 1 | 4,815 | 8 |
| Juha Huttunen | 1 | 0 | 2 | 480 | 0 |
| Michelle Frank | 0 | 0 | 0 | 144 | 0 |
| Kristyna Safrova ⚠️ INACTIVE | 509* | 3 | — | 861 | 2,984* |

> ⚠️ Kristyna Safrova: INACTIVE. All 509 outbound calls appear within Mar 17+. Data integrity issue. Excluded from all totals.

**Team totals (active AEs only):** Outbound: 1,062 | Meeting/Call-Upsell: 48 | Emails: 47,254

**Call - Sales Legacy — additional information, not included in any totals or metrics**

| AE | Legacy Calls YTD 2026 |
|---|---|
| Sofia Bonicelli | 52 |
| Carlos Archanco | 14 |
| Don Patrick Jakobsen | 2 |
| Jessica Civitella | 1 |
| All other AEs | 0 |

> `Call - Sales Legacy` is a deprecated activity type that should not be in active use. Sofia Bonicelli (52) is the largest user by far, followed by Carlos Archanco (14). Flag both reps to migrate to the correct type. These calls are **not** counted in outbound totals above.

---

## Outbound Calls — Monthly Trend

| AE | Jan | Feb | Mar MTD | This Week | Trend |
|---|---|---|---|---|---|
| Sofia Bonicelli | 9 | 9 | 256 | 216 | ↑↑ Best March volume |
| Kirsty Freely | 22 | 12 | 201 | 185 | ↑↑ Consistent + strong |
| Alexandra Dias | 0 | 0 | 135 | 135 | ↑↑ All activity in March |
| Sam Kaplan | 6 | 6 | 106 | 106 | ↑↑ Strong March |
| Don Patrick Jakobsen | 0 | 0 | 107 | 107 | ↑↑ All activity in March |
| Jessica Civitella | 0 | 1 | 88 | 88 | ↑↑ Ramping hard in March |
| Carlos Archanco | 21 | 26 | 31 | 14 | → Slowing in March |
| Scott Goodsir-Smyth | 0 | 0 | 8 | 8 | → Very low |
| Emelie Schneider | 0 | 1 | 6 | 5 | → Very low |
| Juha Huttunen | 1 | 0 | 1 | 1 | → Minimal |
| Michelle Frank | 0 | 0 | 0 | 0 | ⚠️ Zero all year |
| Kristyna Safrova ⚠️ | 0 | 0 | 509* | 509* | DATA ISSUE |

> Alexandra Dias, Don Patrick Jakobsen, and Jessica Civitella show zero or near-zero Jan/Feb. Confirm onboarding dates before interpreting as underperformance.

---

## Discovery Calls

| AE | Discovery Calls YTD |
|---|---|
| Carlos Archanco | 75 |
| Sofia Bonicelli | 36 |
| Kirsty Freely | 10 |
| Emelie Schneider | 7 |
| Jessica Civitella | 2 |
| Alexandra Dias | 1 |
| Sam Kaplan | 1 |
| Don Patrick Jakobsen | 0 |
| Michelle Frank | 0 |
| Juha Huttunen | 0 |
| Scott Goodsir-Smyth | 0 |

> **Logging behaviour varies significantly across reps.** Carlos Archanco (75) and Sofia Bonicelli (36) use `Call - Discovery` systematically. Most other AEs are at single digits or zero despite certainly conducting discovery conversations. This metric reflects logging discipline as much as actual discovery activity — cross-rep comparison should be used with caution until tagging is standardised.

---

## Upsell Activity (Meeting/Call - Upsell)

This type covers both calls and meetings — we do not distinguish format. Reported as-is.

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

> Carlos Archanco's 6 upsell meetings are all from January — none since February. Alexandra Dias has 4 booked but none completed yet.

---

## Emails — Monthly Trend

Includes manual 1:1 and sequence emails. Cannot be separated at email object level. Reported as "Total emails sent."

| AE | Q4 2025 | Jan 2026 | Feb 2026 | Mar MTD | Trend |
|---|---|---|---|---|---|
| Kirsty Freely | 2,088 | 2,843 | 325 | 8,507 | Jan high → Feb drop → Mar surge |
| Carlos Archanco | 2,191 | 194 | 1,664 | 6,169 | Volatile — big Q4, Mar ramp |
| Sofia Bonicelli | 513 | 96 | 958 | 8,180 | Strong Mar ramp |
| Jessica Civitella | 3 | 139 | 432 | 4,870 | Near zero before March |
| Emelie Schneider | 195 | 62 | 79 | 481 ⚠️ | Low and flat |
| Sam Kaplan | 863 | 164 | 284 | 3,121 | Strong March |
| Scott Goodsir-Smyth | 265 | 125 | 193 | 1,474 | Accelerating |
| Alexandra Dias | 0 | 0 | 0 | 1,779 | All in March |
| Don Patrick Jakobsen | 0 | 0 | 0 | 318 | All in March |
| Michelle Frank | 0 | 0 | 0 | 144 | All in March, lowest on team |
| Juha Huttunen | 0 | 0 | 0 | 0 ⚠️ | — |

> ⚠️ **Emelie Schneider:** Monthly query returns 622 emails YTD (62+79+481), but the YTD total from the original analysis was 4,815. Discrepancy likely due to sequence email metadata differences. Flag for investigation.
> ⚠️ **Juha Huttunen:** Monthly query returns 0 emails for all periods, but original YTD showed 480. Same likely cause. Flag for investigation.
> **Kirsty Freely Feb drop:** 325 in Feb vs 2,843 in Jan — possible sequence pause or period off. Recovered strongly in March.

---

## Follow-Up Call Ratio

Flag rule: Follow-Up calls > 3× Outbound calls in a given period.

| AE | Outbound | Follow-Up | Ratio | Flag? |
|---|---|---|---|---|
| Sofia Bonicelli | 274 | 166 | 0.6× | No |
| Kirsty Freely | 235 | 269 | 1.1× | No |
| Alexandra Dias | 135 | 60 | 0.4× | No |
| Sam Kaplan | 118 | 297 | 2.5× | No (borderline — monitor) |
| Don Patrick Jakobsen | 107 | 37 | 0.3× | No |
| Jessica Civitella | 89 | 164 | 1.8× | No |
| Carlos Archanco | 78 | 77 | 1.0× | No |
| Scott Goodsir-Smyth | 8 | 0 | 0× | No |
| Emelie Schneider | 7 | 8 | 1.1× | No |
| Juha Huttunen | 1 | 0 | 0× | No |
| Michelle Frank | 0 | 0 | — | No (no activity) |
| Kristyna Safrova ⚠️ | 509* | 2,984* | 5.9× | ⚠️ DATA ISSUE |

No active AE exceeds the 3× threshold. Sam Kaplan at 2.5× is the closest — monitor through April.

> Note: follow-up calls are not exclusively upsell-related. Because there is no dedicated call type for NB inbound calls, a rep following up on an inbound NB prospect will log it as `Call - Sales Follow-Up`. A high ratio may indicate chasing but could also reflect strong inbound demand being worked.

---

## Who Needs Attention ⚠️

**Michelle Frank — 0 outbound | 0 upsell meetings | 0 discovery calls | 144 emails**
Zero prospecting activity on every metric. Lowest email volume on the team. No visible selling motion all year.

**Emelie Schneider — 7 outbound calls | 1 upsell meeting | 4,815 emails (YTD)**
High email volume but minimal call activity. Working entirely from inbound/referral flow. Sustainable pipeline unclear.

**Juha Huttunen — 1 outbound call | 2 upsell meetings | 480 emails**
Minimal activity on all metrics.

**Scott Goodsir-Smyth — 8 outbound calls | 0 upsell meetings | 1,792 emails**
Low call volume. Likely in a different motion (no upsell in scope either).

**Sam Kaplan — Follow-up ratio 2.5× (borderline)**
Not yet a flag, but warrants a check on whether follow-up calls are structured outreach or reactive chasing.

---

## Data Quality Flags

**Calls logged on meetings object:**
- Sam Kaplan: 6 follow-up calls logged as meetings (2026 YTD)
- Sofia Bonicelli: 3 follow-up calls logged as meetings (2026 YTD)

These should be on the calls object. Flag to both reps each run.

**Call - Sales Legacy in active use:**
Sofia Bonicelli (52 YTD), Carlos Archanco (14). Should not be in use. Migrate to correct type.

**Kristyna Safrova (INACTIVE) — 509 outbound + 2,984 follow-up calls all in Mar 17+ window.** Audit HubSpot for bulk activity on owner 140964498 after Mar 17.

**Email data discrepancy — Emelie Schneider and Juha Huttunen:** Monthly query returns much lower figures than the YTD total from the original analysis. Likely a sequence email metadata issue. Flag for investigation.

---

## Per-AE Detail

---

### Sofia Bonicelli (264419305)

**TLDR:** Top outbound caller (274 YTD). Running a discovery-first motion (36 discovery calls). Strong March ramp (256 MTD). 52 legacy call logs — needs cleanup.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 9 | 9 | 256 | 274 |
| Discovery Calls | — | — | — | 36 |
| Meeting/Call - Upsell | 1 | 0 | 4 | 5 |
| Emails Sent | 96 | 958 | 8,180 | 9,234 |
| Follow-Up Calls | — | — | — | 166 |
| Call - Sales Legacy ℹ️ | — | — | — | 52 |

Follow-up ratio: 0.6× — healthy. 3 follow-up calls logged as meetings (data quality flag).

<details>
<summary>Outbound calls — past 30 days (15 calls: 9 answered, 2 voicemail, 4 no answer)</summary>

| Date | Time | Duration | Outcome |
|---|---|---|---|
| 2026-03-18 | 11:17 | 2:33 | Answered |
| 2026-03-18 | 11:13 | 1:30 | Answered |
| 2026-03-18 | 11:12 | — | No answer |
| 2026-03-18 | 11:00 | 0:21 | Answered |
| 2026-03-18 | 10:53 | 1:32 | Answered |
| 2026-03-18 | 10:32 | 1:57 | Answered |
| 2026-03-12 | 15:32 | 0:59 | Voicemail |
| 2026-03-12 | 15:01 | 1:40 | Answered |
| 2026-03-11 | 11:13 | — | Voicemail |
| 2026-03-06 | 09:29 | — | No answer |
| 2026-03-05 | 08:21 | — | No answer |
| 2026-02-24 | 15:41 | 0:43 | Answered |
| 2026-02-24 | 10:16 | — | No answer |
| 2026-02-24 | 10:04 | 1:46 | Answered |
| 2026-02-24 | 09:51 | 3:02 | Answered |

</details>

---

### Kirsty Freely (124826644)

**TLDR:** #1 by emails (11,675) and upsell meetings (21 YTD, 13 completed). Consistent outbound all 3 months. Strong all-round activity.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 22 | 12 | 201 | 235 |
| Discovery Calls | — | — | — | 10 |
| Meeting/Call - Upsell | 2 | 11 | 8 | 21 |
| Emails Sent | 2,843 | 325 | 8,507 | 11,675 |
| Follow-Up Calls | — | — | — | 269 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

Follow-up ratio: 1.1× — healthy. Note Feb email drop (325 vs 2,843 Jan) — possible sequence pause.

<details>
<summary>Outbound calls — past 30 days (49 calls: 22 answered, 15 voicemail, 10 no answer, 2 unknown)</summary>

| Date | Time | Duration | Outcome |
|---|---|---|---|
| 2026-03-19 | 11:34 | 1:14 | Voicemail |
| 2026-03-16 | 17:04 | 2:28 | Answered |
| 2026-03-11 | 15:43 | 2:26 | Answered |
| 2026-03-10 | 14:44 | — | No answer |
| 2026-03-10 | 09:34 | 0:44 | Voicemail |
| 2026-03-10 | 09:23 | 1:58 | Voicemail |
| 2026-03-04 | 17:10 | 7:08 | Answered |
| 2026-03-04 | 13:48 | — | Answered |
| 2026-03-04 | 13:33 | — | No answer |
| 2026-03-04 | 13:33 | — | No answer |
| 2026-03-03 | 16:09 | 0:45 | Answered |
| 2026-03-03 | 16:04 | 1:16 | Voicemail |
| 2026-03-03 | 14:10 | 6:15 | Answered |
| 2026-03-03 | 13:44 | 0:52 | Answered |
| 2026-03-03 | 13:40 | 1:11 | Answered |
| 2026-03-03 | 13:33 | 0:46 | Answered |
| 2026-03-03 | 13:26 | 0:39 | Answered |
| 2026-03-03 | 13:19 | 1:57 | Voicemail |
| 2026-03-03 | 13:16 | 0:03 | No answer |
| 2026-03-03 | 13:12 | 1:43 | Voicemail |
| 2026-03-03 | 13:08 | 0:28 | No answer |
| 2026-03-03 | 13:04 | 0:10 | No answer |
| 2026-03-03 | 13:03 | 0:59 | Voicemail |
| 2026-03-03 | 10:24 | 0:58 | Answered |
| 2026-03-03 | 09:57 | 1:31 | Answered |
| 2026-03-02 | 17:09 | 1:55 | Answered |
| 2026-03-02 | 17:06 | 0:12 | No answer |
| 2026-03-02 | 15:00 | 0:57 | Voicemail |
| 2026-03-02 | 14:59 | — | No answer |
| 2026-03-02 | 14:54 | 1:50 | Answered |
| 2026-03-02 | 14:53 | 0:40 | Answered |
| 2026-03-02 | 14:50 | 1:06 | Voicemail |
| 2026-03-02 | 14:47 | 1:06 | Voicemail |
| 2026-03-02 | 14:26 | 1:11 | Voicemail |
| 2026-03-02 | 14:19 | 1:36 | Voicemail |
| 2026-03-02 | 13:51 | 1:02 | Voicemail |
| 2026-03-02 | 13:41 | 4:14 | Answered |
| 2026-03-02 | 13:35 | — | No answer |
| 2026-03-02 | 13:30 | 0:38 | Answered |
| 2026-03-02 | 12:48 | 0:44 | Answered |
| 2026-03-02 | 12:39 | 0:58 | Voicemail |
| 2026-03-02 | 12:18 | 1:22 | Unknown |
| 2026-03-02 | 12:09 | 0:58 | Answered |
| 2026-02-25 | 17:11 | — | Unknown |
| 2026-02-25 | 11:19 | 1:03 | Voicemail |
| 2026-02-25 | 11:16 | 0:56 | No answer |
| 2026-02-24 | 13:45 | 1:43 | Answered |
| 2026-02-24 | 13:23 | 2:54 | Answered |
| 2026-02-24 | 13:12 | 2:01 | Answered |

</details>

---

### Alexandra Dias (82586810)

**TLDR:** All activity concentrated in March. 135 outbound calls MTD — strong start. 4 upsell meetings booked, none completed yet (all SCHEDULED). Confirm start date.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 135 | 135 |
| Discovery Calls | — | — | — | 1 |
| Meeting/Call - Upsell | 0 | 0 | 4 | 4 |
| Emails Sent | 0 | 0 | 1,779 | 1,779 |
| Follow-Up Calls | — | — | — | 60 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

Follow-up ratio: 0.4× — healthy.

<details>
<summary>Outbound calls — past 30 days (6 calls: 5 answered, 1 no answer)</summary>

| Date | Time | Duration | Outcome |
|---|---|---|---|
| 2026-03-23 | 10:38 | 2:23 | Answered |
| 2026-03-23 | 10:20 | 0:07 | No answer |
| 2026-03-11 | 15:01 | 1:49 | Answered |
| 2026-03-11 | 10:17 | 9:46 | Answered |
| 2026-02-23 | 12:26 | 3:00 | Answered |
| 2026-02-23 | 10:04 | 2:19 | Answered |

</details>

---

### Sam Kaplan (108125586)

**TLDR:** Strong March ramp (106 outbound MTD). Zero upsell meetings — all activity is NB motion. Follow-up ratio 2.5× — borderline, monitor. 6 follow-up calls logged as meetings (data quality issue).

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 6 | 6 | 106 | 118 |
| Discovery Calls | — | — | — | 1 |
| Meeting/Call - Upsell | 0 | 0 | 0 | 0 |
| Emails Sent | 164 | 284 | 3,121 | 3,569 |
| Follow-Up Calls | — | — | — | 297 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

Follow-up ratio: 2.5× — monitor. Email volume accelerating (Jan 164 → Feb 284 → Mar 3,121).

<details>
<summary>Outbound calls — past 30 days (43 calls: 21 answered, 17 voicemail, 3 no answer)</summary>

| Date | Time | Outcome |
|---|---|---|
| 2026-03-20 | 20:05 | Voicemail |
| 2026-03-20 | 19:04 | Voicemail |
| 2026-03-20 | 18:14 | Answered |
| 2026-03-19 | 19:19 | Answered |
| 2026-03-19 | 17:55 | Answered |
| 2026-03-18 | 20:11 | Answered |
| 2026-03-18 | 18:25 | Answered |
| 2026-03-18 | 18:23 | Answered |
| 2026-03-17 | 14:51 | Answered |
| 2026-03-17 | 14:39 | Answered |
| 2026-03-16 | 23:18 | Answered |
| 2026-03-16 | 17:11 | Answered |
| 2026-03-16 | 17:09 | Voicemail |
| 2026-03-16 | 17:07 | Answered |
| 2026-03-16 | 16:50 | Unknown |
| 2026-03-16 | 16:44 | Answered |
| 2026-03-16 | 15:46 | Voicemail |
| 2026-03-16 | 15:42 | No answer |
| 2026-03-16 | 15:32 | Answered |
| 2026-03-16 | 15:30 | Voicemail |
| 2026-03-16 | 14:23 | Answered |
| 2026-03-16 | 14:18 | Voicemail |
| 2026-03-09 | 20:46 | Voicemail |
| 2026-03-05 | 18:12 | Voicemail |
| 2026-03-05 | 17:49 | Voicemail |
| 2026-03-05 | 17:47 | Unknown |
| 2026-03-05 | 17:46 | Answered |
| 2026-03-05 | 17:44 | Voicemail |
| 2026-03-05 | 15:52 | Answered |
| 2026-03-05 | 15:16 | No answer |
| 2026-03-03 | 15:14 | Answered |
| 2026-03-03 | 15:10 | Voicemail |
| 2026-03-03 | 15:10 | Voicemail |
| 2026-03-03 | 15:05 | Answered |
| 2026-03-02 | 21:56 | No answer |
| 2026-03-02 | 21:56 | Voicemail |
| 2026-03-02 | 20:42 | Voicemail |
| 2026-03-02 | 20:42 | Answered |
| 2026-03-02 | 15:59 | Answered |
| 2026-02-27 | 20:49 | Voicemail |
| 2026-02-25 | 18:51 | Voicemail |
| 2026-02-24 | 16:32 | Voicemail |
| 2026-02-24 | 15:56 | Answered |

</details>

---

### Don Patrick Jakobsen (83717736)

**TLDR:** All 107 outbound calls in March — zero Jan/Feb. Confirm start date. Very low email volume (315). 1 upsell meeting completed in March.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 107 | 107 |
| Discovery Calls | — | — | — | 0 |
| Meeting/Call - Upsell | 0 | 0 | 1 | 1 |
| Emails Sent | 0 | 0 | 318 | 318 |
| Follow-Up Calls | — | — | — | 37 |
| Call - Sales Legacy ℹ️ | — | — | — | 2 |

Follow-up ratio: 0.3× — healthy.

<details>
<summary>Outbound calls — past 30 days (12 calls: 7 answered, 5 no answer)</summary>

| Date | Time | Duration | Outcome |
|---|---|---|---|
| 2026-03-20 | 09:00 | — | Answered |
| 2026-03-17 | 08:44 | 2:56 | Answered |
| 2026-03-17 | 08:38 | 0:02 | No answer |
| 2026-03-16 | 15:37 | 4:03 | Answered |
| 2026-03-16 | 15:31 | 0:09 | No answer |
| 2026-03-16 | 15:27 | 1:54 | Answered |
| 2026-03-16 | 15:24 | — | No answer |
| 2026-03-16 | 15:22 | 0:39 | Answered |
| 2026-03-16 | 15:20 | — | No answer |
| 2026-03-16 | 15:17 | 1:02 | Answered |
| 2026-03-16 | 15:12 | 0:05 | No answer |
| 2026-03-03 | 12:36 | 1:38 | Answered |

</details>

---

### Jessica Civitella (311286579)

**TLDR:** Ramped hard in March (88 outbound, 4,870 emails — vs near zero before). 8 upsell meetings YTD, 7 completed. Aircall user — 43/76 calls answered in past 30 days.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 1 | 88 | 89 |
| Discovery Calls | — | — | — | 2 |
| Meeting/Call - Upsell | 0 | 3 | 4 | 8 |
| Emails Sent | 139 | 432 | 4,870 | 5,441 |
| Follow-Up Calls | — | — | — | 164 |
| Call - Sales Legacy ℹ️ | — | — | — | 1 |

Follow-up ratio: 1.8× — acceptable. Note: Aircall reps have no duration logged (shown as —).

<details>
<summary>Outbound calls — past 30 days (76 calls: 43 answered, 16 voicemail, 14 no answer, 1 booked demo)</summary>

| Date | Time | Outcome |
|---|---|---|
| 2026-03-16 | 19:58 | Voicemail |
| 2026-03-13 | 19:02 | No answer |
| 2026-03-12 | 18:24 | No answer |
| 2026-03-10 | 19:08 | Answered |
| 2026-03-10 | 19:02 | Voicemail |
| 2026-03-10 | 18:15 | Answered |
| 2026-03-10 | 18:13 | Voicemail |
| 2026-03-10 | 18:09 | No answer |
| 2026-03-10 | 18:07 | Answered |
| 2026-03-10 | 18:03 | Answered |
| 2026-03-10 | 18:02 | Answered |
| 2026-03-10 | 18:00 | Answered |
| 2026-03-10 | 17:54 | Answered |
| 2026-03-10 | 17:26 | Answered |
| 2026-03-10 | 16:29 | Answered |
| 2026-03-10 | 16:24 | Answered |
| 2026-03-10 | 16:22 | Answered |
| 2026-03-10 | 16:19 | Answered |
| 2026-03-10 | 16:17 | Answered |
| 2026-03-10 | 16:15 | Voicemail |
| 2026-03-10 | 15:57 | Answered |
| 2026-03-10 | 15:54 | Answered |
| 2026-03-10 | 15:46 | No answer |
| 2026-03-10 | 15:43 | Voicemail |
| 2026-03-09 | 18:31 | No answer |
| 2026-03-09 | 18:27 | Answered |
| 2026-03-09 | 18:23 | Answered |
| 2026-03-09 | 18:05 | Answered |
| 2026-03-09 | 18:00 | Voicemail |
| 2026-03-09 | 17:58 | Answered |
| 2026-03-09 | 17:54 | Voicemail |
| 2026-03-09 | 17:52 | No answer |
| 2026-03-09 | 17:50 | No answer |
| 2026-03-09 | 17:47 | No answer |
| 2026-03-09 | 17:44 | Voicemail |
| 2026-03-09 | 17:35 | No answer |
| 2026-03-06 | 19:50 | Answered |
| 2026-03-04 | 17:45 | Answered |
| 2026-03-04 | 17:28 | Answered |
| 2026-03-04 | 17:16 | Voicemail |
| 2026-03-04 | 17:15 | Voicemail |
| 2026-03-04 | 17:09 | Answered |
| 2026-03-04 | 17:04 | Answered |
| 2026-03-04 | 16:58 | Answered |
| 2026-03-02 | 20:37 | Answered |
| 2026-03-02 | 20:35 | Answered |
| 2026-03-02 | 20:27 | Answered |
| 2026-03-02 | 20:22 | Answered |
| 2026-03-02 | 20:19 | Voicemail |
| 2026-03-02 | 20:18 | Answered |
| 2026-03-02 | 20:12 | Answered |
| 2026-03-02 | 20:09 | No answer |
| 2026-03-02 | 20:07 | Answered |
| 2026-03-02 | 20:04 | Answered |
| 2026-03-02 | 20:01 | Answered |
| 2026-03-02 | 20:00 | Voicemail |
| 2026-03-02 | 19:57 | Voicemail |
| 2026-03-02 | 19:54 | Voicemail |
| 2026-03-02 | 19:52 | Answered |
| 2026-03-02 | 19:49 | Answered |
| 2026-03-02 | 19:46 | No answer |
| 2026-03-02 | 19:43 | Answered |
| 2026-03-02 | 19:40 | Voicemail |
| 2026-03-02 | 19:38 | Answered |
| 2026-03-02 | 19:35 | Answered |
| 2026-03-02 | 19:32 | Answered |
| 2026-03-02 | 19:28 | No answer |
| 2026-03-02 | 19:26 | Voicemail |
| 2026-03-02 | 19:23 | Answered |
| 2026-03-02 | 19:18 | Answered |
| 2026-03-02 | 19:13 | Booked Demo |
| 2026-03-02 | 19:11 | Answered |
| 2026-03-02 | 19:08 | Answered |
| 2026-03-02 | 19:04 | No answer |
| 2026-03-02 | 19:02 | No answer |
| 2026-03-02 | 18:56 | Answered |

</details>

---

### Carlos Archanco (156289960)

**TLDR:** Highest discovery call count (75) and 6 upsell meetings — but all from January. Outbound slowing in March (31 MTD). 14 legacy call logs. Zero outbound in past 30 days in this data batch.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 21 | 26 | 31 | 78 |
| Discovery Calls | — | — | — | 75 |
| Meeting/Call - Upsell | 6 | 0 | 0 | 6 |
| Emails Sent | 194 | 1,664 | 6,169 | 8,027 |
| Follow-Up Calls | — | — | — | 77 |
| Call - Sales Legacy ℹ️ | — | — | — | 14 |

Follow-up ratio: 1.0× — healthy. No outbound calls in past 30 days retrieved in this batch — may be due to pagination cut-off on high-volume team query.

<details>
<summary>Outbound calls — past 30 days (not retrieved in this batch — see full HubSpot call log)</summary>

Carlos Archanco had 31 outbound calls logged in Mar MTD per the YTD totals. The team-wide query pagination did not retrieve these records. View directly in HubSpot filtered to owner 156289960.

</details>

---

### Michelle Frank (85529907) ⚠️

**TLDR:** Zero activity on every metric all year. 144 emails, all in March. No prospecting motion visible. Immediate 1:1 required.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 0 | 0 |
| Discovery Calls | — | — | — | 0 |
| Meeting/Call - Upsell | 0 | 0 | 0 | 0 |
| Emails Sent | 0 | 0 | 144 | 144 |
| Follow-Up Calls | — | — | — | 0 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

<details>
<summary>Outbound calls — past 30 days (0 calls)</summary>

No outbound calls logged in the past 30 days.

</details>

---

### Emelie Schneider (181769737)

**TLDR:** High email volume (4,815 YTD per original analysis) but only 7 outbound calls. Working from inbound/referral flow. 1 upsell meeting completed.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 1 | 6 | 7 |
| Discovery Calls | — | — | — | 7 |
| Meeting/Call - Upsell | 0 | 1 | 0 | 1 |
| Emails Sent | 62 | 79 | 481 | 622 ⚠️ |
| Follow-Up Calls | — | — | — | 8 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

⚠️ Email monthly total (622) does not match YTD figure (4,815). Likely a sequence metadata issue — investigate.

<details>
<summary>Outbound calls — past 30 days (1 call: 1 no answer)</summary>

| Date | Time | Duration | Outcome |
|---|---|---|---|
| 2026-03-05 | 08:48 | 0:04 | No answer |

</details>

---

### Juha Huttunen (37634691)

**TLDR:** Minimal outbound activity (1 call YTD). 2 upsell meetings completed in March. Email data discrepancy — monthly query shows 0, YTD was 480.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 1 | 0 | 1 | 1 |
| Discovery Calls | — | — | — | 0 |
| Meeting/Call - Upsell | 0 | 0 | 2 | 2 |
| Emails Sent | 0 | 0 | 0 | 480 ⚠️ |
| Follow-Up Calls | — | — | — | 0 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

⚠️ Monthly email query returns 0 for all periods despite YTD total of 480. Flag for investigation.

<details>
<summary>Outbound calls — past 30 days (0 calls)</summary>

No outbound calls logged in the past 30 days.

</details>

---

### Scott Goodsir-Smyth (96216654)

**TLDR:** Low call volume (8 YTD). No upsell meetings. Emails accelerating in March (1,474 MTD vs 265 in all of Q4 2025). May be in a different motion.

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 8 | 8 |
| Discovery Calls | — | — | — | 0 |
| Meeting/Call - Upsell | 0 | 0 | 0 | 0 |
| Emails Sent | 125 | 193 | 1,474 | 1,792 |
| Follow-Up Calls | — | — | — | 0 |
| Call - Sales Legacy ℹ️ | — | — | — | 0 |

<details>
<summary>Outbound calls — past 30 days (0 calls)</summary>

No outbound calls logged in the past 30 days.

</details>

---

### Kristyna Safrova (140964498) — INACTIVE ⚠️

| Metric | Jan | Feb | Mar MTD | YTD |
|---|---|---|---|---|
| Outbound Calls | 0 | 0 | 509* | 509* |
| Emails Sent | — | — | — | 861 |
| Follow-Up Calls | — | — | — | 2,984* |

⚠️ INACTIVE rep. All 509 outbound calls and 2,984 follow-up calls appear entirely within the Mar 17+ window. Likely a data migration or re-attribution event. Excluded from all team metrics. Audit required.

---

*Report generated: 2026-03-23 | Data source: HubSpot MCP live pull | YTD = Jan 1 – Mar 23 2026 | GitHub: jeanmascre-cmd/sales-activity-march-2026*
