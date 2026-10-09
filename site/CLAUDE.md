# Mauro Póppolo Fort — Resume Website

Single-page personal resume site. Static HTML/CSS/JS, no framework, no build step, hosted on
GitHub Pages. Keep it that way: no npm, no bundler, no dependencies beyond Google Fonts.

## Files

- `index.html` — all content. Sections in order: Hero, About, Experience (with Education),
  Expertise, Certifications, Selected Impact, Contact, Footer, Pong modal.
- `css/styles.css` — all styling. Design tokens (colours, fonts) are CSS variables in `:root`.
  Class names follow BEM (`block__element--modifier`).
- `js/main.js` — hero name video (plays once; falls back to the last-frame image), mobile nav toggle, certificate pop-up (any link with `data-lightbox` opens its
  image in the `<dialog id="lightbox">` at the end of `index.html`), and reveal-on-scroll
  (`.reveal` → `.is-visible`).
- `js/pong.js` — footer easter egg. Reads `--bg` and `--accent` from the stylesheet.
- `assets/` — portrait, CV PDF, certificate images, the hero name animation
  (`name-animation.mp4`) and its last frame (`name-animation-lastframe.png`).

## Rules

- All facts must come from Mauro. Do not invent numbers, employers, dates or quotes.
- Do not publish a phone number or home address.
- Selected Impact: no salary figures, no statements about colleagues leaving or not being
  replaced, no named partners or transactions, unless Mauro confirms his employer has cleared it.
- A story in Selected Impact may end with an optional `<dl class="project__metrics">` row. Use it
  only for real, sourced numbers.
- New images: resize for the web first (portrait about 1200 px, certificates under 400 KB).
- Mobile-first: check every change at phone width as well as desktop.
- Section numbers (`01`–`06`) in `.section__index` must be renumbered when a section is added
  or removed, and the nav menu updated to match.

## Style

The current look (off-white, charcoal, muted blue accent, Fraunces + Inter) is inherited from
the template and is a placeholder until Mauro chooses his own. Change it through the `:root`
variables and the Google Fonts link in `index.html`, not by editing individual rules.
