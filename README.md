# Outsource to Bangladesh

A small static site for OutsourceToBD.com — verified Bangladeshi tech companies,
real projects, real assurance.

**Live site:** https://tahsinapac-ops.github.io/otb-gitex/

## Pages

| File | URL | What it is |
| --- | --- | --- |
| [`index.html`](index.html) | `/` | Landing page. Intro plus a feature card linking to the current programme. |
| [`gitex.html`](gitex.html) | `/gitex.html` | The GITEX Global 2026 pitch — the full single-page case for a Bangladesh national pavilion. |
| [`flyer.html`](flyer.html) | `/flyer.html` | One-page summary — problem, fix, cost comparison, four USPs. Prints to a single A4 sheet. |

### The flyer

`flyer.html` is a leave-behind: bullets and visuals only, no prose. Hit
**Print / Save PDF** (or Ctrl/Cmd-P) and it lays out as exactly one A4 page —
verified, page count 1. The print stylesheet is fixed at 210×296 mm and the
responsive rules are scoped to `@media screen`, so shrinking a browser window
never affects what comes out of the printer.

### The GITEX 2026 page

- **The gap** — at GITEX Global 2025 India brought 237 companies to its pavilion
  and Pakistan 26 to a 156 m² one; Bangladesh had no national pavilion at all.
  PSEB reports roughly $40 of revenue for every dollar it spends subsidising
  its exhibitors. Every figure on the page is source-linked.
- **The argument** — why this is a positioning problem, not a lead-generation
  problem.
- **The programme** — the offer in three parts, led by five training sessions
  on how to actually win clients on the floor.
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
assets/hero.jpg   optional — see below
```

### The hero photo

`assets/hero.jpg` is the GITEX Global show floor at the Dubai World Trade
Centre, 2022 — photo by **Moneymystica**, licensed
**[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)**, via
[Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Gitex-global.jpg).
The credit line under the image on the page satisfies the licence; **do not
remove it** while this photo is in use.

To swap in your own photo, replace `assets/hero.jpg` (landscape, 1600×1200 or
wider) and update or delete that credit line to match. If the file is missing
the page falls back to the built-in SVG illustration, so it never breaks.

Two caveats with the current photo: it is 1024×768, which is soft on large
screens, and it shows identifiable people. A CC licence covers copyright, not
personality rights — your own photography avoids both problems.

## Deployment

Hosted on GitHub Pages from the `main` branch root. Any push to `main`
republishes the site.
