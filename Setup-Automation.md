# Cortex — Automated Setup

Instead of 40–60 minutes of manual database building, type one command and Claude builds most of the workspace for you.

---

## How it works

```
setup Cortex
```

That's it. Claude runs a 6-phase automated setup:

| Phase | What Claude does | Time |
|---|---|---|
| 1 | Creates all 6 parent pages with icons | ~10 sec |
| 2 | Creates all 5 databases | ~15 sec |
| 3 | Populates with realistic sample data | ~20 sec |
| 4 | Creates Weekly Review template with 8 sections | ~10 sec |
| 5 | Builds Company Pulse dashboard structure | ~10 sec |
| 6 | Generates personalised setup checklist with your database IDs pre-filled | ~10 sec |

**Total automated time:** ~75 seconds

---

## What Claude can't automate

Notion MCP can create pages and rows but can't modify database schemas. Three things still require ~5 minutes of manual work:

**1. Add property schemas** (~3 min)
Each database needs its properties configured — select options, date fields, number formats. Claude provides the exact property list for each database.

**2. Wire the relations** (~1 min)
Sales Pipeline → Linked OKR → OKR Tracker DB
Hiring Pipeline → Linked OKR → OKR Tracker DB

**3. Share pages with the integration** (~1 min)
For each database: `...` → Connect to → Cortex integration

---

## What you get

By the time automated setup completes, you have:

- ✅ All 6 pages created with correct structure
- ✅ All 5 databases with sample data
- ✅ 2 stale deals pre-configured for the stale deal demo
- ✅ 1 At Risk OKR pre-configured for the health check demo
- ✅ 1 investor in Due Diligence for the investor alert demo
- ✅ Weekly Review template ready
- ✅ Your personalised system prompt with database IDs already filled in
- ⬜ Properties to add (~3 min)
- ⬜ Relations to wire (~1 min)
- ⬜ Pages to share with integration (~1 min)

**Total setup time with automation: ~10 minutes vs 60 minutes manually.**

---

## The setup checklist Claude generates

After running `setup Cortex`, Claude creates a `⚡ Cortex Setup Checklist` page in your workspace containing:

1. Your exact database IDs (copied from the just-created databases)
2. A fully filled-in system prompt — paste directly into Claude, no placeholder hunting
3. Step-by-step instructions for the 3 remaining manual steps with exact UI navigation

---

## After automated setup

Once you've completed the 3 manual steps, type:

```
health check
```

Claude verifies every database is accessible and readable. Fix any ❌ errors, then:

```
run Cortex
```

Your first weekly review is generated from live workspace data. You're live.

---

*Cortex — the operating intelligence for startups.*
