# RK Tile & Stone — Website Documentation

A fully responsive single-page website for **RK Tile & Stone Installation Company**, a UK-based tile and stone installation business.

**Live Site:** https://kevm-dev.github.io/rk-tile-stone/  
**Repository:** https://github.com/KevM-dev/rk-tile-stone  
**Designed by:** KevinM-Agency

---

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling, animations, responsive layout |
| Vanilla JavaScript | Slider, filtering, form, scroll behaviour |
| Google Fonts | Dancing Script (hero text), Montserrat (body) |
| Font Awesome 6 | Icons throughout the site |

No frameworks or build tools required — the entire site runs from a single `index.html` file.

---

## Site Structure

### 1. Header / Navigation
- Fixed to the top of the page on scroll
- Left: RK diamond logo (built with inline SVG, no image file needed)
- Right: Nav links — Home, Services, Projects, Contact Us
- Active link highlights as the user scrolls through sections
- Collapses into a hamburger menu on mobile

### 2. Hero Slideshow
- Full-screen 3-slide image carousel
- Auto-advances every 5 seconds with a smooth fade transition
- Diamond-shaped navigation dots on the right side for manual control
- Overlay text: *"Spaces Refined. Lives Transformed."* in Dancing Script font
- CTA button linking to the Services section

### 3. About Strip
- Dark background band displaying 3 key stats:
  - 12+ Years Experience
  - 500+ Projects Done
  - 100% Satisfied Clients

### 4. Services
- 6 service cards in a responsive grid:
  - Residential Tile Installation
  - Commercial Flooring
  - Stone & Marble Work
  - Bathroom Remodeling
  - Custom Mosaic & Patterns
  - Repair & Restoration
- Each card has a diamond-shaped icon, hover lift effect, and red bottom border on hover

### 5. Projects Gallery
- Filterable grid with 4 categories: All, Residential, Commercial, Bathroom
- Hover reveals a red gradient overlay with the project name and category
- Images scale slightly on hover for a polished feel

### 6. Why Choose Us
- 3-point checklist highlighting the company's strengths:
  - Premium Materials
  - On-Time Completion
  - Free Consultation
- Diamond-shaped red check icons matching the brand style

### 7. Contact Section
- Dark background for contrast
- **Left side — contact info (all clickable):**
  - Phone → opens dialler (`tel:`)
  - WhatsApp → opens WhatsApp chat (`wa.me`)
  - Email → opens mail app (`mailto:`)
  - Location: London, United Kingdom
- **Right side — enquiry form:**
  - Name, Email, Phone, Service needed, Message
  - Submit triggers a confirmation alert

### 8. Footer
- Logo (repeated from header)
- Social media icons: Facebook, Instagram, WhatsApp
- Copyright notice: Non Copyrighted © 2026
- Design credit: *Designed by KevinM-Agency*

---

## Design System

| Element | Value |
|---|---|
| Primary Red | `#C41E3A` |
| Dark / Black | `#111111` |
| Background Light | `#f8f6f3` |
| White | `#ffffff` |
| Body Font | Montserrat (400, 600, 700) |
| Hero Font | Dancing Script (700) |
| Brand Shape | Rotated diamond (45°) — used in logo, icons, dots, buttons |

---

## Responsive Behaviour

| Breakpoint | Behaviour |
|---|---|
| Desktop (>900px) | Full two-column layouts, all sections visible |
| Tablet (680–900px) | Why Us image hidden, Contact stacks to single column |
| Mobile (<680px) | Hamburger nav, single column form, footer stacks vertically |

---

## File Structure

```
rk-tile-stone/
└── index.html      # Entire site — HTML, CSS, and JS in one file
└── README.md       # This document
```

---

## How to Edit

### Change contact details
Search for `07700 900000` and replace with the real phone number.  
Search for `info@rktileandstone.co.uk` and replace with the real email.

### Change social media links
Find the footer social `<a href="#">` tags and replace `#` with the actual profile URLs.

### Change hero images
Find `.slide:nth-child(1)`, `.slide:nth-child(2)`, `.slide:nth-child(3)` in the CSS and update the `background-image` URLs.

### Add/remove services
Copy or delete a `<div class="service-card">` block inside the `#services` section.

### Add/remove projects
Copy or delete a `<div class="project-card">` block inside `#projectsGrid`. Set `data-cat` to `residential`, `commercial`, or `bathroom`.

---

## Deployment

The site is deployed via **GitHub Pages** on the `master` branch.  
Any `git push` to `master` automatically updates the live site within ~1 minute.
