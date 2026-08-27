# B Bad — Wedding DJ & MC Website

A single-page, no-build-step website promoting Andel James (DJ **B Bad**)'s
wedding DJ & MC services in Toronto & the GTA. Self-contained: `index.html` +
`style.css` + `assets/` — no framework, no bundler.

**Design:** hip-hop / record-culture aesthetic in a warm palette (espresso
`#1e140f`, terracotta `#c1573a`, gold `#c89b4a`, cream `#f7ede0`) — vinyl
records as the recurring visual motif (hero turntable graphic, the "Decades"
crate-digging section, the About avatar), bold condensed display type
(Big Shoulders) for headlines paired with a warm serif (Lora) for body
headings and a mono face (DM Mono) for label/tracklist-style copy. Buttons
use a stamped, hard-shadow style rather than soft pills. All fonts are
self-hosted, OFL-licensed (see `assets/fonts/*-OFL.txt`) — no external font
requests.

The whole page is built to drive one action: booking a consult call. Every
section ends in a "Check Availability" CTA, pricing is transparent, and the
FAQ + "How It Works" sections are there to remove booking friction.

## How to publish

This folder is self-contained and can be deployed on its own:

- **Netlify / Vercel:** point the site's base directory at `djbbad/`.
- **GitHub Pages:** Pages only serves from the repo root or `/docs`, so either
  move these files to their own repo (matching `djbbad.com`), or copy them
  into a `docs/` folder on whichever branch you point Pages at.
- **Any static host:** upload the contents of this folder as-is.

## ✅ Replace-before-launch checklist

These are called out with an HTML comment at the top of `index.html` too:

| Placeholder | Where | Replace with |
|---|---|---|
| `book@djbbad.com` | Contact form action, mailto links, footer | confirmed real inbox |
| `https://www.instagram.com/djbbad` | Header CTA area, gallery, footer, contact, JSON-LD | confirmed real handle |
| Pricing (`$1,395` / `$1,895` / `$2,595`) | `#packages` | confirmed current rates — these are samples |
| Testimonials | just above `#faq` | **sample copy** — swap in real couples' words, first names & season |
| Deposit / payment schedule | `#faq` | confirmed exact percentage & schedule |
| Travel fee threshold | `#faq` | confirmed distance/amount outside the GTA |

### Contact form

The inquiry form submits via [FormSubmit](https://formsubmit.co/) to
`book@djbbad.com`, no backend required. **The first submission triggers a
one-time confirmation email that must be clicked before FormSubmit will
deliver any further submissions.** Send a test inquiry and confirm the
activation email lands (check spam) before relying on this form for real
bookings.

### Assets

- `assets/fonts/` — self-hosted OFL font files (Lora, Work Sans, Big
  Shoulders, DM Mono) plus their license files.
- `assets/img/` — generated OG image, favicon PNGs and apple-touch-icon
  (warm vinyl-record graphic). `assets/favicon.svg` is the primary favicon.
- To swap in real photos (couples, dance floors, Andel DJing), replace the
  gradient tiles in `#gallery` with `<img>` tags — real photos will convert
  better than the current abstract placeholders once available.
