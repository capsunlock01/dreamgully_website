# Case Study Page Template

**Version:** 1.0
**Applies to:** All 11 case study pages (4 real/in-progress + 7 fictional)
**Owner:** DreamGully
**Last updated:** 2026-06-03

---

## What this template is

Every case study page on `dreamgully.com` is built from this structure. Some sections are required for all, some are conditional based on case study depth (light / medium / heavy) and source (real client / in-progress / fictional concept).

The template defines:
- Page structure (sections, in order)
- Visual treatment per section
- Required vs. optional content
- Per-tier content rules (light / medium / heavy)
- Per-source content rules (real / in-progress / fictional)
- Reusable CSS class names and HTML patterns
- Image specs per section
- Tone of voice

This is the contract. New case study pages ship when they conform to this template. Variations are exceptions, not the rule.

---

## URL structure

`/case-studies/{slug}.html`

Examples:
- `/case-studies/dreamgully.html`
- `/case-studies/beyond-basics.html`
- `/case-studies/vogue-atelier.html`
- `/case-studies/dubai-realestate.html` (in-progress placeholder page)
- `/case-studies/{fictional-brand-slug}.html` (7 pages)

All case study pages link to each other via "Next case study" footer (rotates, not random).

---

## Page sections (in order)

### 1. HERO

**Required for all.** Sets the brand, the work, the visual.

**Content:**
- **Eyebrow tag:** `{Vertical} · {Geography}` (e.g., "Streetwear · India", "Cafe · Melbourne", "Real Estate · Dubai")
- **Brand name:** H1. The actual brand name, large, gradient text (matches site style)
- **Tagline / one-liner:** the brand's positioning statement, italic or muted
- **Hero image:** full-width, 16:9 or 4:3, the strongest single visual from the case study
- **Badge (top-right or top-left of hero):** "Client Work" or "Concept" or "In Progress" — see Badge rules below
- **CTA (top-right or inline):** "View live" (real only) or "View case study" (fictional)

**Visual treatment:** full-bleed dark hero with blue gradient text (matches site design), image below or beside text per case study layout.

**For fictional case studies ONLY — Concept Study Callout (required):**

A small text block in the hero, between the brand name and the tagline. This is the per-page reinforcement of the "Concept" badge and the section header disclaimer. It's the third layer of protection, placed where the most-engaged reader will see it (right after the brand name, before the brand story begins).

**Content (default copy, adjustable):**

> **Concept study** — This brand is a designed concept created to showcase DreamGully's process. No real client exists. The work shown is conceptual, not a shipped client engagement.

**Visual treatment:**
- Smaller font than the tagline (~14-16px)
- Muted text color (NOT the gradient blue) — uses `--text-muted` token
- Italic or normal weight (your call, both work)
- 1-2 lines on desktop, 2-3 on mobile
- Sits between the brand name (H1) and the tagline (italic brand description)
- Top margin matches the brand description's top margin (visual rhythm)

**Why three layers (badge + section header + per-page callout):**
- **Section header disclaimer** catches visitors browsing the case studies section
- **Per-card "Concept" badge** catches visitors who click a card
- **Per-page callout** catches visitors who are now reading the brand story — this is the most engaged reader, the one most likely to think the brand is real
- Three layers = much harder for a trademark holder to argue "likely confusion"

**Optional removal:** Taimoor can drop one of the three layers later if it feels redundant. Recommended order to drop if needed: section header disclaimer first (least visible), then per-card badge, last is per-page callout (most important to keep).

### 2. OVERVIEW

**Required for all.** Three short data points + a 1-paragraph summary.

**Content:**
- **Three data tiles** (varies by case study, choose from this list as applicable):
  - Client / Brand
  - Industry / Vertical
  - Geography
  - Year / Duration
  - Services delivered
  - Notable result / outcome
- **Summary paragraph:** 2-3 sentences. What the brand was, what we did, what changed. (Fictional: "Concept study demonstrating how a brand identity could be built for..." with the result being a designed system, not a business outcome.)

### 3. THE BRIEF

**Required for all.** What the client (or fictional client) needed from us.

**Content:**
- 1-2 paragraphs. Plain language. What was the problem, what was the constraint, what did success look like.
- Optional pull-quote from the client (real only, with permission) or a "hypothetical brief" framing (fictional).

**Fictional framing:** "If a modern Melbourne fitness studio approached us to launch their brand from scratch, here's how we'd approach the brief." Then the brief section reads as if it were real.

### 4. THE WORK

**Required for all.** What we actually did. This is the longest section and varies most by tier.

**Light tier (2 case studies):**
- 1 section per deliverable. Maximum 3 deliverable sections.
- Each deliverable: 1 image + 1 paragraph of description.
- Deliverables for light tier: Brand identity only (logo + color + typography).

**Medium tier (3 case studies):**
- 1 section per deliverable. 3-5 deliverable sections.
- Each deliverable: 1-2 images + 1-2 paragraphs.
- Deliverables for medium tier: Brand identity + supporting collateral (e.g., business cards, social templates, mood board).

**Heavy tier (2 case studies):**
- 1 section per deliverable. 5-8 deliverable sections.
- Each deliverable: 2-3 images + 1-2 paragraphs.
- Deliverables for heavy tier: Brand identity + website screens + social content samples + marketing collateral + signage/packaging (as applicable).

### 5. RESULTS / OUTCOME

**Required for real case studies, optional for in-progress, replaced for fictional.**

- **Real:** metrics, client quote, before/after. Lead with the strongest number.
- **In-progress:** "Engagement in progress — case study updates as deliverables ship." No fake metrics.
- **Fictional:** "Concept study — no real outcomes to report. The deliverables shown are designed to demonstrate our process and craft, not business results." Replaced with a process note.

### 6. CREDITS

**Required for all.** Who did what. Honest, specific.

- **Creative direction:** Taimoor / DreamGully
- **Brand strategy:** Taimoor / DreamGully
- **Design:** Taimoor / DreamGully (or with named collaborator if any)
- **Copy:** Taimoor / DreamGully
- **Web development:** (if applicable) Taimoor / DreamGully
- **Photography:** credited source or "Generated with AI tools" (transparent)

For fictional case studies: "All work shown is a concept study designed to demonstrate DreamGully's process. No real client, no shipped deliverables."

### 7. NEXT CASE STUDY

**Required for all.** Link to the next case study in rotation. Footer of page, with the next case study's hero image + brand name + vertical tag.

---

## Badge rules

Top-right or top-left of the hero, on every case study:

| Source | Badge text | Color treatment |
|---|---|---|
| Real client work, shipped | "Client Work" | Blue gradient pill, white text |
| Real client work, in progress | "In Progress · Coming Q3 2026" | Muted grey pill, italic |
| Fictional concept study | "Concept" | Outline-only pill, muted text |

Badges are visible but not loud. They read at hover and at glance.

---

## Section label / framing rules

The "Selected Work" section header on the main case studies landing page says:

> **"Selected Work"**
> A mix of client engagements and concept studies designed to demonstrate our process across verticals.

Bottom of section (small, single line):

> "Concept studies are fictional brands designed to showcase our process. Real client work is shipped and on the record."

This is the only place the "concept" framing appears at the section level. Per-card "Concept" badges are the per-card reinforcement.

---

## Image specs

| Image location | Aspect ratio | Notes |
|---|---|---|
| Hero | 16:9 or 4:3 | Single strongest image. High quality, ~2400px wide native. |
| Overview tiles | N/A | Text only, no images |
| Brief section | Optional 1 image | 16:9, contextual to the brief |
| Work section — per deliverable | 4:3 or 1:1 | 1 image for light, 1-2 for medium, 2-3 for heavy |
| Work section — website screenshots | 16:9 or 16:10 | Browser-frame mockup, show desktop + mobile if possible |
| Work section — social posts | 1:1 or 4:5 | Grid display, 3-9 posts per row |
| Results | Optional 1 image | Hero-style, 16:9 |
| Credits | N/A | Text only |
| Next case study card | 4:3 | Same image as the next case study's hero (smaller crop) |

**Image source policy:**
- **Real case studies:** Use real shipped assets. If assets are missing, the case study is incomplete and doesn't ship.
- **Fictional case studies:** Use AI-generated imagery (Freepik / Seedream / Flux) following the same `image-prompt-engineer` methodology already in `dreamgully/assets/prompts/`. No readable text, no legible logos, no people identifiable. Image generation prompts stored in `dreamgully/assets/prompts/fictional/{brand-slug}/` for reuse.

---

## Tone of voice

Case study pages are written in the **DreamGully voice** (locked in `brand/identity.md` — confident, direct, not apologetic, not breathless). The same voice across real and fictional case studies. The difference is the framing (real = "we did this for a real client," fictional = "we designed this concept to demonstrate our process") — not the writing quality.

**Tone rules:**
- No superlatives without evidence ("best," "world-class," "unforgettable" — all banned unless the work itself is the evidence)
- No marketing-speak. Plain language.
- Specific over general. "We redesigned the navigation to surface the services menu" beats "we reimagined the user experience."
- Honest about scope. If we only did brand identity, we say "brand identity" — not "full creative direction."
- Fictional case studies are framed as craft demonstrations, not business outcomes. The work shown is real design work. The outcomes are not real business outcomes.

---

## Required meta per case study (front matter, not visible)

Each case study page has a hidden JSON block at the top of the file for tooling:

```json
{
  "slug": "brand-slug-here",
  "brandName": "Brand Name",
  "vertical": "Cafe",
  "geography": "Melbourne, AU",
  "tier": "medium",
  "source": "concept",
  "year": 2026,
  "services": ["brand-identity", "supporting-collateral"],
  "liveUrl": null,
  "heroImage": "assets/images/cases/{slug}/hero.jpg",
  "shipped": false,
  "clientPermissionOnFile": false,
  "trademarkCleared": true,
  "domainAvailable": true,
  "socialHandleAvailable": true,
  "lastUpdated": "2026-06-03"
}
```

**Required fields for fictional:** `trademarkCleared`, `domainAvailable`, `socialHandleAvailable` must all be `true` before the page ships. Verified by the trademark sweep (separate workflow).

**Required for real:** `clientPermissionOnFile` must be `true`. The permission artifact (WhatsApp screenshot, email, signed form) lives in `dreamgully/clients/{brand-slug}/permission.md`.

---

## File / folder structure

```
dreamgully/site/case-studies/
├── TEMPLATE.md                  ← this file
├── dreamgully.html              ← Case 1 (real, anchor)
├── beyond-basics.html           ← Case 2 (real)
├── vogue-atelier.html           ← Case 3 (real)
├── dubai-realestate.html        ← Case 4 (in-progress placeholder)
├── {fictional-slug-1}.html      ← Fictional 1 (fitness — light)
├── {fictional-slug-2}.html      ← Fictional 2 (skincare — light)
├── {fictional-slug-3}.html      ← Fictional 3 (cafe — medium)
├── {fictional-slug-4}.html      ← Fictional 4 (app/saas — medium)
├── {fictional-slug-5}.html      ← Fictional 5 (foam & fold — medium)
├── {fictional-slug-6}.html      ← Fictional 6 (restaurant — heavy)
└── {fictional-slug-7}.html      ← Fictional 7 (boutique hotel — heavy)
```

```
dreamgully/assets/images/cases/
├── {brand-slug}/
│   ├── hero.jpg
│   ├── overview-1.jpg
│   ├── work-{deliverable-number}.jpg
│   └── next-preview.jpg
```

---

## Reusable CSS classes (add to `index.html` `<style>` block)

These classes are added to the master stylesheet and reused across all case study pages.

```css
/* Case study shared */
.cs-hero { ... }
.cs-hero__eyebrow { ... }
.cs-hero__title { ... }
.cs-hero__tagline { ... }
.cs-hero__image { ... }
.cs-badge { ... }
.cs-badge--client { ... }
.cs-badge--in-progress { ... }
.cs-badge--concept { ... }
.cs-concept-callout { ... }  /* Per-page "Concept study" notice in the hero, fictional only */
.cs-overview { ... }
.cs-overview__grid { ... }
.cs-overview__tile { ... }
.cs-section-label { ... }
.cs-section-title { ... }
.cs-brief { ... }
.cs-work { ... }
.cs-work__deliverable { ... }
.cs-work__deliverable-image { ... }
.cs-results { ... }
.cs-results__metric { ... }
.cs-credits { ... }
.cs-next { ... }
```

The actual CSS will be added when the first case study page is built. We build the page first, then extract the shared CSS into reusable classes.

---

## Build order

1. **Template approval** (this document) — Taimoor reviews, adjusts, approves
2. **Real case studies** (4 pages, in this order):
   1. DreamGully (anchor, sets the bar)
   2. Beyond Basics (Etsy scope)
   3. Vogue Atelier (with the 500k + 1M reels prominently featured)
   4. Dubai real estate (in-progress placeholder)
3. **Fictional case studies** (7 pages, by tier):
   1. Fitness studio (light) — fastest to ship
   2. Skincare brand (light)
   3. Cafe (medium)
   4. App/SaaS (medium)
   5. Foam & Fold (medium)
   6. Restaurant (heavy)
   7. Boutique hotel (heavy)

For fictional case studies, the trademark sweep runs in parallel with name generation. We don't start a fictional case study page until the name is cleared.

---

## What this template does NOT include

- **Pricing or "starting from" copy** — that's for the services page, not case studies
- **Testimonial carousels** — single quote per case study, in the Results section, not a separate section
- **Related work** — replaced by "Next case study" footer, simpler and intentional
- **Process explanation** — that's the Process page (separate). Case study pages assume the visitor already understands the process.

---

## Approval

Template v1.0 awaiting Taimoor's review. After approval, the 4 real case study pages begin. Fictional work starts in parallel with trademark sweeps.
