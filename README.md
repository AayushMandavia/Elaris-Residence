# ELARIS Residence — Contemporary Mediterranean Residences

> An ultra-luxury, boutique residential showcase on Spain's New Golden Mile (Estepona / Málaga), pairing bespoke Mediterranean architecture with fluid web animation choreography.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)
![License](https://img.shields.io/badge/license-Proprietary-gold.svg)
![Status](https://img.shields.io/badge/status-Production--Ready-success.svg)

---

## Overview

**ELARIS Residence** is an exclusive boutique residential enclave of 25 contemporary homes situated between Marbella and Estepona. Designed around privacy, wellbeing, and timeless Mediterranean living, each residence features expansive private terraces, landscaped natural materials, and panoramic coastal vistas.

This web showcase delivers a digital brand experience matching the physical architecture's elegance—combining continuous velocity-tied micro-animations, editorial typography, GSAP text morphing, and interactive floor plans.

---

## Architectural & Experience Highlights

- **Boutique Privacy**: 25 private residences comprising Ground Floor Garden Suites, Mid-Level Residences, and Dual-Level Penthouse Duplexes with rooftop solariums.
- **Resort Amenities**: Private wellness spa, sauna, heated saltwater pool, children's splash pool, fitness studio, landscaped sensory walking paths, and underground EV-ready parking.
- **Natural Materiality**: Hand-carved sandstone facades, warm timber louvers, lime plaster textures, floor-to-ceiling double-glazed minimalist glass curtains.
- **Location**: Prime Costa del Sol address — *Paseo de las Palmeras 18, 29688 New Golden Mile, Málaga, Spain*.

---

## Creative Engineering & Architecture

- **Smooth Inertial Scrolling**: Powered by `@studio-freight/lenis` for 1:1 hardware-accelerated momentum scroll dynamics across desktop and touch displays.
- **Scroll Choreography**: Custom GSAP timelines orchestrating word-spacing stretching, sticky section transitions, architecture curtain unveils, and multi-layer parallax depth.
- **SplitText Typography**: Bespoke letter-by-letter and line-by-line editorial reveals using GSAP SplitText and custom bezier timing functions (`CustomEase`).
- **Dynamic Circular Vector Emblem**: Mathematical SVG `<textPath>` with calibrated character-length spacing (`textLength="272"` / `181"`) rotating continuously in harmony with scroll velocity.
- **Self-Contained & Immutable**: All fonts (`Maison Neue Extended`, `Cormorant Garamond`), scripts, stylesheets, vectors, and ambient video loops are localized offline for maximum durability, zero CDN downtime risk, and sub-second load times.

---

## Project Structure

```
├── index.html              # Main landing page & interactive architectural experience
├── apartments/             # Dedicated residence catalogue & floor plan detail view
│   └── index.html
├── style.css               # Design tokens, typography rules & layout responsive grid
├── script.js               # Choreography engine (GSAP, Lenis, SplitText, CustomEase)
├── vendor/                 # Self-contained offline JavaScript and CSS libraries
│   ├── gsap.min.js
│   ├── ScrollTrigger.min.js
│   ├── SplitText.min.js
│   ├── CustomEase.min.js
│   ├── lenis.min.js
│   ├── lenis.css
│   ├── lottie.min.js
│   ├── swiper-bundle.min.js
│   ├── swiper-bundle.min.css
│   ├── barba.min.js
│   ├── jquery.min.js
│   └── webflow.js
├── assets/                 # Fully localized offline media assets
│   ├── branding/           # Vector emblem logos, favicon & typography assets
│   ├── fonts/              # Maison Neue Extended typography (woff2)
│   ├── images/             # Architectural renders, elevation drawings & photography
│   └── videos/             # Ambient looping video textures (bougainvillea & lightplay)
├── vercel.json             # Vercel deployment configuration (cleanUrls, cache headers)
└── package.json            # Node.js & Vite local development scripts
```

---

## Running Locally

### Option 1: Python HTTP Server (Zero Dependencies)
```bash
python -m http.server 3000
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Option 2: Vite Dev Server (Node.js)
```bash
npm install
npm run dev
```

---

## Deployment on Vercel

This repository is pre-configured with `vercel.json` including:
- `cleanUrls: true` for clean navigation (`/apartments` without `.html`)
- Long-term immutable caching headers for static assets (`/assets/*` and `/vendor/*`)

To deploy via Vercel CLI:
```bash
npm i -g vercel
vercel --prod
```

Or connect this GitHub repository directly to [Vercel](https://vercel.com) for automatic CI/CD preview and production deployments on every push.

---

## Contact & Inquiries

- **Sales Office**: Paseo de las Palmeras 18, 29688 New Golden Mile, Málaga, Spain
- **Phone**: [+91 76780 46520](tel:+917678046520) / [+91 79774 57097](tel:+917977457097)
