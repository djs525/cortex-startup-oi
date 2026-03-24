# Cortex
**The operating intelligence for startups — powered by Claude + Notion MCP**

---

Type `run Cortex`. In under 60 seconds, Claude reads your deals, goals, investors, and hiring pipeline — then writes your entire weekly company review into Notion. No manual input. No context needed. Just two words.

That's what superpowers feel like.

---

## What it does

Cortex is a system prompt that turns Claude into an autonomous operating agent for your startup. Connected to your Notion workspace via MCP, it runs on natural language commands:

| Command | Result |
|---|---|
| `run Cortex` | Full weekly review written to Notion — health scored, all 8 sections populated |
| `stale deals` | Pipeline scanned, silent deals flagged, personalised follow-up emails drafted |
| `investor check` | Overdue investor follow-ups surfaced with drafted messages |
| `loss analysis` | Closed-lost deals scanned for product and pricing patterns |
| `activate [MODULE]` | Plug in Engineering, Product, People, or Finance as your team grows |
| `health check` | Verify all databases are connected and readable |

Full command list: [`system-prompt/COMMANDS.md`](system-prompt/commands.md)

---

## Why it's different

Every other Notion OS is a static template. Cortex reads your workspace and **acts** on it.

It connects what nobody manually connects — a stale deal linked to an at-risk OKR, an investor who asked for a demo video 13 days ago that still hasn't been sent, a hiring role open for 35 days blocking a revenue goal. That cross-database intelligence is what makes it feel like a co-founder, not a search tool.

And it scales. A 3-person startup activates Stage 1 and has a complete operating system. As the team grows, modules plug in one at a time — same commands, more signal.

---

## How it's built

**Layer 1 — Notion workspace.** 5 linked databases (OKRs, Sales, Investors, Hiring, Weekly Review) wired with relations and rollups. Company Pulse dashboard pulls everything into one view.

**Layer 2 — System prompt.** Plain-English instructions loaded into Claude Desktop or a Claude Project. Defines the workspace map, trigger commands, health scoring logic, and writing rules. The program, written in English instead of Python.

**Layer 3 — Claude via Notion MCP.** Reads every database, cross-references across all of them, writes pages back to Notion. The intelligence layer.

**Lines of code written: 0**

---

## The demo

Watch `run Cortex` live → [Demo video](#) *(added after recording)*

Duplicate the template and try it yourself:
👉 **[Get the Cortex Notion template](#https://cortex-startup-os.notion.site/Cortex-Startup-OS-Template-32c722f645ad81159441c7e947394d35)** 

---

## Get started

1. [Build your Notion workspace](getting-started/1-build-your-notion-workspace.md) — ~30 min
2. [Connect Notion MCP](getting-started/2-connect-notion-mcp.md) — ~5 min
3. [Install the system prompt](getting-started/3-install-system-prompt.md) — ~10 min
4. [Run your first workflow](getting-started/4-run-your-first-workflow.md) — type `run Cortex`

---

## Repo structure

```
cortex-os/
├── README.md
├── DEMO.md                               ← demo script
├── system-prompt/
│   ├── cortex-system-prompt-template.md  ← copy into Claude, fill in your IDs
│   └── COMMANDS.md                       ← all 15 commands
├── getting-started/                      ← step-by-step setup guides
└── modules/                              ← database specs per team module
```

---

*Built for the MLH Notion AI Challenge 2026 · Powered by Claude · Notion MCP · Notion*
