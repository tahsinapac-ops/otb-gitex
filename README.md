# Outsource to Bangladesh

A small static site for OutsourceToBD.com — verified Bangladeshi tech companies,
real projects, real assurance.

**Live site:** https://tahsinapac-ops.github.io/otb-gitex/

## Pages

| File | URL | What it is |
| --- | --- | --- |
| [`index.html`](index.html) | `/` | Landing page. Intro plus a feature card linking to the current programme. |
| [`gitex.html`](gitex.html) | `/gitex.html` | The GITEX Global 2026 pitch — the full single-page case for a Bangladesh national pavilion. |

### The GITEX 2026 page

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

Plain HTML and CSS — no build step, no dependencies. Serve the folder:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

(Opening `index.html` directly from the filesystem works too.)

## Structure

```
index.html        landing page
gitex.html        GITEX Global 2026 programme (self-contained, images inlined)
assets/logo.png   wordmark, used by the landing page
```

## Deployment

Hosted on GitHub Pages from the `main` branch root. Any push to `main`
republishes the site.
