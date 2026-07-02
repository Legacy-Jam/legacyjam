# Legacy Jam 2026 — Website

A simple, accessible, single-page website for **Legacy Jam** (October 23–25, 2026, Toronto).
No build step, no JavaScript — just `index.html` + `style.css` + `assets/`.

**Design:** gold-on-navy palette pulled from the Legacy Jam logo set (deep navy `#0c111c`,
cream `#f4e9cf`, gold `#e0ae5a`, maroon `#64251e`), with a script typeface (Yellowtail) echoing
the brand wordmark, gold-gradient headings, subtle film grain, hairline gold rules echoing the
"— JAM —" mark, and a timeline-styled schedule. All decorative; content order and reading
clarity come first, and `prefers-reduced-motion` disables the entrance animation.

## How to publish

Easiest option — GitHub Pages:

1. Merge this branch to `main`.
2. Repo **Settings → Pages → Source: Deploy from a branch → `main` / root**.
3. The site goes live at `https://<username>.github.io/legacyjam/`.

Or drag the folder into Netlify / Vercel, or upload to any web host.

## ✅ Replace-before-launch checklist

These placeholders are marked with `TODO` comments in `index.html`:

| Placeholder | Where | Replace with |
|---|---|---|
| `https://www.eventbrite.ca/e/legacy-jam-2026` | every "Get Tickets" button | real Eventbrite event URL (search-and-replace) |
| `https://forms.gle/REPLACE-ME` | "Register to Battle" button | real battle registration form URL |
| `https://www.instagram.com/legacyjam` | hero, schedule, footer | confirmed Instagram handle |
| `shuttle@legacyjam.ca` / `hello@legacyjam.ca` | travel section, footer | confirmed email addresses |
| Text wordmark in hero | `#top` section | official logo file → `assets/legacy-jam-logo.png` (an `<img>` tag is ready in a comment) |
| Legacy Talks topics | `#festival` section | the two confirmed talk topics from the deck |
| Crew bio | `#about` section | final copy from the crew bio file |
| Friday Oct 23 venue | `#schedule` | opening-night location once confirmed |

### Logos

Real logos are in place for **Toronto Arts Council, Sheridan College, Outbreak Europe and
Bboy Network** (`assets/logos/`). Still showing **styled placeholder SVGs** — to swap in a
real logo, save the official file over the placeholder using the same filename (or update
the `src` in `index.html`):

- **Unity Charity** — <https://www.unitycharity.com>
- **Expand the Cypher / Cypher Playground** — request from partners
- **National partners** — real logos are in for BRKN Québec, WNTR MSSV, Break TO and The
  Flava Factory. Placeholder tiles remain for The Legits Blast (`legits-blast.svg`),
  Break City (`break-city.svg`), ABA (`aba.svg`), The Spot Arts Community (`the-spot.svg`),
  Breaking Canada (`breaking-canada.svg`) and TUFF (`tuff.svg`); overwrite
  each placeholder with the real logo file.

## 📋 Internal production notes (keep off the public site)

- [ ] Check if **Mad Track** is still available Oct 24
- [ ] Look into Exchanges opponents — **Stripes? Luigi?**
- [ ] Confirm Friday Oct 23 opening-night venue
- [ ] Confirm shuttle logistics + who monitors the shuttle inbox
- [ ] Confirm Eventbrite ticket tiers match: $20 dancer / $30 audience / $30–$70 workshops / $75 full weekend

## Confirmed details baked into the site

- **Oct 24 (Sat)** — Battle Day, 918 Bathurst St, Toronto, 12–7 PM; Legacy Party after (DJ Mensa × Cypher Playground)
- **Oct 25 (Sun)** — Workshops & Talks, Unity Studio, 1560 Yonge St Suite 204, Toronto
- **Battles** — Generations (2v2 teacher×student, 10-yr age gap), Youth Cypher (U18), Pro Cypher, Legacy Exchanges (Canada vs. international)
- **Prizes** — Youth + Pro winners: flight & entry to Outbreak Europe 2027
- **Judges** — Ronnie (Full Force), Logistx (Red Bull BC One All Star), MGability
- **DJs** — Timber, B Bad; DJ Mensa for the Legacy Party
- **Funders** — Toronto Arts Council, Sheridan College
- **Media partners** — Bboy Network, Outbreak Europe / The Legits
