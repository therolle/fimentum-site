# Fimentum Site Implementation Plan

## Overview

Modern single-page landing site for Fimentum Oy - funding advisory for Finnish startups and growth companies.

**Tech Stack:** Astro + Tailwind v4 + TypeScript
**Deployment:** AWS Amplify
**Language:** English primary

---

## Site Architecture

### Single-Page Sections

1. **Hero** - Gradient background, headline, dual CTAs, trust stats
2. **Problem/Solution** - Pain points and Fimentum's value
3. **Services** - 4 service cards with icons
4. **Track Record** - Key metrics, funding source logos
5. **About** - Company + Tommi Pajala bio with photo
6. **Process** - 3-4 step visualization
7. **Contact** - Multiple CTAs (book call, email, phone)
8. **Footer** - Social links, legal, company info

---

## Components to Build

| Component | Description |
|-----------|-------------|
| `Hero.astro` | Gradient bg, headline, stats bar, dual CTAs |
| `Services.astro` | 4 service cards in grid |
| `Stats.astro` | Animated counters, partner logos |
| `About.astro` | Photo + bio section |
| `Process.astro` | Steps visualization |
| `Contact.astro` | Form + booking link + contact info |
| `Header.astro` | Sticky nav with scroll links |
| `Footer.astro` | Social links, legal |

---

## Content Needed

### Copy
- [ ] Hero headline and subheadline
- [ ] Problem/solution section
- [ ] 4 service descriptions
- [ ] About section (company + Tommi bio)
- [ ] 3-4 process steps
- [ ] CTA variations

### Assets
- [ ] Fimentum logo (from current site)
- [x] Tommi photo (LinkedIn)
- [ ] Partner logos (Business Finland, EU, Finnvera)
- [ ] Service icons (Heroicons)

---

## Interactive Features

- Smooth scroll navigation
- Animated stat counters on scroll
- Mobile menu toggle
- Calendly integration (or similar)
- Contact form (Formspree/Netlify Forms)

---

## Future Expansion

- Finnish language version
- Blog/resources section
- Case studies page
- Funding calculator tool
