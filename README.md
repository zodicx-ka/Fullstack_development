# CET138 Mastery Portfolio — Yash Raj Sharma

> **Module:** CET138 Full Stack Development
> **Student:** Yash Raj Sharma · `bj02yl`
> **Course:** BSc Computer System Engineering — University of Sunderland
> **Submitted:** March 2026

---

## Overview

A fully responsive, interactive ePortfolio built as part of Assignment 1 for CET138 Full Stack Development. The portfolio demonstrates practical understanding across five core topic areas through live working examples, annotated code snippets, and interactive demonstrations — all implemented without any backend or build tools.

---

## Live Demos Inside the Portfolio

| Section | Demo |
|---|---|
| Full Stack Development | Interactive 3-tier architecture diagram with hover tooltips |
| HTML | AJAX contact form with HTML5 validation, fieldset/legend, and simulated submission |
| CSS | Tabbed showcase — CSS Grid gallery, Flexbox navbar, animations, CSS variables with theme switching |
| CSS | Profile card with animated gradient, pulsing status dot, slide-in social icons |
| Bootstrap | Interactive product store with cart, toast notifications, accordion, modal, and responsive navbar |
| JavaScript | Weather widget (simulated API), priority-based to-do list with localStorage, async/await demo |

---

## Project Structure

```
/
├── index.html          # Main portfolio page — all 5 sections
├── css/
│   └── style.css       # All custom styles, design tokens, theme overrides
└── js/
    └── script.js       # All interactive behaviour
```

No build step, no package manager, no framework dependencies beyond the CDN links already in `index.html`.

---

## Technologies Used

| Technology | Version | Purpose |
|---|---|---|
| HTML5 | — | Semantic page structure, forms, accessibility |
| CSS3 | — | Custom properties, Grid, Flexbox, animations |
| Bootstrap | 5.3.3 | Responsive grid, components, JS plugins |
| JavaScript (ES6+) | — | DOM manipulation, async/await, localStorage |
| Font Awesome | 6.4.0 | Icons throughout |
| Google Fonts | — | Poppins, Open Sans, Fira Code |
| AOS | 2.3.1 | Scroll-triggered reveal animations |

All dependencies are loaded via CDN — no installation required.

---

## Features

- **Responsive** — Mobile-first layout, tested across 4 breakpoints (576 / 768 / 992 / 1200px)
- **Theme switching** — Light, Dark, and Purple themes via CSS custom properties; switching is instant and affects every component
- **Accessible** — Semantic HTML5, ARIA labels, `<fieldset>`/`<legend>`, keyboard-navigable Bootstrap components
- **XSS protection** — User input in the to-do list is sanitised via `escapeHtml()` before DOM insertion
- **localStorage persistence** — To-do list survives page reloads
- **Print styles** — Decorative elements hidden, sections preserved across page breaks
- **Scroll-to-top button** — Appears after 500px scroll, smooth-scrolls to top
- **Active nav highlight** — Current section highlighted in navbar on scroll

---

## How to Run

1. Download or clone the repository
2. Open `index.html` in any modern browser

That's it — no server, no build step, no dependencies to install.

```bash
# Or serve locally with any static server, e.g.:
npx serve .
# then visit http://localhost:3000
```

---

## Sections

### 1 — Full Stack Development
Explains the three-tier architecture (presentation, logic, data), the technologies at each layer, how front end and back end communicate via HTTP/REST APIs, and why full stack understanding is valuable in professional development.

### 2 — HTML
Demonstrates semantic HTML5 structure, HTML5 form features (input types, constraint validation attributes, `fieldset`, `legend`), accessibility with ARIA, and a fully functional AJAX contact form with loading state and error handling.

### 3 — CSS
Covers CSS custom properties as a design token system, CSS Grid (named template areas), Flexbox, keyframe animations, transitions, and media queries. Includes a live theme switcher demonstrating how `[data-theme]` attribute selectors cascade through an entire UI. Also features a hand-crafted profile card component showcasing gradients, hover effects, and the pulsing status animation — all without JavaScript.

### 4 — Bootstrap 5
An interactive product store demonstrates the grid, cards, badges, a toast notification system, Bootstrap accordion, and a modal dialogue — all wired together with Bootstrap's data-attribute API and JavaScript plugin system.

### 5 — JavaScript
Two live demos: a weather widget using `async/await` and simulated `fetch()` with full loading/error state handling, and an advanced to-do list with priority levels, filter tabs (All / Active / Completed), `localStorage` persistence, and XSS sanitisation. Annotated code snippet demonstrates the async/await pattern in full.

---

## Known Limitations

- The weather widget uses **simulated data** — random values are generated locally. A real implementation would require an OpenWeatherMap API key substituted into `getWeather()` in `script.js`.
- The contact form submission is **simulated** via `fakeApiCall()` with a 1.5 s delay and 90% success rate. To connect it to a real endpoint, replace the `fakeApiCall(formData)` call with a `fetch()` to a service such as Formspree or Getform.

---

## Browser Support

| Browser | Supported |
|---|---|
| Chrome 90+ | ✅ |
| Firefox 88+ | ✅ |
| Safari 14+ | ✅ |
| Edge 90+ | ✅ |
| IE 11 | ❌ (CSS custom properties not supported) |

---

## Assessment Context

This project was submitted as **Assignment 1 (ePortfolio)** for CET138 Full Stack Development, worth **30% of the overall module mark**. The five portfolio sections map directly to the five grading criteria in the assessment rubric.

---

## Author

**Yash Raj Sharma**
Student ID: `bj02yl`
BSc Computer System Engineering
University of Sunderland
