# BUDT748 Fall 2026 — Client Side Technologies Project

A three page responsive website designed in **Figma** and rebuilt with
**HTML, CSS, and Bootstrap 5**.

**Student:** Manish Malhotra
**Course:** BUDT748 — Client Side Technologies, Fall 2026
**Professor:** Dr. Paul T. Shapiro
**Institution:** Robert H. Smith School of Business, University of Maryland

---

## Live Site

<!-- Paste your GitHub Pages URL here once it is deployed -->
https://YOUR-USERNAME.github.io/budt748-website/

---

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero banner, call-to-action buttons, three feature cards, course snapshot |
| About | `about.html` | Course description, course details panel, tools grid |
| Contact | `contact.html` | Professor / TA / student contacts and a Bootstrap contact form |

---

## Project Structure

```
budt748-website/
├── index.html          Home page
├── about.html          About page
├── contact.html        Contact page
├── css/
│   └── styles.css      Custom stylesheet (loaded after Bootstrap)
├── images/             Figma exports and screenshots
└── README.md
```

---

## Design System

Colors were defined in Figma and carried into CSS as custom properties
in `:root`.

| Token | Hex | Used for |
|-------|-----|----------|
| `--navy` | `#0B1020` | Page background |
| `--navy-soft` | `#131A33` | Card and panel background |
| `--text-main` | `#F5F7FF` | Headings and primary text |
| `--text-muted` | `#B8C1D9` | Secondary / body text |
| `--accent` | `#7C5CFC` | Buttons and highlights |
| `--cyan` | `#2DE2E6` | Links and gradient accents |

**Typography:** Montserrat (400, 500, 600, 700) loaded from Google Fonts.

---

## Bootstrap Components Used

- **Navbar** — `navbar navbar-expand-lg` collapses into a hamburger menu below 992px
- **Grid system** — `container` / `row` / `col-md-4`, `col-md-6`, `col-lg-3`, `col-lg-5`, `col-lg-7`
- **Buttons** — `btn` base class extended by custom `.btn-accent` and `.btn-ghost`
- **Forms** — `form-label`, `form-control`, and an alert for the confirmation message
- **Utilities** — `h-100`, `g-4`, `mb-3`, `text-center`, `d-flex`, `justify-content-end`

Bootstrap is loaded from the CDN, so there are no files to install:

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

---

## Custom CSS Beyond Bootstrap

- CSS custom properties for the whole color palette
- A radial purple glow behind each hero section
- An animated underline that grows under the active navigation link
- Hover lift and glow on the call-to-action buttons
- Hover lift and purple border on the info cards
- Dark theme restyling of Bootstrap form controls
- Media queries at 991px and 767px for tablet and phone layouts

---

## Running Locally

1. Clone or download this repository.
2. Open the folder in **VS Code**.
3. Install the **Live Server** extension.
4. Right click `index.html` and choose **Open with Live Server**.

An internet connection is required the first time so the Bootstrap and
Montserrat CDN files can load.

---

## Deployment

Published with **GitHub Pages** from the `main` branch, root folder.
