# Legacy Jam 2026 — Website

A simple, accessible, single-page website for **Legacy Jam** (October 24–25, 2026, Toronto).
No build step — just `index.html` + `style.css` + `assets/`. The only JavaScript is a
~10-line progressive enhancement that shows/hides the back-to-top button; the button's
`href="#top"` link works with plain CSS scrolling even if it never runs.

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
| `https://forms.gle/REPLACE-ME-PARTNER` | "Become a Generations Partner" button | real Generations Partner sign-up form URL |
| `https://www.instagram.com/legacyjam` | hero, schedule, footer | confirmed Instagram handle |
| `info@legacyjam.com` | travel, footer, volunteer button | confirmed email address |
| ~~`assets/legacy-jam-logo.svg`~~ | header, hero, footer | ✅ done — official logo (vector, transparent background) |
| Crew bio + milestones | `#about` section | ✅ done — real bios/milestones from confirmed source copy |
| Artist Instagram handles | `#artists` section | verify every handle — several are best guesses (djbbad, djtimber, switchb, deadlymike, bgirltiff, bboymadtrack, bboystripes, mgbility, boobjester) |
| Legacy Party venue address | `#schedule` section (Sat, Oct 24 card) | confirmed venue name/address — site currently says only "a separate event at a different venue" |

### Logos

All partner and funder logos are real files in `assets/logos/` — nothing left to swap.
To add a new partner: drop the logo file in `assets/logos/` and add an `<li>` to the
matching `logo-row` list in `index.html`.

## 📋 Internal production notes (keep off the public site)

- [ ] Check if **Mad Track** is still available Oct 24
- [ ] Look into Exchanges opponents — **Stripes? Luigi?**
- [ ] Confirm airport shuttle logistics + who monitors the info@legacyjam.com inbox
- [ ] Confirm Eventbrite ticket tiers match: $20 dancer / $30 audience / $30–$90 workshops / $75 full festival pass
- [ ] Set up the Generations Partner sign-up form (school registration, promo code, VIP meet & greet)

## Confirmed details baked into the site

- **Oct 24 (Sat)** — Battle Day, 918 Bathurst St, Toronto, 12–7:30 PM; Legacy Party after
  (DJ Mensa × Cypher Playground confirmed — public site copy keeps this to a general
  "one night to remember" line, doesn't name the DJ/duo)
- **Oct 25 (Sun)** — Workshops & Panels, Unity Studio, 1560 Yonge St Suite 204, Toronto — cyphers, 2 panel discussions (mentorship; breaking & parallel careers), 4 workshops
- **Battles** — Generations (2v2 teacher×student, 10-yr age gap), Youth Cypher (Under 19), Pro Cypher (19+); Legacy Exchanges (Canada vs. international) is a showcase, not a competitive battle — lives in "The Festival" copy
- **Prizes** — Youth + Pro winners: flight & entry to Outbreak Europe 2027
- **Judges** — Ronnie (Full Force), Logistx (Red Bull BC One All Star), MGability
- **DJs** — Timber, B Bad; DJ Mensa for the Legacy Party
- **Funders** — Toronto Arts Council
- **Academic partner** — Sheridan College
- **Media partners** — Bboy Network, Outbreak Europe / The Legits
- **Generations Partners** — schools/crews that register students for the Generations Battle
- **MEC Crew** — produces Legacy Jam; organizing team is Piecez (Michael Prosserman), Boobjester (Roberto Veruela Jr.), B Bad (Andel James), Switch B (Adrian Bernard), and MEDÊIO (Rei Misiri)
