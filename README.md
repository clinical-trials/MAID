# Luminaria — New Mexico End-of-Life Options (website)

A patient-facing, multi-page static website for **Luminaria**, a proposed medical
aid-in-dying (MAID) care-coordination service operating under New Mexico's
**Elizabeth Whitefield End-of-Life Options Act** (NMSA 24-7C).

> **This is a demonstration site.** The brand name, phone number, email, and
> address are placeholders. Nothing here is medical or legal advice. Services
> described would be available only to New Mexico residents who qualify under the
> Act (mentally capable adults with a terminal prognosis of six months or less who
> can self-administer medication).

## Pages
- `index.html` — home
- `is-this-for-me.html` — eligibility
- `how-it-works.html` — the process
- `costs.html` — pricing & assistance
- `our-approach.html` — values / clinicians
- `faq.html` — frequently asked questions
- `contact.html` — free-consultation request
- `styles.css` — shared styles

## Tech
Plain HTML + CSS, no build step. Fonts via Google Fonts (Spectral + Figtree).

## Before going live
- **Contact form:** `contact.html` runs in safe demo mode (transmits nothing) until
  you set a real endpoint. Use a form/back-end provider that will sign a **HIPAA
  Business Associate Agreement (BAA)** — e.g. JotForm HIPAA, Formstack Healthcare,
  Paubox, Hushmail. Standard Formspree/Netlify Forms are **not** BAA-covered by
  default. Set both `data-endpoint` and `action` on the `#intake` form.
- **Safety:** every page carries a 988 Suicide & Crisis Lifeline notice; keep it.
- **Compliance & legal review** by New Mexico healthcare counsel is required before
  operating.

## GitHub Pages
Settings → Pages → deploy from `main` branch, root. The site is fully static.
