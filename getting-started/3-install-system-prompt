# Step 3 — Install the system prompt

**Time:** ~10 minutes · No technical experience required

---

## What it does

The system prompt is Cortex's brain. It tells Claude what databases exist, what every command means, how to score health, and how to write. Without it you'd explain everything every session. With it loaded, `run Cortex` just works.

---

## Step 1 — Find your database IDs

Open each database in Notion, copy the URL. The UUID in the URL is the ID.

```
https://notion.so/yourworkspace/326722f6-45ad-807a-b0e5-dfd0472eb89d
                                ↑ this is your database ID
```

Collect IDs for:
- [ ] OKR Tracker DB
- [ ] Sales Pipeline DB
- [ ] Investor CRM DB
- [ ] Hiring Pipeline DB
- [ ] Weekly Review DB
- [ ] Company Pulse page
- [ ] Sales Pipeline parent page
- [ ] Investor CRM parent page

---

## Step 2 — Fill in the template

Open [`cortex-system-prompt-template.md`](cortex-system-prompt-template.md). Find and replace:

| Placeholder | Replace with |
|---|---|
| `[YOUR_COMPANY_NAME]` | Your startup's name |
| `[YOUR_OKR_DB_ID]` | OKR Tracker data source ID |
| `[YOUR_SALES_DB_ID]` | Sales Pipeline data source ID |
| `[YOUR_INVESTOR_DB_ID]` | Investor CRM data source ID |
| `[YOUR_HIRING_DB_ID]` | Hiring Pipeline data source ID |
| `[YOUR_WEEKLY_DB_ID]` | Weekly Review data source ID |
| `[YOUR_PULSE_PAGE_ID]` | Company Pulse page ID |
| `[YOUR_SALES_PAGE_ID]` | Sales Pipeline parent page ID |
| `[YOUR_INVESTOR_PAGE_ID]` | Investor CRM parent page ID |

Leave all `INACTIVE` module placeholders as-is — fill them in when you activate each module.

---

## Step 3 — Load into Claude

**Claude Desktop:** Settings → Custom Instructions → paste → Save

**Claude Project:** Open project → Edit Instructions → paste → Save

Open a **new conversation** after saving — existing ones won't pick up the new instructions.

---

## Step 4 — Verify

In the new conversation, type:

```
module status
```

You should see a table with 5 ACTIVE modules and 4 INACTIVE. If so, the system prompt is loaded correctly.

→ **Next: [04-run-your-first-workflow.md](04-run-your-first-workflow.md)**
