# maacdc.org Redesign — Design Spec

**Date:** 2026-06-14
**Owner:** Karthik Balasubramanian (MAAC Chair)
**Status:** Approved (brainstorming) → building

## Goal
Rebuild maacdc.org as a clean, fast, fully-accessible static site that reflects the
real depth of MAAC's work and fixes the current site's rough edges.

## Decisions (locked)
- **Platform:** Hand-authored semantic HTML + one shared CSS file, no build step.
  Deployed to GitHub Pages from new repo `kartbala/maacdc`.
- **Scope:** Full content overhaul (new design + rewritten/restructured content).
- **Deploy target this pass:** Build → push to GitHub → enable Pages (`*.github.io`
  preview). Do NOT touch maacdc.org DNS. HubSpot stays the public site until Karthik flips it.
- **Bios:** Names, roles + short 1-2 sentence bios drafted from MAAC context; Karthik reviews before going truly live.

## Problems being fixed
- "Something Sketchy" section title (placeholder cruft).
- Chair contact shown as personal Gmail → use `info@maacdc.org`.
- Footer leftover `accessibledc@gmail.com` + `@AccessibleDC` (pre-transfer branding) → removed.
- Thin content vs. real scope of MAAC's advocacy.

## Information architecture (8 pages)
1. **index.html** — Home: mission, what MAAC does, next meeting, quick links, report-card teaser.
2. **who-we-are.html** — Members + coordinator, statute § 50-2361.31, appointment/vacancy.
3. **what-we-do.html** — Arterial street priorities, advocacy areas, recent letters & resolutions.
4. **report-card.html** — 5 priority metrics + key stats.
5. **meetings.html** — Cadence, how to attend (Meet + dial-in), location, ASL accommodations.
6. **minutes.html** — Rolling Google Doc + YouTube links, full meeting-guest history.
7. **contact.html** — info@maacdc.org, vacancy application, mailing list.
8. **accessibility.html** — Accessibility statement (fitting for this body).

## Design language: "Civic Clarity"
- **Type:** Public Sans (body/UI), Fraunces (large display headlines only).
- **Color:** Navy `#102d7b` primary, DC-red `#a00405` accent (sparing), white + soft navy tint `#f4f6fc`.
- **Motif:** DC flag (3 stars, 2 bars) as recurring geometric signature.
- **Accessibility baseline:** WCAG 2.2 AA contrast min (AAA where feasible), skip link,
  semantic landmarks/headings, visible focus rings, full keyboard nav, descriptive alt text,
  `prefers-reduced-motion`, responsive to mobile, large touch targets. Automated a11y check before finish.
- **Contact mechanism:** `mailto:info@maacdc.org` + official MOTA vacancy application link. No third-party form.

## Assets
- `assets/img/maac-logo.png` — official DC-outline MAAC logo (301×121).
- `assets/img/hero-transit.jpg`, `assets/img/about-maacdc.jpeg` — carried from current site.
