# Airtable Schema — myOS

Complete field definitions for all 7 tables.
Base name: myOS
Created: April 2026

---

## Memory table

The most important table. Your external autobiographical memory.

| Field | Type | Options / Notes |
|---|---|---|
| date | Date | ISO format |
| content | Long text | User's exact words wherever possible |
| source | Single select | You / Gmail / Agent / Calendar |
| type | Single select | Event / Commitment / Feeling / Admin / Health / Culture |
| person | Text | Name if this involves someone |
| keep_forever | Checkbox | Never auto-archive if checked |
| tags | Multiple select | Artist / Festival / Concert / Work / Personal / Medical / Joy |
| linked_event | Link to Shows | Connect to a specific show |

---

## Health table

| Field | Type | Options / Notes |
|---|---|---|
| medication | Text | Full medication name |
| dose | Text | e.g. 500mg twice daily |
| next_renewal | Date | When prescription needs refilling |
| refill_lead_days | Number | Default: 14 |
| pharmacy | Text | Name and location |
| doctor | Text | Prescribing doctor |
| notes | Long text | Any additional context |

---

## People table

| Field | Type | Options / Notes |
|---|---|---|
| name | Text | Full name |
| relationship | Single select | Family / Friend / Colleague / Other |
| birthday | Date | Year optional |
| anniversary | Date | Any other important date |
| what_to_remember | Long text | Everything about them and your relationship |
| gift_style | Text | What they love |
| last_contact | Date | Updated by Gmail agent |
| reminder_lead_days | Number | Default: 14 |

---

## Shows & Concerts table

| Field | Type | Options / Notes |
|---|---|---|
| artist | Text | Artist or festival name |
| venue | Text | Name and city |
| date | Date | Date of show |
| type | Single select | Concert / Festival / DJ Set / Other |
| discovery | Checkbox | First time hearing this artist? |
| went_alone | Checkbox | Solo show? |
| my_words | Long text | What you said afterward — exact words |
| engagement_score | Number | 1–10 |
| status | Single select | Core Artist / Deep Listener / Casual Follow / Faded |
| discovered_artists | Text | New artists found at this show |

---

## Artists table

| Field | Type | Options / Notes |
|---|---|---|
| name | Text | Artist name |
| spotify_id | Text | From Spotify artist URL |
| songkick_id | Text | For tour tracking |
| discovered_at | Link to Shows | Where you first heard them |
| engagement_score | Number | 1–10, updated monthly |
| times_seen_live | Number | Total live shows |
| genre_tags | Multiple select | Psychedelic / Electronic / World / Ambient / Other |
| active_tracking | Checkbox | Watch for releases and tour dates? |
| next_tour_date | Date | Populated by Culture Agent |
| notes | Long text | Favourites, discoveries, notes |

---

## Admin & Life table

| Field | Type | Options / Notes |
|---|---|---|
| item | Text | What it is |
| due_date | Date | When action needed |
| reminder_lead_days | Number | Days ahead to surface |
| urgency | Single select | Critical / High / Medium / Low |
| status | Single select | Upcoming / Action needed / Done / Recurring |
| recurring | Checkbox | On a schedule? |
| frequency | Single select | Monthly / Quarterly / Annual / Other |
| provider | Text | Who handles this |
| notes | Long text | Extra context |
| amount | Currency | If relevant |

---

## Financial & Bills table

| Field | Type | Options / Notes |
|---|---|---|
| description | Text | What it is |
| amount | Currency | Amount |
| due_date | Date | Payment due |
| status | Single select | Upcoming / Paid / Overdue / Recurring |
| source | Single select | Gmail extract / Manual / Agent |
| recurring | Checkbox | Regular charge? |
| frequency | Single select | Monthly / Quarterly / Annual |
| payment_method | Text | How paid |
| category | Single select | Tax / Subscription / Utility / Insurance / Invoice / Other |
| notes | Long text | Reference numbers, account info |

---

## Setup checklist

- [ ] Create base named "myOS" at airtable.com
- [ ] Create all 7 tables with fields above
- [ ] Set refill_lead_days to 14 for all medications
- [ ] Set reminder_lead_days to 14 for all people
- [ ] Seed Memory table with concerts, commitments, significant moments
- [ ] Seed Health table with all current medications and doctors
- [ ] Seed People table with family and close friends
- [ ] Seed Shows table with last 12 months of concerts
- [ ] Seed Artists table with active tracking artists
- [ ] Seed Admin table with car, passport, and upcoming renewals
- [ ] Seed Financial table with known upcoming bills and taxes
