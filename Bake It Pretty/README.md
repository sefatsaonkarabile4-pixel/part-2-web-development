# Bake It Pretty — Website Project

**Student:** Onkarabile Sefatsa
**Project:** Part 2 — CSS Styling, Responsive Design & GitHub
**Repository:** [paste your GitHub URL here]

---

## 1. Project Overview

A responsive, pastel-pink bakery website built with semantic HTML5 and an
external CSS stylesheet. The site showcases the bakery's story, packages,
pricing, and contact details, and adapts to desktop, tablet, and mobile.

---

## 2. File & Folder Structure
Bake It Pretty/
├── index.html
├── about.html
├── services.html
├── enquiry.html
├── contact.html
├── style.css
├── README.md
├── .gitignore
├── images/


## 3. Changelog

### Part 2.1 — External Stylesheet
- Created `style.css` and linked it to every HTML page via
  `<link rel="stylesheet" href="style.css">` inside `<head>`.
- Removed all inline `style="…"` attributes and embedded `<style>` blocks.

### Part 2.2 — Base Style + CSS Reset
- Universal reset: `*, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }`.
- Base `font-family` (Quicksand), `font-size`, `line-height`, colour and background set on `body`.
- Colour palette + spacing scale defined using CSS custom properties (`:root`).

### Part 2.3 — Typography
- Modular scale: `--fs-xs` (0.8rem) → `--fs-xl` (2.6rem).
- Applied `font-family`, `font-size`, `font-weight`, `line-height`, and `letter-spacing` to body and h1–h4.

### Part 2.4 — Layout
- **Flexbox** for body, header, nav, hero, footer.
- **CSS Grid** for `.treat-grid` (`repeat(auto-fit, minmax(220px, 1fr))`).
- Uses `display`, `flex-direction`, `justify-content`, `align-items`, `grid-template-columns`.

### Part 2.5 — Visual Styles & Pseudo-classes
- `color`, `background-color`, `border`, `box-shadow` applied throughout.
- Interactive states: `:hover`, `:focus`, `:active` on nav and cards.

### Part 3.1 — Responsive Breakpoints
- Breakpoints: mobile (≤600px), tablet (≥601px), desktop (≥1024px), large (≥1400px).
- Treat grid: **4 → 2 → 1** columns as screen narrows.
- Hero: **row** on desktop → **column** on mobile.
- Nav padding, heading sizes, and footer alignment adjusted per breakpoint.

### Part 3.2 — Relative Units
- `rem` for all font sizes, padding, margin, and gaps.
- `%` for widths: `.bakery-storefront { width: 100%; }`, `.awning { width: 80%; }`.
- `100vh` for `body { min-height }`.

### Part 3.3 — Responsive Images
- Storefront image uses `srcset` + `sizes` for resolution switching.
- `<picture>` element example documented in `index.html` comments.
- `loading="lazy"`, `decoding="async"`, and `max-width:100%` applied.

### Part 3.4 — Testing
- Tested with Chrome DevTools device toolbar.
- Screenshots captured at 1440px, 768px, 375px and 1920px (see section 4).

### Feedback Edits from Part 1
- Added HTML5 semantic elements (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
- Added consistent navigation on all pages.
- Fixed broken filenames (`Contact Us .html` → `contact.html`, `Services.html` → `services.html`).
- Added `<meta name="description">` per page.
- Added HTML comments to explain structure.
- Added this README with changelog and references.

---

## 4. Screenshots (Section 3.4)

### Desktop — 1440px
![Desktop 1440](screenshots/desktop-1440.png)
*Multi-column treat grid (4 cols); hero text + image side by side.*

### Tablet — 768px
![Tablet 768](screenshots/tablet-768.png)
*Treat grid in 2 columns; nav still in one row.*

### Mobile — 375px
![Mobile 375](screenshots/mobile-375.png)
*Single-column layout; hero stacks vertically; footer centred.*

### Large Desktop — 1920px
![Desktop 1920](screenshots/desktop-1920.png)
*Max-width container keeps content centred and readable.*

---

## 5. Skills & References

- MDN — HTML5 Semantic Elements:
  https://developer.mozilla.org/en-US/docs/Web/HTML/Element
- MDN — Responsive Images (`srcset`, `sizes`, `<picture>`):
  https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images
- CSS-Tricks — Complete Guide to Flexbox:
  https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- CSS-Tricks — Complete Guide to Grid:
  https://css-tricks.com/snippets/css/complete-guide-grid/
- Google Fonts — Quicksand:
  https://fonts.google.com/specimen/Quicksand
- Squoosh — image compression for srcset variants:
  https://squoosh.app
- Keep a Changelog:
  https://keepachangelog.com/

---

## 6. Author

**Onkarabile Sefatsa** · Bake It Pretty Bakery · 2025