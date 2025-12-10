# Fimentum Website

Modern landing page for Fimentum Oy - funding advisory for Finnish startups and growth companies.

## Tech Stack

- **Framework:** Astro (Static Site Generation)
- **Styling:** Tailwind CSS v4
- **Language:** TypeScript
- **Deployment:** AWS Amplify

## Project Structure

```
/
├── docs/                    # Project documentation
│   ├── PLAN.md             # Implementation plan
│   ├── BRAND.md            # Brand strategy & positioning
│   └── DESIGN.md           # Visual design specs
├── public/
│   ├── logo.webp           # Original logo (dark, for light backgrounds)
│   ├── logo-white.webp     # White logo (for dark backgrounds)
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Header.astro    # Fixed nav with scroll behavior
│   │   ├── Hero.astro      # Dark gradient hero with stats
│   │   ├── Services.astro  # Service cards grid
│   │   ├── Stats.astro     # Track record & partners
│   │   ├── About.astro     # Founder bio section
│   │   ├── Process.astro   # How we work steps
│   │   ├── Contact.astro   # Contact form & info
│   │   ├── Footer.astro    # Footer with social links
│   │   └── Analytics.astro # Google Analytics 4
│   ├── layouts/
│   │   └── Layout.astro    # Base HTML layout
│   ├── pages/
│   │   └── index.astro     # Single-page landing
│   └── styles/
│       └── global.css      # Tailwind config & custom styles
├── amplify.yml             # AWS Amplify build config
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Development

```bash
# Install dependencies
pnpm install

# Start dev server (port 8801)
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview
```

## Environment Variables

Copy `.env.example` to `.env` and configure:

```
PUBLIC_GA_ID=G-XXXXXXXXXX  # Google Analytics 4 Measurement ID
```

## Deployment

The site is configured for AWS Amplify deployment via `amplify.yml`.

1. Connect repository to AWS Amplify
2. Add `PUBLIC_GA_ID` environment variable in Amplify console
3. Amplify auto-detects build settings from `amplify.yml`

## Brand Assets

- **Logo (dark):** `/public/logo.webp` - For light backgrounds
- **Logo (white):** `/public/logo-white.webp` - For dark backgrounds

See `/docs/BRAND.md` for brand guidelines and `/docs/DESIGN.md` for visual specifications.
