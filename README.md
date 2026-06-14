# maacdc.org

Static website for the **Multimodal Accessibility Advisory Council (MAAC)** — an
advisory body of the Government of the District of Columbia that advises the Mayor,
the DC Council, and District agencies on multimodal accessibility for people with
disabilities. Established under D.C. Code § 50-2361.31.

## How it's built

Plain semantic HTML + one shared CSS file. **No build step, no framework, no dependencies.**
Edit an `.html` file, commit, and GitHub Pages publishes it.

```
index.html            Home
who-we-are.html       Members, coordinator, the statute
what-we-do.html       Priorities, advocacy areas, letters & resolutions
report-card.html      The five priority metrics
meetings.html         Schedule, how to attend, accommodations
minutes.html          Minutes/recordings links + meeting-guest history
contact.html          Contact, apply for a seat, mailing list
accessibility.html    Accessibility statement
404.html              Not-found page
assets/css/styles.css Design system ("Civic Clarity")
assets/js/nav.js      Mobile-menu toggle (progressive enhancement)
assets/img/           Logo + photography
docs/                 Design spec
```

## Editing common things

- **Next meeting / dial-in:** `meetings.html` (and the callout on `index.html`).
- **Members:** the member cards in `who-we-are.html`.
- **A new letter/resolution:** add a `<li>` to the `.doc-list` in `what-we-do.html`.
- **A new meeting in the history table:** add a `<tr>` at the top of the table in `minutes.html`.

## Design

Type: Public Sans (body/UI) + Fraunces (display). Color: MAAC navy `#102d7b` with a
DC-flag red `#a00405` accent. Motif: the DC flag (three stars, two bars). Built to
WCAG 2.2 AA (AAA where practical) — see `accessibility.html` and `docs/`.

## Deploying to a custom domain

This repo currently publishes to GitHub Pages (`*.github.io`). To serve `maacdc.org`
from it, add a `CNAME` file containing `www.maacdc.org`, set the custom domain in the
repo's Pages settings, and point Namecheap DNS at GitHub Pages — **without disturbing
the existing email (MX) records for `@maacdc.org`.**
