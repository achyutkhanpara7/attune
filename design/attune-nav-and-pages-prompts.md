# Attune — Mega-Menu Nav + New Pages
### Claude Design paste-prompts, modeled on BetterUp's real nav and page anatomy

---

## What BetterUp actually does (so you're matching the real thing)

**Nav** is a mega-menu. Top items — Platform, Solutions, Use Cases, Insights, Customers, Company — each open a wide dropdown panel containing a grid of items (icon + title + one-line description), plus a "featured" promo tile on the right. Login + Request a demo sit far right.

**Platform page anatomy:** hero (proof-driven headline "Transformation that scales. Data that proves it." + floating product-UI cards over a soft gradient) → logo bar → positioning line → "the platform in a nutshell" value props (Human+AI, personalized development, measurable impact, enterprise security, strategic partners) → product cards → 4 benefit icons ("Change that sticks") → case-study proof with metrics + video → integrations ("works where you do" — Slack/Teams/Workday + stats) → FAQ accordion → CTA band → footer.

**Product page anatomy (BetterUp Lead):** eyebrow "BetterUp Lead™" + hero headline + subhead + demo CTA + device/product image → logo bar → stats band (1.5x promotion, 20% productivity, 29% capability) → "the engine behind the results" — 3–4 feature blocks each with a product-UI overlay image → 4 icon features → outcomes grid ("How inspired leadership pays off" — Retain / Accelerate / Culture / ROI) → featured case study with video → FAQ → CTA → footer.

---

## Attune nav map (adapted to your pages)

| Top item | Dropdown items (icon + title + one-liner) | Featured tile |
|---|---|---|
| **Platform** | Overview · Integrations · Powered by AI · Trust & Security | "How Attune works" → Platform page |
| **Products** | Attune Guide (1:1 human coaching) · Attune Flow (AI coaching in the flow of work) · Attune Signal (performance intelligence) | "See all three in action" → demo |
| **Solutions** | Leadership development · Manager effectiveness · Whole-workforce coaching · Change & resilience · For government | "Proof by industry" → Customers |
| **Customers** | Case studies · Results & ROI | Featured story: "Orbital +15%" |
| **Company** | About · Coaches · Careers · Newsroom | — |

---

## 1) MEGA-MENU NAV — paste prompt

> Upgrade the Attune top nav into a mega-menu, keeping the existing glass pill styling and scroll-shrink behavior. Top items: Platform, Products, Solutions, Customers, Company — with Login and an ember "Request a demo" button on the far right.
>
> Each of Platform, Products, and Solutions opens a dropdown **panel** on hover (desktop) or tap (mobile):
> - The panel is a rounded glass card (pine #14312A at ~94% + backdrop-blur, thin light border, soft shadow) that drops just below the nav and fades-and-rises in (150ms).
> - Inside: a grid of menu items, each = a small rounded sand-tile icon + a Fraunces title + a one-line Inter description in muted ivory. Item hover = subtle background tint + ember title.
> - On the right of each panel, a "featured" promo tile with a small gradient thumbnail, a label, and a link.
> - Populate with the Attune nav map: Platform → Overview / Integrations / Powered by AI / Trust & Security; Products → Attune Guide / Attune Flow / Attune Signal; Solutions → Leadership development / Manager effectiveness / Whole-workforce coaching / Change & resilience / For government.
> - Customers and Company are simple links (or small dropdowns: Customers → Case studies, Results & ROI; Company → About, Coaches, Careers, Newsroom).
>
> Interaction + accessibility: open on hover with a ~120ms close delay so the cursor can travel into the panel; also open on click/focus for keyboard users; close on mouse-leave, Esc, or outside-click; use aria-haspopup and aria-expanded. On mobile (<900px) the nav collapses to a hamburger, and the dropdowns become expandable accordions. Respect prefers-reduced-motion.
>
> Wire each item to its page (Platform, the three Product pages, the Solutions page, Customers) so navigation works.

---

## 2) PLATFORM PAGE — paste prompt

> Using the Attune design system (ivory #F7F3EC, pine #14312A, ember #E8674C, jade #3E7C6A, sand #EDE4D6; Fraunces display + Inter body; scroll-reveal + count-up motion; glass cards; mega-menu nav + 5-column footer on every page), create the **Platform** page in this order:
> 1. Hero on a soft pine gradient: headline "Transformation that scales. Proof that follows." + subhead + "Request a demo" (ember) and "Watch it in action" (ghost). Float 3–4 real product-UI cards (a coaching-topic card, a chat-based session, a strategic-thinking chart, an energy-rating screen).
> 2. Logo bar (Northwind, Vela Health, Orbital, Kestrel Bank, Lumina, Foundry).
> 3. Positioning line: "Some tools scale but don't work. Others work but don't scale. Attune does both."
> 4. "The platform in a nutshell" — five value props with small UI/图 visuals: Human + AI combined · Personalized development at scale · Measurable impact & ROI · Enterprise-grade security (SOC 2, ISO 27001, GDPR) · Strategic partnership from day one.
> 5. Product row: Attune Guide / Flow / Signal cards, each with a mini interface preview, linking to their pages.
> 6. "Change that sticks" — four benefit tiles with icons (faster transformations, consistent performance, clearer signals, earlier risk detection).
> 7. "The proof is in the platform" — a case-study strip with switchable logos and a headline metric each (e.g., Orbital +15% performance, Vela Health 21% productivity), with a muted background video.
> 8. Integrations: "Attune works where you do." Slack, Teams, Zoom, Workday, Salesforce, Outlook logos + a stat line (e.g., "Teams that integrate Attune see 47% higher performance").
> 9. FAQ accordion (5 questions on frameworks, integrations, measurement, security).
> 10. CTA band on a textured pine background: "Explore a plan for your workforce." + demo button.
> Alternate ivory/pine section backgrounds for rhythm.

---

## 3) PRODUCT PAGE TEMPLATE — paste prompt (reuse for Guide, Flow, Signal)

> Using the Attune design system and shared nav/footer, create the **Attune Guide** product page in this order (this becomes the template — I'll swap content for Flow and Signal after):
> 1. Eyebrow "Attune Guide" + hero headline "The leadership system your strategy runs on." + subhead + "Request a demo". Large product/device image of the coaching interface on the right.
> 2. Logo bar "Trusted by leading teams."
> 3. Stats band: three proof stats with customer logos (e.g., 1.5x higher promotion rate, 20% productivity boost, 29% lift in coaching capability). *(illustrative)*
> 4. "The engine behind the results" — four feature blocks, each a large background image with a floating product-UI overlay card: 1:1 dedicated coaching · Whole-person assessments · Specialized support · Always-on AI learning.
> 5. "Features" — four icon features (Human + AI in sync, better prepared for breakthroughs, fewer notes/more alignment, instantly trustworthy).
> 6. "How it pays off" — four outcome tiles: Retain your best · Accelerate business gains · Craft a winning culture · Prove your ROI.
> 7. Featured case study with a muted video and a headline ("Greater innovation for Orbital's product leaders") + "See the story."
> 8. FAQ accordion (difference between Guide/Flow/Signal, coach matching, data security, ROI measurement).
> 9. CTA band: "Lead your business into the next era." + demo button.
>
> **For Attune Flow:** same layout, content about always-on AI coaching in the flow of work — chat interface, daily nudges, mobile UI; stats about adoption and habit-building.
> **For Attune Signal:** same layout, content about performance intelligence — dashboards, manager effectiveness, attrition-risk, ROI; product UI shows jade analytics charts.

---

## 4) SOLUTIONS PAGE — paste prompt

> Using the Attune design system and shared nav/footer, create the **Solutions** page: hero "Coaching for every layer of your business." → five alternating solution blocks (Leadership development, Manager effectiveness, Whole-workforce coaching, Change & resilience, For government), each with a one-line outcome, a headline stat, a supporting image/UI, and a "Read the story" link → a 4-tile "by industry" grid (Financial services, Healthcare, Technology, Public sector) → CTA band + footer.

---

## 5) CUSTOMERS PAGE — paste prompt

> Using the Attune design system and shared nav/footer, create the **Customers** page: hero "Proof, not promises." → a large featured case study with a headline metric ("Orbital shifted the performance curve +15%") and a muted background video → a metric-highlights row → a logo wall → one strong testimonial quote → a 6-card case-study grid (each: logo, metric, one-line result, "Read story") → CTA band + footer.

---

## Wiring checklist
- [ ] Mega-menu items, footer links, and every "Learn more" on the home pillars point to the real pages
- [ ] Nav + footer identical across all pages
- [ ] Each new page opens with the shared design-system tokens (paste the system-lock line at the top if Claude Design drifts)
- [ ] All invented stats keep the "illustrative" footnote
- [ ] Mobile: mega-menu → hamburger + accordions; product device images stack
