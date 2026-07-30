# Attune — Coaching Platform Case Study
### Brand system + page content + Claude Design build prompts

*A fictional enterprise coaching platform created for a UX case study. All content, naming, and metrics below are original and illustrative — nothing is copied from BetterUp.*

---

## 1. The brand

**Name:** Attune
*(alt names if you want a different flavor: **Cairn** or **Meridian**)*

**One-liner:** The coaching platform that develops every person — and proves every gain.

**Positioning:** Attune pairs world-class human coaches with always-on AI coaching, then ties every session to the performance metrics leadership actually cares about. One platform, from the C-suite to the frontline.

**Voice:** Warm, confident, precise. Human first, data-backed second. Short declarative sentences. No hype words, no exclamation marks.

**Three product pillars (original — don't reuse BetterUp's Lead/Manage/Grow/Ready):**
- **Attune Guide** — 1:1 human coaching for leaders and managers
- **Attune Flow** — AI coaching in the flow of work, for everyone
- **Attune Signal** — performance intelligence that connects growth to outcomes

---

## 2. Theme (visual system)

**Palette**

| Role | Name | Hex |
|---|---|---|
| Canvas / background | Ivory | `#F7F3EC` |
| Deep base / dark sections / headings | Pine | `#14312A` |
| Primary accent (CTAs, kinetic word) | Ember | `#E8674C` |
| Secondary accent / data viz / links | Jade | `#3E7C6A` |
| Card tint / section bands | Sand | `#EDE4D6` |
| Body text | Charcoal | `#33322E` |
| Muted text / borders | Mist | `#9A9488` |

Single-accent discipline: Ember does the pointing (CTAs + the one kinetic word), Jade supports (data, secondary buttons). That restraint is what reads as "expensive."

**Type**
- **Display / headlines:** Fraunces (warm humanist serif — free on Google Fonts). This is your differentiator from BetterUp's sans.
- **Body / UI:** Inter.
- **Scale:** Hero display 64–80px · H2 40–48 · H3 24–28 · body 17–18 · caption 14. Tight line-height on headers, generous whitespace everywhere.

**Motion:** Scroll-triggered fade-and-rise on section entrance; one kinetic hero word that cycles; gentle parallax on imagery. Entrances only — over-animating reads as junior.

**Imagery:** Warm, real-people lifestyle photography. Not illustration.

---

## 3. The pages (all copy original)

### Page 1 — Landing / overview
- **Hero H1 (kinetic):** Develop every ⟨person⟩, and prove it. — bracketed word cycles: person → leader → manager → team → maker (in Ember)
- **Subhead:** Attune pairs world-class human coaches with always-on AI, then ties every session to the metrics your CEO cares about.
- **CTAs:** See Attune in action (Ember) · Watch the 2-min tour (ghost)
- **Trust bar:** "The best teams grow with Attune" + wordmarks: Northwind · Vela Health · Orbital · Kestrel Bank · Lumina · Foundry
- **Problem section H2:** Development that stops at the top never reaches the work.
- **Pillars section H2:** One platform. Three ways to grow. (Guide / Flow / Signal cards)
- **Metrics band (Pine bg) H2:** What changes when growth is measured. → 12x average ROI · 43% more top performers · 2.4x faster manager ramp · 38% less regretted attrition *(illustrative)*
- **How it fits (3 steps):** Coaches build the mindset → AI reinforces it daily → Signal proves the impact.
- **Closing CTA:** See what your workforce could become. → Request a demo

### Page 2 — Coach matching (Attune Guide)
- **Hero:** The right coach, matched in minutes.
- **Flow:** Goals intake → matched on domain, style, and timezone → meet 2–3 coaches → pick your fit. Book, meet, and get an AI-written recap with action items after every session.
- **UI to design:** coach-match cards (photo, specialty tags, style, availability), a "why this match" panel, and a session-booking moment.
- **Quote (illustrative):** "My coach felt hand-picked. Because she was." — VP Engineering, Orbital

### Page 3 — Member dashboard (the product UI — your strongest UX page)
The logged-in home. Design: a warm greeting + next session card, 2–3 active goals with circular progress, this-week focus, habit streaks pulled from Flow, and a "recent insight" surfaced by Signal. This page shows you can design data-dense product UI, not just a homepage.

### Page 4 — Attune Signal (analytics / exec view)
The admin view: manager effectiveness, engagement, attrition-risk cohorts, and ROI — Jade data viz on ivory. *(Alternative if you'd rather close on marketing: a "See Attune in action" demo-request page.)*

---

## 4. Paste this into Claude Design first (Page 1)

> Design a premium marketing landing page for a fictional enterprise coaching platform called **Attune**.
>
> Brand feel: warm, human, and precise — editorial magazine meets enterprise SaaS. Confident but calm, never hypey.
>
> **Palette:** canvas ivory #F7F3EC · deep pine #14312A for dark sections and headings · ember coral #E8674C as the single accent (CTAs + one kinetic word) · jade #3E7C6A for secondary accents and data · sand #EDE4D6 for card tints · charcoal #33322E body text.
> **Type:** Fraunces (serif) for all display/headlines, Inter for body and UI. Big editorial scale, generous whitespace, tight header line-height.
> **Motion:** subtle scroll-triggered fade-and-rise reveals; a kinetic hero word that cycles; gentle parallax on imagery. Entrances only.
> **Imagery:** warm real-people lifestyle photography, not illustration.
>
> Build these sections:
> 1. Sticky slim top nav — logo "Attune", links Platform / Solutions / Customers / Company, and an ember "Request a demo" button.
> 2. Hero — oversized Fraunces headline "Develop every ⟨person⟩, and prove it." where the bracketed word cycles person → leader → manager → team → maker in ember. Subhead: "Attune pairs world-class human coaches with always-on AI, then ties every session to the metrics your CEO cares about." CTAs: "See Attune in action" (ember), "Watch the 2-min tour" (ghost).
> 3. Trust logo bar — "The best teams grow with Attune" + six muted wordmarks: Northwind, Vela Health, Orbital, Kestrel Bank, Lumina, Foundry.
> 4. Problem section on ivory — H2 "Development that stops at the top never reaches the work." + one short paragraph.
> 5. Three-pillar cards — Attune Guide (1:1 human coaching), Attune Flow (AI coaching in the flow of work), Attune Signal (performance intelligence). Each: icon, name, one line, "Learn more."
> 6. Dark pine metrics band — H2 "What changes when growth is measured." + four big animated stats: 12x average ROI, 43% more top performers, 2.4x faster manager ramp, 38% less regretted attrition. Small footnote: illustrative.
> 7. "How it fits together" 3-step row — Coaches build the mindset → AI reinforces it daily → Signal proves the impact.
> 8. Closing CTA band — "See what your workforce could become." + demo button.
> 9. Footer with columns.
>
> Make it feel like a $200M-funded brand's site. Responsive.

Then for each next page, start a new message in the same Claude Design project: *"Same Attune brand system and palette. Now design Page 2: the coach-matching experience…"* and paste the Page 2/3/4 notes above. Iterating page-by-page keeps each one sharp.

---

## 5. One integrity note
The stats (12x ROI, 43%, etc.) are **invented placeholders** so the page feels enterprise-real. Keep the "illustrative" footnote on them, or swap in real published coaching-industry benchmarks if you want to cite something defensible in the interview. Don't present invented numbers as real research — that's the one thing that can sink an otherwise great case study.
