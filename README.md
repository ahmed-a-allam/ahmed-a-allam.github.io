# ahmed-a-allam.github.io

Personal website of **Ahmed Adel Allam** — bioinformatics researcher (MSc Biotechnology, The American University in Cairo).

Live at: https://ahmed-a-allam.github.io/

## Structure

- `index.html` — single-page site (About, Research, Projects, Apps & Tools, Writing, Contact), English + Arabic content side by side
- `style.css` — styles; uses CSS logical properties so the same layout works LTR and RTL

## Language toggle

Every translatable piece of text exists twice, marked `data-lang="en"` and `data-lang="ar"`.
The header button switches `<html lang>` / `<html dir>` and CSS hides the other language.
The choice is remembered in `localStorage`.

## Content notes

- Publications show a neutral "Co-author" label (EN) / "مؤلف مشارك" (AR) instead of the author order. Titles are the published titles.
- There are no visible placeholder boxes. When the Google Scholar profile, project links, apps, tools or writing pieces are ready, add them to `index.html` in both English and Arabic.

## Adding an app teaser card

1. Put the logo in `images/` (square PNG or SVG, e.g. `images/myapp.png`).
2. In `index.html`, inside the Apps & Tools section's `<div class="cards">`, add a card like this (both languages):

```html
<article class="card">
  <img class="app-logo" src="images/myapp.png" alt="" width="56" height="56" loading="lazy">
  <p class="card-meta"><span data-lang="en">Mobile app</span><span data-lang="ar">تطبيق جوال</span></p>
  <h3>App name</h3>
  <p data-lang="en">One short line about what kind of app it is.</p>
  <p data-lang="ar">سطر واحد قصير عن نوع التطبيق.</p>
  <p class="card-link"><span class="badge-soon"><span data-lang="en">Coming soon</span><span data-lang="ar">قريبًا</span></span></p>
</article>
```

3. Commit and push to `main`; GitHub Pages republishes in a minute or two.
