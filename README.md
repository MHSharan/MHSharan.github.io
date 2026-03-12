# Md Mahbub Ul Hassan Sharan — Personal Site

This repository contains the source for my personal website: a static HTML/CSS portfolio showcasing research, writings, teaching, and a downloadable CV.

## Overview
- **Purpose**: Host a professional, accessible personal website and portfolio.
- **Tech Stack**: HTML5, Tailwind CSS (CDN), Google Fonts, FontAwesome icons, vanilla JavaScript
- **Mobile Responsive**: Yes, fully responsive design with sticky header and mobile menu
- **Build** : No build step required—fully static site

## Project Structure

```
d:/Github/MHSharan.github.io/
├── index.html              # About/Bio page (main entry)
├── about.html              # Landing/Hub page with links to all sections
├── resume.html             # CV display & PDF download
├── research.html           # Research projects & grants
├── writings.html           # Creative works & publications (with accordion)
├── teaching.html           # Teaching contributions & courses
├── styles.css              # Centralized custom CSS
├── tailwind-config.js      # Tailwind theme configuration
├── README.md               # This file
├── cv/
│   └── MHS_academic.pdf    # Downloadable academic CV
└── images/
    ├── logo.png            # Header logo
    ├── mhsharan.png        # Profile photo
    ├── writing cover.jpg   # Writing section cover
    └── Photography Cover.jpeg  # Photography cover
```

## Navigation
- **Entry Point**: Start at `about.html` (hub page with link grid to all sections)
- **Main Bio**: `index.html` shows full biography, contact info, and current roles
- **Consistent Navigation**: All pages have the same header (sticky), nav menu, and footer
- **Mobile Menu**: Hamburger menu auto-activates on screens < 1024px
- **Active Page Indicator**: Current page highlighted in nav with blue underline

## Features
✅ Responsive grid layout (1 col mobile, 2 col tablet, 3 col desktop)
✅ Sticky header with logo and navigation
✅ Mobile hamburger menu
✅ Colored social media icons (email, LinkedIn, Instagram, WordPress)
✅ Footer with auto-updating year
✅ Accordion functionality for publications (writings.html)
✅ Dark theme footer with visible social icons
✅ Smooth hover transitions on all interactive elements

## Styling & Customization

### Colors
- **Primary Blue**: `#1e3a8a` (Tailwind `blue-900`)
- **Secondary**: `#f59e0b` (Tailwind `amber-500`)
- **Dark Background**: `#0f1724`
- **Light Background**: `#f9fafb` (Tailwind `gray-50`)

### Custom CSS
All custom styles are in `styles.css`:
- `.site-header` — Header styling
- `.nav-link.active-nav` — Active page indicator
- `.page-section` — Fade-in animation
- `.card-cover` — Image container helper

### Tailwind Config
Theme colors defined in `tailwind-config.js`. Loaded before Tailwind CDN on all pages.

## Local Preview

1. From the repository root, run:
```bash
python -m http.server 8000
```

2. Open `http://localhost:8000/about.html` in your browser.

## Scripts
- **Footer Year**: `document.getElementById('year').textContent = new Date().getFullYear()`
- **Mobile Menu Toggle**: Hamburger button toggles menu visibility
- **Accordion Toggle**: Publications use `toggleAccordion()` function (writings.html)

## Notes
- This is a fully static site; no backend or build process required.
- All external resources (Tailwind, Google Fonts, FontAwesome) loaded via CDN.
- All pages use consistent HTML structure with header, main content, and footer.
- Logo links back to `index.html` on all pages for easy navigation home.