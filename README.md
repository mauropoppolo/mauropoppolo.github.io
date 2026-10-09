# Mauro Póppolo Fort — Resume Website

Personal resume site: one page, plain HTML, CSS and JavaScript. No framework, no build step.

## Structure

```
.
├── index.html                  the whole page and all text
├── css/styles.css              all styling; colours and fonts are set at the top
├── js/
│   ├── main.js                 mobile menu, fade-in on scroll
│   └── pong.js                 hidden game in the footer
└── assets/
    ├── portrait-web.jpg
    ├── cv-mauro-poppolo-fort.pdf
    └── certifications/
```

## View it locally

Open `index.html` in a browser. Nothing needs to be installed.

## Change content

| To change | Edit |
|-----------|------|
| Any text | `index.html` — each section starts with a comment such as `<!-- ===== ABOUT ===== -->` |
| Colours and fonts | The `:root { ... }` block at the top of `css/styles.css` |
| Portrait | Replace `assets/portrait-web.jpg` (square, about 1200 px, under 300 KB) |
| CV download | Replace `assets/cv-mauro-poppolo-fort.pdf`, same file name |
| Add a certificate | Put the image in `assets/certifications/`, copy one `<li>…</li>` block in the Certifications section. Keep `data-lightbox` on the links so they open in the pop-up |
| Add a job | Copy one `<li class="timeline__item reveal">…</li>` block in the Experience section |

## Publish (GitHub Pages)

One time:

1. Create a public GitHub repository named `<username>.github.io`.
2. Put the contents of this folder in it.
3. Repository → Settings → Pages → Source: branch `main`, folder `/ (root)`.

After every change:

```bash
git add .
git commit -m "Describe the change"
git push
```

The live site updates within a minute or two.

## License

© 2026 Mauro Póppolo Fort. All rights reserved.
