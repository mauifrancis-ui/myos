# myOS — Build phases

---

## Phase 1 — Foundation (Week 1)
**Status: In progress**

Goal: Working external memory layer and structured database.

- [ ] Claude Project created at claude.ai
- [ ] System instruction + memory profile pasted into Project Instructions
- [ ] Test: "Good morning myOS. Who am I and what do I need to know today?"
- [ ] Airtable base created with all 7 tables
- [ ] All tables seeded with real data
- [ ] Daily habit established: open myOS Project every morning

**Stack:** Claude Projects + Airtable  
**Outcome:** Brain backup working tonight. Database seeded.

---

## Phase 2 — Passive intelligence (Week 2)
**Status: Upcoming**

Goal: Gmail scanned automatically. Data files without you touching it.

- [ ] Make account created at make.com
- [ ] Gmail connected to Make via OAuth
- [ ] Email extraction scenario built (nightly at 2am)
- [ ] Claude API key created at console.anthropic.com
- [ ] Email extraction prompt connected (see prompts/brief-agent.md)
- [ ] Airtable connection from Make confirmed
- [ ] Test run with 1 week of emails
- [ ] Go live

**Stack:** Make + Gmail API + Claude API + Airtable  
**Outcome:** Inbox scanning automatically. Nothing in email slips.

---

## Phase 3 — Morning briefing (Week 3)
**Status: Upcoming**

Goal: Real HTML email arrives at 7am. Approve directly from email.

- [ ] Orchestrator scenario built in Make
- [ ] All agent outputs connected to orchestrator
- [ ] Orchestrator prompt connected (see prompts/orchestrator.md)
- [ ] Email template built (HTML)
- [ ] Briefing send scheduled for 7am daily
- [ ] Approve-by-email webhooks connected
- [ ] Test run for 3 days before going live

**Stack:** Make + Claude API + Gmail (send) + Airtable  
**Outcome:** The daily ritual. Feels like a product for the first time.

---

## Phase 4 — Live dashboard (Week 4)
**Status: Upcoming**

Goal: The freestanding tool. Full UI with live data.

- [ ] Framer account set up
- [ ] Airtable API connected to Framer
- [ ] Dashboard sections wired to live tables
- [ ] Approval queue connected to Make webhooks
- [ ] Quick capture input connected
- [ ] Custom domain set up (myos.app or similar)
- [ ] Mobile-responsive confirmed

**Stack:** Framer + Airtable API + Make webhooks  
**Outcome:** The full product. Open it in any browser. No Claude required.

---

## Phase 5 — Memory intelligence (Month 2)
**Status: Future**

Goal: Memory Agent running. Preferences learned automatically.

- [ ] Memory Agent scenario built in Make
- [ ] Nightly preference update running
- [ ] Monthly pattern analysis running
- [ ] Artist score updates automated
- [ ] Preference profile updating silently
- [ ] Culture Agent festival discovery pipeline active

**Stack:** Make + Claude API + Spotify API + Songkick API + Airtable  
**Outcome:** myOS stops reacting and starts anticipating.

---

## Non-negotiable rules (never break these)

1. **5-item hard cap on today's read.** Orchestrator must cut if more than 5 candidates. No exceptions.
2. **Health items always surface within lead time.** Never deprioritised. Never skipped.
3. **Forward-facing language only.** Never "you forgot." Always "renews in X days."
4. **Undo for every approval.** Minimum 30 seconds. Always in the same spot as the confirmation.
5. **Silence when healthy.** Green dot and a timestamp. No fanfare.
6. **Trust through attribution.** Every approval card shows which agent prepared it and why.
