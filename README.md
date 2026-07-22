# Outsource to Bangladesh · GITEX Global 2026

A single-page pitch site making the case for a Bangladesh national pavilion at
GITEX Global 2026 in Dubai — one pavilion, twenty companies, at a fraction of
the cost of exhibiting alone.

**Live site:** https://tahsinapac-ops.github.io/otb-gitex/

## What's on the page

- **The gap** — Bangladesh had zero exhibitors at GITEX Global 2024, against 199
  Indian exhibitors and an 80+ firm Pakistani national pavilion that PSEB
  reported generated $10.5M in business leads.
- **The argument** — why this is a positioning problem, not a lead-generation
  problem.
- **The programme** — the offer, broken into three parts.
- **Cost calculator** — an interactive slider showing how the shared-pavilion
  price falls as more companies join.
- **Reserve** — the referral offer: bring a company you trust, you both pay less.

## Running it locally

It's one self-contained HTML file — no build step, no dependencies. Open
`index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Hosted on GitHub Pages from the `main` branch root. Any push to `main`
republishes the site.
