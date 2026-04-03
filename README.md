# myOS

> A personal AI operating system that holds what I can no longer reliably hold myself.

myOS is a personal agent OS built for someone with epilepsy whose medication causes progressive memory loss. It tracks your cultural life, health, finances, relationships, and life admin — pulling from Gmail automatically overnight and surfacing everything that needs attention each morning. You approve. It acts.

---

## What this is

- **Not a productivity app.** An external cognitive support system and identity archive.
- **Built for progressive memory loss.** The system grows into the role as you need it to.
- **Design-first.** Built by a Sr. UX Designer with 20+ years experience at Google.
- **Agent-powered.** Five specialized agents run overnight so you wake up to a prepared morning.

---

## Project structure

```
myos-project/
├── dashboard/          # The standalone UI (HTML/CSS/JS)
│   └── index.html      # Full interactive dashboard — open in any browser
├── onboarding/         # User onboarding flow
│   └── index.html      # Memory profile capture — fill this in first
├── prompts/            # Claude API system prompts for each agent
│   ├── orchestrator.md
│   ├── brief-agent.md
│   ├── culture-agent.md
│   ├── admin-agent.md
│   └── memory-agent.md
├── airtable-schema/    # Database field definitions
│   ├── memory.md
│   ├── health.md
│   ├── people.md
│   ├── shows.md
│   ├── artists.md
│   ├── admin.md
│   └── financial.md
├── docs/               # Build guides and project documentation
│   └── build-phases.md
└── README.md
```

---

## The five agents

| Agent | Job | Runs |
|---|---|---|
| **Orchestrator** | Assembles morning briefing from all agent outputs | 6am daily |
| **Brief Agent** | Reads Gmail, drafts email replies | 2–5am |
| **Culture Agent** | Tracks artists, tour dates, new releases | 2–5am |
| **Admin Agent** | Manages health, life admin, important dates | 2–5am |
| **Memory Agent** | Learns preferences, updates profile silently | 11pm daily |

---

## Build phases

| Phase | What | Stack | Status |
|---|---|---|---|
| Phase 1 | Claude Project + Airtable base | Claude + Airtable | 🔨 In progress |
| Phase 2 | Gmail scanning | Make + Gmail API | ⏳ Next |
| Phase 3 | Morning briefing email | Make + Claude API | ⏳ Upcoming |
| Phase 4 | Live dashboard | Framer + Airtable API | ⏳ Upcoming |

---

## Core design principles

- **Silence is the success state** — when everything works, myOS is quiet
- **You approve, never micromanage** — myOS acts, you confirm
- **Memory makes it yours** — learns preferences and applies them silently
- **Trust through transparency** — every agent shows its work
- **Voice has personality** — warm, dry, never robotic
- **Never make you feel like you forgot** — always forward-facing language
- **Joy is tracked too** — cultural life is as important as admin life
- **5-item hard cap** on today's read — never more, ever

---

## Tech stack

| Layer | Tool |
|---|---|
| AI intelligence | Claude API (claude-sonnet-4-5) |
| Automation | Make (Integromat) |
| Database | Airtable |
| Email source | Gmail API via Make |
| Music tracking | Spotify API + Songkick API |
| Dashboard UI | Framer (Phase 4) |
| Payments | Lemon Squeezy (if productised) |

---

## The voice

myOS speaks like a brilliant, trusted friend who already read your emails before you woke up. Calm. Intelligent. Occasionally dry. Never robotic. Never corporate. Never makes you feel bad about forgetting something.

> *"Your car's been waiting 3 weeks. It's not going to book itself."*

---

## License

Private project. Not open source.
