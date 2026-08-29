# Pierce Maheu — Jekyll Site

A 6-page Jekyll site for Pierce Maheu (classical & fingerstyle guitar,
Charleston Lowcountry), structurally modeled on tomofujitamusic.com:
centered nav with active-page underline, alternating full-bleed
light/dark bands, and full-bleed black-and-white photo breaks between
sections. Palette and copy are Pierce's own ("classical guitar, but
coastal") — cream/charcoal instead of pure black/white, with a single
teal accent as the signature detail.

## Pages
- `index.html` — Home (split hero + teasers)
- `about.html` — About Pierce
- `lessons.html` — Lesson formats & rates
- `testimonials.html` — Student/parent testimonials
- `gallery.html` — Photo grid
- `contact.html` — Contact form + details

## Photo placeholders
Every photo slot is a dashed-outline placeholder with a label describing
the shot needed (e.g. "PHOTO — PIERCE PLAYING CLASSICAL GUITAR, STUDIO").
Search for `photo-band.html` in each page to find and swap these once
real photography is available — just replace the include with a real
`<img>` or `<picture>` tag using the same wrapper class for sizing.

## Running locally
Requires Ruby + Bundler.

```bash
bundle install
bundle exec jekyll serve
```

Then visit `http://localhost:4000`.

## Deploying to GitHub Pages
1. Push this repo to GitHub.
2. In the repo's Settings → Pages, set the source to the `main` branch
   (root). GitHub Pages will build it automatically via Jekyll —
   no build step needed on your end.
3. If using a custom domain, add it in Settings → Pages and update
   `url` in `_config.yml` to match.

## Still needs your input
- **Photos**: nine placeholder slots total across the site (see above).
- **Contact form**: not yet wired to a backend. Easiest path is
  [Formspree](https://formspree.io) (free tier) — sign up, then set
  the `action` attribute in `contact.html`'s `<form>` tag to your
  Formspree endpoint URL. No JavaScript required.
- **Lesson rates**: placeholder numbers in `lessons.html` — update to
  match actual pricing.
- **Email address**: `hello@piercemaheu.com` is a placeholder — update
  in `_includes/footer.html` and `contact.html`.
