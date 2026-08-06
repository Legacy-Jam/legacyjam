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
| ~~`https://www.eventbrite.ca/e/legacy-jam-2026`~~ | every "Get Tickets" button | ✅ done — links to `https://legacyjam2026.eventbrite.ca` |
| ~~`https://forms.gle/REPLACE-ME`~~ | "Register to Battle" buttons | ✅ done — links to `https://breakkonnect.com/event/4898` |
| ~~`https://forms.gle/REPLACE-ME-PARTNER`~~ | "Become a Generations Partner" button | ✅ done — built-in application at `generations-partner.html` |
| ~~`https://www.instagram.com/legacyjam`~~ | hero, artists, schedule, footer | ✅ done — confirmed handle `@legacy.jam` |
| `info@legacyjam.com` | travel, footer, volunteer button | confirmed email address |
| ~~`assets/legacy-jam-logo.svg`~~ | header, hero, footer | ✅ done — official logo (vector, transparent background) |
| Crew bio + milestones | `#about` section | ✅ done — real bios/milestones from confirmed source copy |
| Artist Instagram handles | `#artists` section | verify every handle — several are best guesses (djbbad, djtimber, switchb, deadlymike, bgirltiff, bboymadtrack, bboystripes, mgbility, boobjester) |
| Legacy Party venue address | `#schedule` section (Sat, Oct 24 card) | confirmed venue name/address — site currently says only "a separate event at a different venue" |

### Logos

All partner and funder logos are real files in `assets/logos/` — nothing left to swap.
To add a new partner: drop the logo file in `assets/logos/` and add an `<li>` to the
matching `logo-row` list in `index.html`.

### Volunteer & Generations Partner applications

`volunteer.html` and `generations-partner.html` are standalone, fully working
application forms (linked from the "Apply to volunteer" and "Become a Generations
Partner" buttons on the main page). Both submit via
[FormSubmit](https://formsubmit.co/) straight to `info@legacyjam.com` — no signup,
no server, no build step, matching the rest of the site:

- **Volunteer form** — contact info, 19+ confirmation, areas of interest, skills,
  whether they drive / have car access, availability, a note about the mandatory
  orientation (date/time TBC), emergency contact, and a waiver & release of
  liability (typed-name e-signature + agreement checkbox).
- **Generations Partner form** — contact info, attendee names, high-res logo
  upload, arrival/departure flight details, accommodation, airport pickup/drop-off
  requests, and checkboxes for which optional benefits they want (VIP meet &
  greet, event table, Sunday organizers' conversation).

**⚠️ URGENT — likely already affecting real submissions:** the *first* submission
ever made to `info@legacyjam.com` through FormSubmit triggers a one-time
confirmation email — someone monitoring that inbox needs to click "Activate Form"
in it, or submissions are silently accepted by FormSubmit but never delivered
(visitors still see a success message on the site, so this can go unnoticed).
This only needs to happen once and covers both forms. Check the inbox's spam/junk
folder too — search for an email from FormSubmit. Until this is confirmed done,
assume any volunteer or Generations Partner applications submitted so far were
lost and may need to be re-requested from applicants.

## 📋 Internal production notes (keep off the public site)

- [ ] Check if **Mad Track** is still available Oct 24
- [ ] Look into Exchanges opponents — **Stripes? Luigi?**
- [ ] Confirm airport shuttle logistics for Generations Partners (now the only guests offered a pre-booked shuttle) + who monitors the info@legacyjam.com inbox
- [ ] Confirm Eventbrite ticket tiers match: $20 dancer / $30 audience / $30–$90 workshops / $75 full festival pass
- [ ] **URGENT:** Activate FormSubmit for info@legacyjam.com — confirmed not delivering submissions yet (see "Volunteer & Generations Partner applications" above)
- [ ] Have the volunteer waiver text in `volunteer.html` reviewed — it's a reasonable starting template, not legal advice
- [x] Set up the Generations Partner sign-up form (school registration, promo code, VIP meet & greet)

## Confirmed details baked into the site

- **Oct 24 (Sat)** — Battle Day, 918 Bathurst St, Toronto (not wheelchair accessible),
  12–7:30 PM; Legacy Party after (DJ Mensa × Cypher Playground confirmed —
  public site copy keeps this to a general "one night to remember" line, doesn't name the DJ/duo)
- **Oct 25 (Sun)** — Workshops & Panels, Unity Studio, 1560 Yonge St Suite 204, Toronto (wheelchair accessible) — cyphers, 2 panel discussions (mentorship; breaking & parallel careers), 4 workshops
- **Battles** — Generations (2v2 teacher×student, 10-yr age gap), Youth Cypher (Under 19), Pro Cypher (19+); Legacy Exchanges (Canada vs. international) is a showcase, not a competitive battle — lives in "The Festival" copy
- **Prizes** — Youth + Pro winners: flight & entry to Outbreak Europe 2027
- **Judges** — Ronnie (Full Force), Logistx (Red Bull BC One All Star), MGability
- **DJs** — Timber, B Bad; DJ Mensa for the Legacy Party
- **Funders** — Toronto Arts Council
- **Academic partner** — Sheridan College (not yet confirmed for 2026: logo hidden on site until they confirm)
- **Media partners** — Bboy Network, Outbreak Europe / The Legits
- **Generations Partners** — schools/crews that register students for the Generations Battle
- **MEC Crew** — produces Legacy Jam; organizing team is Piecez (Michael Prosserman), Boobjester (Roberto Veruela Jr.), B Bad (Andel James), Switch B (Adrian Bernard), and MEDÊIO (Rei Misiri)
