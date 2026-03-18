# Cortex — Module Reference

All modules are inactive by default. Run `activate [MODULE NAME]` and Cortex walks you through setup.

---

## Founder Core — Stage 1 · Active from day 1

**Databases:** OKR Tracker · Sales Pipeline · Investor CRM · Hiring Pipeline · Weekly Review

**Cortex monitors:** Goal health · Deal staleness · Investor follow-ups · Hiring bottlenecks · Weekly company health

**Commands:** `run Cortex` · `full briefing` · `company status` · `stale deals` · `pipeline health` · `loss analysis` · `investor check` · `draft investor update` · `hiring check` · `OKR check`

See [`getting-started/01-build-your-notion-workspace.md`](../getting-started/01-build-your-notion-workspace.md) for full setup.

---

## Engineering — Stage 2

**Activate when:** You hire your first engineer or engineering lead.

**Adds:** Sprint tracking, bug management, engineering work linked to OKRs. Cortex includes engineering health in weekly reviews and flags blocked items.

| Property | Type | Purpose |
|---|---|---|
| Sprint / Task | Title | Work item name |
| Type | Select | Feature · Bug · Chore · Spike |
| Status | Select | Backlog · In Progress · Review · Done · Blocked |
| Priority | Select | Critical · High · Normal · Low |
| Sprint | Select | Sprint 1 · Sprint 2 · etc. |
| Assignee | Person | Owner |
| Due date | Date | Expected completion |
| Linked OKR | Relation | → OKR Tracker DB |
| Notes | Text | Context, blockers, PR links |

**New command:** `sprint check` — blocked items, completion %, OKR linkage health.

---

## Product — Stage 2

**Activate when:** You have a dedicated PM or significant product strategy work.

**Adds:** Roadmap visibility, feature-to-OKR linkage, customer demand tracking. Cortex surfaces misalignment between roadmap and what's blocking deals.

| Property | Type | Purpose |
|---|---|---|
| Feature | Title | Feature or initiative name |
| Status | Select | Now · Next · Later · In Review · Shipped · Cut |
| Priority score | Number | 1–10 |
| Owner | Person | PM or founder |
| Linked OKR | Relation | → OKR Tracker DB |
| Linked deals | Relation | → Sales Pipeline DB |
| Customer request count | Number | How many asked for this |
| Notes | Text | Spec context, decisions |

**New command:** `roadmap check` — features blocking deals, OKR gaps, top customer requests stuck in Later.

---

## People — Stage 3

**Activate when:** You have 10+ people or hire a People function.

**Adds:** 1:1 tracking, sentiment monitoring, team health. Cortex flags overdue 1:1s and at-risk team members early.

| Property | Type | Purpose |
|---|---|---|
| Team member | Title | Person's name |
| Role | Text | Job title |
| Team | Select | Engineering · Product · Sales · Marketing · Ops |
| Last 1:1 | Date | Date of last one-on-one |
| Next 1:1 | Date | Next scheduled meeting |
| Sentiment | Select | Great · Good · Neutral · Concerned · At Risk |
| Linked OKR | Relation | → OKR Tracker DB |
| Notes | Text | 1:1 notes, feedback, goals |

**New command:** `team check` — overdue 1:1s, at-risk sentiment, people without linked OKRs.

---

## Finance — Stage 3

**Activate when:** You've raised a round or need runway visibility.

**Adds:** Monthly financial tracking, runway monitoring, burn alerts. Cortex flags runway below 6 months as 🔴 Critical — early enough to act.

| Property | Type | Purpose |
|---|---|---|
| Month | Title | e.g. "March 2026" |
| Revenue | Number | MRR or ARR |
| Burn | Number | Total monthly spend |
| Runway (months) | Number | Cash / monthly burn |
| Headcount | Number | Total employees |
| Target vs actual | Select | Ahead · On target · Behind |
| Linked OKR | Relation | → OKR Tracker DB |
| Notes | Text | Variance context |

**New command:** `finance check` — runway status, burn trend, revenue vs OKR target.

---

## Marketing — Stage 2/3

**Activate when:** You have a dedicated marketing person or multiple simultaneous campaigns.

**Adds:** Campaign tracking, spend efficiency, lead attribution. Cortex flags campaigns with no OKR link and channels generating the most pipeline.

| Property | Type | Purpose |
|---|---|---|
| Campaign | Title | Campaign name |
| Status | Select | Planning · Live · Complete · Paused |
| Channel | Select | Content · Paid · Email · Events · SEO · Social |
| Owner | Person | Who runs this |
| Budget | Number | Allocated spend |
| Leads generated | Number | Attributed pipeline entries |
| Linked OKR | Relation | → OKR Tracker DB |
| Notes | Text | Results, learnings |

**New command:** `marketing check` — campaign performance, spend efficiency, OKR coverage gaps.

---

## When to activate

| Situation | Activate next |
|---|---|
| First engineer hired | Engineering |
| Dedicated PM or product focus | Product |
| Multiple campaigns running | Marketing |
| 10+ people, managing team health | People |
| Raised a round or significant revenue | Finance |
| Just starting | Stay on Stage 1 |

The right time to activate a module is when you catch yourself manually tracking that information somewhere else.

---

*Cortex — the operating intelligence for startups.*
