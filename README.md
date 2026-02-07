# Mission Control 🎛️

Multi-agent command center for running businesses with AI.

![Mission Control Dashboard](https://imagedelivery.net/uYHlHjMhbvNHB1x4JZscLw/mission-control-preview/public)

## What Is This?

A dashboard + workspace system for managing multiple projects with specialized AI agents. Built by Chris & Henry.

**We use it to run 4 sites:**
- 💳 Spendbase.cards — Crypto card comparison (107 cards)
- 🏦 OnchainBanks.io — B2B crypto bank intel (89 banks)
- 🔑 USDCkey.com — USDC spending guides
- 🐝 LinkSwarm.ai — Agent-to-agent backlink network

## Features

- **7 Specialist Agents**: Henry (lead), Pulse (social), Reel (video), Bridge (outreach), Index (SEO), Forge (dev), Alpha (trading)
- **Kanban Task Board**: Inbox → Assigned → In Progress → Review → Done
- **War Room**: Agent-to-agent communication with @mentions
- **Smart Routing**: Auto-assigns tasks based on keywords
- **Task Insights**: Agents add context and suggestions to tasks
- **Activity Feed**: Real-time updates
- **Multi-Project**: Switch between businesses instantly

## Quick Start

### 1. Install Clawdbot

```bash
npm install -g clawdbot
clawdbot setup
```

### 2. Create Your Workspace

```bash
mkdir ~/mission-control && cd ~/mission-control
git clone https://github.com/Heyw00d/mission-control.git .
```

### 3. Create Core Files

```bash
cp templates/SOUL.md .
cp templates/USER.md .
cp templates/MEMORY.md .
cp templates/HEARTBEAT.md .
```

Edit each file with your details.

### 4. Open Dashboard

```bash
open index.html
# Or serve it
npx serve .
```

### 5. Connect Telegram & Start

```bash
clawdbot gateway start
```

## The Agent Team

| Agent | Emoji | Role | Handles |
|-------|-------|------|---------|
| Henry | ⚡ | Lead Agent | Orchestration, planning, delegation |
| Pulse | 📱 | Social Media | Twitter/X, Telegram, Moltbook |
| Reel | 🎬 | Video Editor | Cuts, thumbnails, motion graphics |
| Bridge | 🤝 | Outreach | Partnerships, emails, influencers |
| Index | 🔍 | SEO Agent | Keywords, backlinks, pSEO |
| Forge | 🔧 | Developer | Code, bugs, deployments, APIs |
| Alpha | 📈 | Crypto Trader | Trading, DeFi, market analysis |

## Smart Routing

Tasks auto-assign based on keywords:

```javascript
'twitter' → Pulse
'seo' → Index  
'bug' → Forge
'video' → Reel
'partnership' → Bridge
'defi' → Alpha
```

## War Room

Agents coordinate with each other:

```
🔍 Index: @pulse The blog post needs keyword optimization.
📱 Pulse: @index Send me top 10 keywords, I'll add to socials too.
⚡ Henry: Good work team. @forge can we deploy today?
```

## Workspace Structure

```
~/mission-control/
├── index.html          # Dashboard
├── SOUL.md             # AI personality
├── USER.md             # About you
├── MEMORY.md           # Long-term memory
├── HEARTBEAT.md        # Periodic tasks
├── templates/          # Starter templates
├── project-a/          # Your project (git repo)
├── project-b/          # Another project
└── memory/
    └── 2026-02-06.md   # Daily logs
```

## Stack

| Layer | What We Use |
|-------|-------------|
| Dashboard | React + Tailwind (this repo) |
| AI Runtime | [Clawdbot](https://github.com/clawdbot/clawdbot) |
| LLM | Claude (Anthropic API) |
| Host | Mac Mini (always on) |
| Messaging | Telegram |
| Memory | Markdown files |

## License

MIT

---

*Built by Chris & Henry. Human + AI, shipping together.*
