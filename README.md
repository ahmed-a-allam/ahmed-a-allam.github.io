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
