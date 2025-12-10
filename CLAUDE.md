# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
pnpm dev      # Start dev server at localhost:8801
pnpm build    # Build for production to ./dist/
pnpm preview  # Preview production build locally
```

## Architecture

Single-page Astro landing site for Fimentum Oy (funding advisory).

### Stack
- **Astro 5** - Static site generation
- **Tailwind CSS v4** - Uses `@tailwindcss/vite` plugin (not PostCSS)
- **TypeScript** - Strict mode via `astro/tsconfigs/strict`
- **Node 22+** required

### Tailwind v4 Configuration
Tailwind v4 uses CSS-first configuration in `src/styles/global.css`:
- Custom colors defined via `@theme { }` block
- Custom utility classes (`.gradient-text`, `.btn-gradient`, `.gradient-hero`)
- No `tailwind.config.js` file - everything in CSS

### Page Structure
Single page (`src/pages/index.astro`) composed of section components:
```
Layout → Header → Hero → Services → Stats → About → Process → Contact → Footer
```

Each section is a standalone Astro component in `src/components/`.

### Logo Assets
- `/public/logo.webp` - Original dark logo (light backgrounds)
- `/public/logo-white.webp` - White logo (dark backgrounds)

### Environment Variables
- `PUBLIC_GA_ID` - Google Analytics 4 measurement ID (only loads in production)

### Deployment
AWS Amplify via `amplify.yml`. Uses corepack to enable pnpm.

## Documentation
- `/docs/PLAN.md` - Implementation plan
- `/docs/BRAND.md` - Brand strategy, positioning, tone of voice
- `/docs/DESIGN.md` - Visual specs, colors, typography
