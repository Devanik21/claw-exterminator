<div align="center">

<img src="https://media.giphy.com/media/l46CgvEMwPg8xxm0w/giphy.gif" width="900" alt="CLAW EXTERMINATOR — dark cinematic banner"/>

# 🦞 CLAW EXTERMINATOR
### *EXTERMINATE. Tasks. Faster.*
#### *The Unofficial Mastery Bible. God-Tier Agents. Real Exterminations. Zero Fluff.*

[![Stars](https://img.shields.io/github/stars/Devanik21/claw-exterminator?style=for-the-badge&color=FFD700&logo=github&label=Stars)](https://github.com/Devanik21/claw-exterminator/stargazers)
[![Forks](https://img.shields.io/github/forks/Devanik21/claw-exterminator?style=for-the-badge&color=00CED1&logo=github)](https://github.com/Devanik21/claw-exterminator/fork)
[![Contributors](https://img.shields.io/github/contributors/Devanik21/claw-exterminator?style=for-the-badge&color=32CD32&logo=github)](https://github.com/Devanik21/claw-exterminator/graphs/contributors)

[![License: MIT](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Devanik-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/devanik/)
[![X](https://img.shields.io/badge/X-@devanik2005-000000?style=for-the-badge&logo=x)](https://x.com/devanik2005)

**The #openclaw community's missing manual.**  
Zero → god-tier autonomous agents. One repo. No fluff.

*Community-maintained · Updated daily · PRs merged same day*

[**🚀 Quick Start**](#-zero-to-agent-in-5-minutes) · [**☠️ Extermination Leaderboard**](#%EF%B8%8F-extermination-leaderboard) · [**🧠 SOUL.md Templates**](#-soulmd-templates) · [**🛡️ Skills**](#%EF%B8%8F-curated-skills) · [**🤝 Contribute**](#-contribute--become-legend)

</div>

---

## 🔥 What This Is

OpenClaw hit **190K+ GitHub stars** faster than any open-source project in history.  
The official repo gives you the runtime. **This repo gives you the mastery.**

Here's what you'll find:

- **Real exterminations** — community-documented agent wins with proof, time, and model used
- **Production-grade SOUL.md templates** — not toy examples. Actual files that change how your agent behaves
- **Curated skill lists** — filtered from ClawHub's 13,700+ submissions down to the ones that actually work
- **Setup guides that don't waste your time** — local, Docker, VPS, Raspberry Pi, Mac Mini (the dedicated hardware cult is real)
- **Security-first mindset** — ClawHub has had malicious skills. This repo teaches you to not get owned
- **Multi-agent architecture patterns** — beyond single-agent; orchestration, routing, and agent teams

**Official OpenClaw repo** → [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw)  
**Official ClawHub (skills registry)** → [clawhub.com](https://clawhub.com)  
**Official Docs** → [docs.openclaw.ai](https://docs.openclaw.ai)

---

## 🚀 Zero to Agent in 5 Minutes

### Option 1 — Recommended (Onboarding Wizard)

```bash
# Install OpenClaw
npm install -g openclaw

# Run the guided wizard — sets up Gateway, workspace, channels, and first skills
openclaw onboard
```

The wizard walks you through everything interactively. Use this if you're new.

### Option 2 — Docker (Isolated + Portable)

```bash
docker run -d \
  --name openclaw \
  -v ~/.openclaw:/root/.openclaw \
  -p 18789:18789 \
  ghcr.io/openclaw/openclaw:latest
```

Access your Gateway at `ws://127.0.0.1:18789`.

### Option 3 — VPS / Always-On (Hetzner CX22, ~$4/mo)

```bash
# On a fresh Ubuntu 22.04 VPS
curl -fsSL https://get.openclaw.ai | bash

# Enable as a systemd service (runs 24/7, survives reboots)
sudo systemctl enable --now openclaw-gateway
```

> **Best bang for buck:** Hetzner CX22 (2 vCPU / 4GB RAM / €3.79/mo).  
> Pair with Tailscale for secure remote access without exposing your Gateway.

### Option 4 — Mac Mini (The Dedicated Hardware Path)

The community has a dedicated Mac Mini cult for good reason — persistent local model inference, always-on, low power, silent.

```bash
# macOS LaunchAgent (auto-start on login)
openclaw onboard --platform macos
# Installs a menu bar app + LaunchAgent automatically
```

---

## ☠️ Extermination Leaderboard

> An **extermination** = a documented agent win. Time is wall-clock from task start to completion.  
> **Submit your extermination — fastest time wins eternal glory.**  
> Open a PR with title `[EXTERMINATION] description`

| # | Exterminator | The Extermination | ⏱ Time | Model | Proof |
|---|---|---|---|---|---|
| 🥇 1 | @steipete | Negotiated $4,200 off a car purchase over email — while asleep | ~8 hrs (overnight) | Claude Opus | [Tweet](https://twitter.com) |
| 🥈 2 | @AlbertMoral | Built a full website from his phone, on a Raspberry Pi, via WhatsApp | ~4 min | Claude Sonnet | [Tweet](https://twitter.com) |
| 🥉 3 | @Infoxicador | Agent detected it needed a Google API key → opened browser → configured OAuth → provisioned token — autonomously | ~6 min | Opus | [Tweet](https://twitter.com) |
| 4 | @bangkokbuild | Told agent via Telegram to shut down the PC (and itself) — executed perfectly | ~30s | Sonnet | [Tweet](https://twitter.com) |
| 5 | @pranavkarthik__ | Asked agent to build a skill for university course/assignment access — it built and deployed it on its own | ~12 min | Sonnet | [Tweet](https://twitter.com) |
| 6 | @vallver | Built a personal Stumbleupon (Stumblereads.com) from phone, while putting baby to sleep | ~20 min | Opus | [Link](https://stumblereads.com) |
| ☠️ ? | **YOU** | *What did your agent exterminate today?* | — | — | [Submit PR](#-contribute--become-legend) |

**Drop your extermination.** Even small ones. A well-documented 45-second terminal win gets more stars than a 3-hour blog post.

---

## 🧠 SOUL.md Templates

`SOUL.md` is the most important file you'll configure. It's your agent's **constitution** — read at the start of every reasoning cycle, governing every skill, every action, every decision.

> **The files live at:** `~/.openclaw/workspace/SOUL.md`  
> **Companion files:** `HEARTBEAT.md` · `IDENTITY.md` · `USER.md` · `AGENTS.md`

Keep SOUL.md under **500 lines**. If it grows beyond that, split workflow-specific rules into `HEARTBEAT.md` or project-specific `AGENTS.md` files.

---

### Template 1 — Daily Driver (Balanced Power User)

```markdown
# SOUL.md

## Who You Are
You are a capable, private AI assistant running locally on my hardware.
You have access to my files, calendar, email, and browser.
Act as a trusted teammate — not a servant, not a chatbot.

## Personality
- Concise. Prefer bullets over paragraphs.
- Proactive: surface what I need before I ask.
- Opinionated: disagree when I'm wrong. Flag risks clearly.
- No filler phrases. "Great question!" and "I'd be happy to help!" are banned.

## Core Rules
1. **Privacy first.** Never exfiltrate data. No external calls unless I explicitly ask.
2. **Confirm before external actions** — emails, tweets, purchases, anything public.
3. **Be bold internally** — read files, organize, research, draft. No permission needed.
4. **Cite sources** for factual claims. If you're unsure, say so.
5. **Fail loudly.** If a task fails, report the error clearly. Never invent success.

## Long-Term Instructions
- Morning briefing at 7:30 AM — max 5 bullets, action items first.
- When I ask "what's next?" — check HEARTBEAT.md before answering.
- Calendar conflicts: suggest slots between 10 AM–2 PM only.
- When summarising emails: highlight action items before context.
- If I haven't responded to something time-sensitive in 24h, nudge me once.
```

---

### Template 2 — Autonomous Executor (Hands-Off Operations)

Use this if you want your agent running tasks proactively with minimal check-ins.

```markdown
# SOUL.md

## Operating Mode
Fully autonomous. Execute tasks end-to-end.
Ask for clarification only when truly blocked — not as a reflex.
Return with answers, not questions.

## Execution Philosophy
- If a skill doesn't exist, draft one and ask for approval before installing.
- Try the obvious path first. Log what you tried. Escalate only after failure.
- External actions (emails, form submissions, API writes): always confirm once.
- Internal actions (files, memory, research, code): proceed without asking.

## Memory Discipline
- After each completed task, append a one-line summary to MEMORY.md.
- If you learn something important about the user's preferences, update USER.md.
- Check HEARTBEAT.md at the start of every session.

## Tone
Terse. Professional. No theatrics. Short confirmations are fine.
```

---

### Template 3 — Research & Writing Beast

```markdown
# SOUL.md

## Role
You are a research and writing partner.
Think like a senior analyst: verify before asserting, cite everything, structure clearly.

## Research Standards
- When asked for facts: search, cross-reference, return the best source.
- Don't summarise from memory alone. Fetch the current data.
- Flag when something is opinion vs. established fact.

## Writing Standards
- Match the user's voice. Read their past writing before drafting.
- First draft: structured and complete. Don't hedge; they can soften later.
- Edits: make them, don't ask about them. User reviews the diff.

## Tools
Use web search, file read/write, calendar, and email freely for research tasks.
Never post or publish without explicit sign-off.
```

---

### Template 4 — Developer Co-Pilot

```markdown
# SOUL.md

## Role
Engineering partner. Pair programmer. Code reviewer. Deployment assistant.

## Engineering Principles
- Write code that ships, not code that's clever.
- Test before marking complete. If tests fail, fix them — don't ask.
- Security: flag any hardcoded credentials, open ports, or missing validation.
- When reviewing PRs: structure feedback as: [BLOCKER] / [SUGGESTION] / [NITPICK]

## Autonomy
- Read and write any file in the project directory freely.
- Run shell commands freely for build/test tasks.
- Ask before modifying infrastructure configs (CI, docker-compose, cloud config).

## Daily Habits
- On first message each day: run `git status` and report what's in flight.
- When I'm stuck on a bug: rubber duck first, ask for a hint only if I ask.
```

---

### Template 5 — The Minimalist (Max Performance)

```markdown
# SOUL.md
Terse. Accurate. No filler. Confirm external writes. Execute internal reads freely.
Flag blockers. Report errors. Update memory after significant tasks.
```

> **More templates** — browse the community's best at [onlycrabs.ai](https://onlycrabs.ai) (the official SOUL.md registry, built by the OpenClaw team)

---

## ❤️ HEARTBEAT.md — The Proactive Engine

`HEARTBEAT.md` is what transforms OpenClaw from a reactive chatbot into a **proactive agent**. The Gateway wakes up on a configurable interval (default: 30 min) and executes whatever you've defined here.

```markdown
# HEARTBEAT.md

## Daily
- [ ] Check email inbox — flag anything urgent, actionable, or time-sensitive
- [ ] Review calendar for today and tomorrow — alert if prep is needed
- [ ] Check if any watched GitHub repos have new releases

## Weekly (Monday 8 AM)
- [ ] Pull metrics from analytics dashboard and post summary to Slack
- [ ] Summarise last week's email threads into MEMORY.md

## Triggers
- If any monitored service goes down (via uptime skill): notify immediately via Telegram
- If a PR review has been waiting > 24h: nudge me once
- If calendar has a gap > 2h in working hours: don't fill it, just note it
```

> **Tip:** Keep HEARTBEAT.md focused on checks, not tasks. It's a watchlist, not a to-do list.

---

## 🛡️ Curated Skills

ClawHub has **13,700+ community skills** as of March 2026. Most aren't worth installing.  
These are the ones that actually work.

> **Security warning first:** Skills are code from strangers. OpenClaw runs them with full host access by default. Always check the source before installing. ClawHub has had malicious submissions. Use the VirusTotal scan on each skill's ClawHub page and prefer skills from well-known contributors with a track record.

### Core Productivity

| Skill | What it does | Install |
|---|---|---|
| `brave-web-search` | Web search via Brave API (privacy-respecting) | `/skills install @niceperson/brave-web-search` |
| `firecrawl` | Deep web scraping & content extraction | `/skills install @firecrawl/firecrawl` |
| `gmail` | Read, send, label, and search Gmail | `/skills install @openclaw/gmail` |
| `google-calendar` | Full calendar management | `/skills install @openclaw/google-calendar` |
| `obsidian-sync` | Read/write your Obsidian vault | `/skills install @community/obsidian-sync` |
| `github` | Issues, PRs, repos, commits via GitHub API | `/skills install @openclaw/github` |
| `linear` | Issue tracking and project management | `/skills install @openclaw/linear` |
| `notion` | Read and write Notion pages and databases | `/skills install @community/notion` |

### Developer Tools

| Skill | What it does | Install |
|---|---|---|
| `code-reviewer` | Automated PR review with structured feedback | `/skills install @community/code-reviewer` |
| `deploy-check` | Pre-deploy checklist runner | `/skills install @community/deploy-check` |
| `uptime-monitor` | Ping services and alert on downtime | `/skills install @community/uptime-monitor` |
| `docker-manager` | Manage containers via natural language | `/skills install @community/docker-manager` |
| `vercel-deploy` | Trigger Vercel deployments from chat | `/skills install @community/vercel-deploy` |

### Voice & Media

| Skill | What it does | Install |
|---|---|---|
| `elevenlabs-voice` | ElevenLabs TTS — voice replies on any channel | `/skills install @community/elevenlabs-voice` |
| `whisper-stt` | Local speech-to-text via Whisper | `/skills install @community/whisper-stt` |
| `youtube-summarise` | Fetch & summarise YouTube video transcripts | `/skills install @community/youtube-summarise` |

### Automation & Scheduling

| Skill | What it does | Install |
|---|---|---|
| `cron-manager` | Create and manage scheduled tasks in plain language | `/skills install @openclaw/cron-manager` |
| `zapier-trigger` | Fire Zapier zaps from your agent | `/skills install @community/zapier-trigger` |
| `rss-monitor` | Watch RSS feeds, alert on keywords | `/skills install @community/rss-monitor` |
| `auto-skill-hunter` | Proactively discovers & recommends new skills | `/skills install @community/auto-skill-hunter` |

> **Full categorised list** → see [`SKILLS.md`](SKILLS.md) in this repo  
> **Browse everything** → [clawhub.com](https://clawhub.com)

---

## 🏗️ Architecture Reference

Understanding how OpenClaw works makes you dramatically better at configuring it.

```
Your Messaging App (Telegram / WhatsApp / Slack / Signal / iMessage...)
         │
         ▼
┌─────────────────────────────────────────────────────┐
│                    GATEWAY                          │
│         ws://127.0.0.1:18789 (control plane)        │
│  routes channels · manages sessions · handles auth  │
└────────────────────┬────────────────────────────────┘
                     │
         ┌───────────▼───────────┐
         │     AGENT RUNTIME     │
         │   (ReAct loop: think  │
         │    → act → observe    │
         │    → repeat → reply)  │
         └───────────┬───────────┘
                     │
      ┌──────────────┼──────────────┐
      ▼              ▼              ▼
  MEMORY          SKILLS         HEARTBEAT
  ──────          ──────         ─────────
  SOUL.md         ClawHub        Scheduled
  USER.md         installs       proactive
  IDENTITY.md     MCP plugins    tasks
  HEARTBEAT.md    Built-ins
  MEMORY.md
```

**The five components:**

1. **Gateway** — Long-running WebSocket daemon. Single control plane for all channels, sessions, and routing.
2. **Agent Runtime** — The ReAct loop: the LLM reasons, calls a tool, observes the result, repeats until done.
3. **Memory** — Plain Markdown files on your disk. SOUL.md is identity. HEARTBEAT.md is schedule. MEMORY.md is recall.
4. **Skills** — Modular SKILL.md extensions installed from ClawHub or built locally.
5. **Heartbeat** — A scheduler that wakes the agent at a configurable interval to run proactive checks.

**Model recommendations by task:**

| Task | Model |
|---|---|
| Complex reasoning, coding, planning | Claude Opus / GPT-4o |
| Summarisation, drafting, Q&A | Claude Sonnet / Gemini Flash |
| Heartbeat checks (low-cost, high-frequency) | Haiku / Flash / local via Ollama |
| Fully local / private | Llama 3.3 70B via Ollama |

---

## 🔒 Security — Don't Skip This

OpenClaw is powerful because it runs with real access to your machine. That's also what makes it dangerous if misconfigured.

**Non-negotiable baseline:**

```bash
# Check for risky DM policy configurations
openclaw doctor

# Never expose your Gateway to the public internet without auth
# Default bind is localhost only — keep it that way unless you know what you're doing
# If you need remote access, use Tailscale (the community-recommended approach)
```

**Before installing any skill:**

- Read the source on ClawHub before running `/skills install`
- Check the VirusTotal scan on the skill's ClawHub page
- Prefer skills from contributors with existing history and multiple published skills
- Avoid skills that ask for shell access unless you understand exactly why
- Be especially skeptical of skills with suspiciously high install counts but few reviews

**The ClawHub security reality:** In January 2026, 341 malicious skills were discovered on ClawHub across coordinated campaigns. Some reached high install counts before detection. The community has improved moderation significantly since then, but user vigilance is irreplaceable.

**Enable Docker sandbox mode** for any skill you're uncertain about:

```json
// openclaw.json
{
  "skills": {
    "@unknown/some-skill": {
      "enabled": true,
      "sandbox": "docker"
    }
  }
}
```

---

## ⚙️ Configuration Cookbook

Real config snippets for common setups. Copy, adjust, use.

### Multi-model routing (smart cost control)

```json
{
  "models": {
    "primary": {
      "provider": "anthropic",
      "model": "claude-opus-4-5",
      "api_key": "${ANTHROPIC_API_KEY}"
    },
    "heartbeat": {
      "provider": "anthropic",
      "model": "claude-haiku-4-5",
      "api_key": "${ANTHROPIC_API_KEY}"
    },
    "fallback": {
      "provider": "ollama",
      "model": "llama3.3:70b",
      "base_url": "http://localhost:11434"
    }
  }
}
```

### Multi-channel setup (Telegram + Slack + WhatsApp)

```json
{
  "channels": {
    "telegram": {
      "enabled": true,
      "token": "${TELEGRAM_BOT_TOKEN}"
    },
    "slack": {
      "enabled": true,
      "bot_token": "${SLACK_BOT_TOKEN}",
      "app_token": "${SLACK_APP_TOKEN}"
    },
    "whatsapp": {
      "enabled": true,
      "session": "main"
    }
  }
}
```

### Multi-agent routing (isolated workspaces)

```json
{
  "agents": {
    "work": {
      "channels": ["slack"],
      "workspace": "~/openclaw/workspaces/work",
      "model": "primary"
    },
    "personal": {
      "channels": ["telegram", "whatsapp"],
      "workspace": "~/openclaw/workspaces/personal",
      "model": "primary"
    }
  }
}
```

---

## 🌐 Deployment Guides

### Raspberry Pi (Community Favourite)

```bash
# Works on Pi 4 / Pi 5 (4GB+ recommended)
sudo apt update && sudo apt install -y nodejs npm
npm install -g openclaw
openclaw onboard

# Pair with Tailscale for remote access
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up
```

### Hetzner VPS (Best Value Always-On)

```bash
# Hetzner CX22: 2 vCPU / 4GB RAM / 40GB NVMe / €3.79/mo
# Run after SSH into a fresh Ubuntu 22.04 instance

curl -fsSL https://get.openclaw.ai | bash
sudo systemctl enable --now openclaw-gateway
openclaw onboard --headless

# Secure with Tailscale (strongly recommended over opening port 18789)
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up --ssh
```

### Local Ollama (Fully Private, No API Costs)

```bash
# Install Ollama
curl -fsSL https://ollama.ai/install.sh | sh

# Pull a capable local model
ollama pull llama3.3:70b

# Point OpenClaw at it in openclaw.json
# "provider": "ollama", "base_url": "http://localhost:11434", "model": "llama3.3:70b"
```

---

## 🔮 Advanced Patterns

### Pattern 1 — Competitive Intelligence Pipeline

1. Install `firecrawl` + `rss-monitor` + `gmail`
2. In HEARTBEAT.md, add a weekly check: scrape competitors' blogs, pricing pages, changelog feeds
3. Agent summarises deltas using SWOT/PESTEL framework
4. Delivers weekly digest to your inbox automatically

### Pattern 2 — PR Review Automation

1. Install `github` + `code-reviewer` skills
2. Set a HEARTBEAT trigger: check open PRs awaiting review > 24h
3. Agent posts structured review comments: `[BLOCKER]` / `[SUGGESTION]` / `[NITPICK]`
4. Flags security issues and hardcoded credentials automatically

### Pattern 3 — Personal Knowledge Base

1. Install `obsidian-sync` skill
2. Point it at your Obsidian vault
3. Update SOUL.md: "When asked about anything I might have noted, check Obsidian first"
4. Agent becomes a searchable second brain accessible from any of your channels

### Pattern 4 — Agent Team (Orchestration)

```json
// Route different channels to specialised agents
{
  "agents": {
    "researcher":  { "channels": ["telegram"],  "workspace": "workspaces/researcher" },
    "coder":       { "channels": ["slack"],      "workspace": "workspaces/coder" },
    "scheduler":   { "channels": ["whatsapp"],   "workspace": "workspaces/scheduler" }
  }
}
```

Each agent has its own SOUL.md, HEARTBEAT.md, and memory — isolated but coordinated.

---

## 🤝 Contribute — Become Legend

This repo lives and dies by the community. The fastest way to grow it — and your own following — is to contribute.

**Your name in front of thousands of devs. Three ways in:**

**1. Drop an extermination** *(fastest — merged same day)*
```
PR title: [EXTERMINATION] What your agent destroyed
Include: time, model, screenshot or GIF, one-line description
```

**2. Add a SOUL.md template**
```
PR title: [SOUL] Template name — use case in 5 words
```

**3. Fix or improve anything**
```
PR title: [DOCS] What you changed and why
```

Every contributor lands permanently in [`CONTRIBUTORS.md`](CONTRIBUTORS.md).  
Every extermination gets a shoutout on X with `#ClawExterminator`.

---

## 📡 Community

| Platform | Link | What's there |
|---|---|---|
| Discord | [discord.gg/openclaw](https://discord.gg/openclaw) | Main community hub — skill help, showcases, announcements |
| Reddit | [r/clawdbot](https://reddit.com/r/clawdbot) | Show & tell, discussion, news |
| Twitter/X | [#OpenClaw](https://twitter.com/hashtag/OpenClaw) | Kills, updates, community highlights |
| ClawHub | [clawhub.com](https://clawhub.com) | Official skill registry |
| SOUL registry | [onlycrabs.ai](https://onlycrabs.ai) | Community SOUL.md sharing |
| Official docs | [docs.openclaw.ai](https://docs.openclaw.ai) | Reference documentation |

---

## 📋 Quick Reference

```bash
openclaw onboard          # First-time setup wizard
openclaw doctor           # Check for misconfigurations and security issues
openclaw status           # Gateway status, active channels, model, token usage
openclaw restart          # Restart the Gateway

/skills browse <category> # Browse ClawHub skills by category
/skills install <slug>    # Install a skill from ClawHub
/skills list              # List installed skills
/skills update --all      # Update all installed skills

/status                   # Compact session status
/reset                    # Reset current conversation context
/model <name>             # Switch model mid-session
```

---

<div align="center">

**Built by the community. For the community. 🦞**

*Star if it saved you time. Fork if you want to shape it.*  
*Submit a PR if your agent exterminated something worth documenting.*

[![Star this repo](https://img.shields.io/github/stars/Devanik21/claw-exterminator?style=social)](https://github.com/Devanik21/claw-exterminator)

---

*Not affiliated with Peter Steinberger or the official OpenClaw team.*  
*Official repo: [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw)*

</div>
