# Step 2 — Connect Notion MCP

**Time:** ~5–10 minutes · No technical experience required

---

## What is Notion MCP?

MCP (Model Context Protocol) lets Claude take actions inside Notion — reading databases, creating pages, updating records. This is what turns Cortex from a chat assistant into an operating agent.

---

## Option A — Claude Desktop (recommended)

1. Download [Claude Desktop](https://claude.ai/download)
2. Settings → Connections → find **Notion** → Connect
3. Log into your Notion account, select your **Cortex workspace**
4. Approve access

---

## Option B — Claude Project

1. [claude.ai](https://claude.ai) → Projects → New Project → name it `Cortex`
2. In the project, enable Notion via the connections/tools panel
3. Authenticate and select your Cortex workspace
4. Paste your system prompt into Project Instructions (see Step 3)

---

## Share pages with the integration

**This is the step most people miss.** After connecting, Notion requires you to explicitly share pages.

For every database: open the page → `...` → **Connect to** → select your Claude integration.

Do this for: Company Pulse, OKR Tracker, Sales Pipeline, Investor CRM, Hiring Pipeline, Weekly Review — **and their child databases**.

> Skipping this causes "object not found" errors even with a valid connection.

---

## Verify

In a new Claude session, type:

```
health check
```

Cortex will report which databases are accessible, empty, or inaccessible.

→ **Next: [03-install-system-prompt.md](03-install-system-prompt.md)**
