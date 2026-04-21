# Golden Corner Printing Press LLC — Website

> Premium corporate website for **Golden Corner Printing Press LLC**, Abu Dhabi, UAE.  
> Established 1999 · +971 2 658 7770

---

## Overview

A fully responsive, single-page business website built with clean HTML5, CSS3, and vanilla JavaScript.  
Designed with a dark + gold colour scheme to reflect the premium, corporate identity of the brand.

---

## Project Structure

```
golden-corner/
├── index.html          # Main HTML — all sections, markup, and page structure
├── css/
│   └── style.css       # All styles: variables, layout, components, animations, responsive
├── js/
│   └── main.js         # All interactions: nav scroll, mobile drawer, fade-in, form, tabs
├── assets/             # Place images, icons, and brand assets here
│   └── (empty — add logo.svg, favicon.ico, portfolio images here)
└── README.md           # This file
```

---

## Pages / Sections

| Section        | ID                | Description                                      |
|----------------|-------------------|--------------------------------------------------|
| Hero           | `#home`           | Full-screen headline, stats, dual CTA buttons    |
| Marquee        | —                 | Animated gold ticker of services                 |
| About          | `#about`          | Company story, pillars, 25-year badge            |
| Services       | `#services`       | 6-card grid: Digital, Offset, Screen, Design … |
| Why Choose Us  | `#why`            | 5 differentiating reasons                        |
| Portfolio      | `#portfolio`      | Filterable 6-item project showcase               |
| Testimonials   | `#testimonials`   | 3 corporate client reviews                       |
| CTA Banner     | —                 | Mid-page conversion strip                        |
| Contact        | `#contact`        | Quote form + contact info + map                  |
| Footer         | —                 | Links, brand, legal                              |

---

## Design System

### Colour Palette

| Token          | Hex       | Usage                              |
|----------------|-----------|------------------------------------|
| `--gold`       | `#C9A84C` | Primary accent, CTAs, highlights   |
| `--gold-light` | `#E8C97A` | Hover states                       |
| `--gold-dark`  | `#8B6914` | Deep gold, gradients, scrollbar    |
| `--black`      | `#0A0A0A` | Page background                    |
| `--charcoal`   | `#141414` | Section alternate background       |
| `--dark`       | `#1C1C1C` | Cards, inputs                      |
| `--white`      | `#FAFAF8` | Body text                          |

### Typography

| Family                | Role         |
|-----------------------|--------------|
| Cormorant Garamond    | Headings (h1–h4), display text, logo |
| DM Sans               | Body, navigation, labels, buttons    |

Both loaded via Google Fonts.

---

## Features

- ✅ Sticky navigation with scroll-triggered frosted glass effect
- ✅ Mobile hamburger drawer navigation
- ✅ Hero section with staggered CSS animation (fadeUp)
- ✅ Animated gold marquee ticker bar
- ✅ Scroll-triggered fade-in for all sections (IntersectionObserver)
- ✅ Interactive service cards with hover underline reveal
- ✅ Portfolio filter tabs (UI only — extend with JS filtering as needed)
- ✅ Testimonials grid
- ✅ Quote request form with success state
- ✅ WhatsApp floating button with pulse animation
- ✅ Smooth anchor scroll with nav offset
- ✅ Fully responsive: 1200px → 1024px → 900px → 768px → 480px
- ✅ SEO meta tags + Open Graph
- ✅ Accessible: ARIA labels, semantic HTML, `for`/`id` form pairs

---

## Getting Started

No build tools required. Open `index.html` directly in a browser, or serve with any static host.

```bash
# Option 1 — Open directly
open index.html

# Option 2 — Local dev server (Node)
npx serve .

# Option 3 — Python simple server
python3 -m http.server 8080
```

---

## Customisation Guide

### Update contact details
Edit `index.html` — search for `+97126587770` and `wa.me/97126587770`  
Update phone number, WhatsApp link, email, and address as needed.

### Add a real logo
Place `logo.svg` (or `logo.png`) in `assets/` and replace the `.nav-logo-mark` GC block in `index.html`.

### Add a favicon
Place `favicon.ico` in the root and add to `<head>`:
```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```

### Embed a real Google Map
Replace the `.map-embed` placeholder div in `index.html` with:
```html
<iframe
  src="https://www.google.com/maps/embed?pb=YOUR_EMBED_URL"
  width="100%" height="220" style="border:0;" allowfullscreen loading="lazy">
</iframe>
```

### Add portfolio images
Replace the CSS mockup divs inside `.portfolio-item` with real `<img>` tags  
pointing to files in `assets/portfolio/`.

### Connect the quote form
The form currently shows a success state on submit.  
To send real emails, wire up to [Formspree](https://formspree.io),  
[EmailJS](https://www.emailjs.com), or your own backend endpoint.

---

## Browser Support

| Browser         | Support |
|-----------------|---------|
| Chrome 90+      | ✅      |
| Firefox 88+     | ✅      |
| Safari 14+      | ✅      |
| Edge 90+        | ✅      |
| IE 11           | ❌      |

---

## Deployment

Deploy to any static hosting provider:

- **Netlify** — drag & drop the folder or connect Git repo
- **GitHub Pages** — push to `gh-pages` branch
- **Vercel** — `vercel --prod`
- **cPanel / FTP** — upload all files maintaining the folder structure

---

## Contact

**Golden Corner Printing Press LLC**  
Abu Dhabi, United Arab Emirates  
📞 +971 2 658 7770  
💬 [WhatsApp](https://wa.me/97126587770)  
🗓 Sun – Thu: 8:00 AM – 6:00 PM
