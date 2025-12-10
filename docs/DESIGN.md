# Fimentum Visual Design Specifications

## Design Direction

**Style:** Tech-Forward Modern
- Clean with purposeful visual interest
- Gradient accents (modern SaaS aesthetic)
- Generous whitespace
- Strong typography hierarchy
- Dark/light section contrast

---

## Color Palette

### Primary Colors
```css
--primary-600: #4f46e5;     /* Indigo - primary actions */
--primary-700: #4338ca;     /* Indigo dark - hover states */
--primary-500: #6366f1;     /* Indigo light - accents */
```

### Accent Colors
```css
--accent-400: #22d3ee;      /* Cyan - highlights */
--accent-500: #06b6d4;      /* Cyan - CTAs */
--accent-600: #0891b2;      /* Cyan dark */
```

### Gradient
```css
--gradient-primary: linear-gradient(135deg, #4f46e5 0%, #7c3aed 50%, #06b6d4 100%);
--gradient-dark: linear-gradient(180deg, #0f172a 0%, #1e293b 100%);
```

### Neutrals
```css
--slate-50: #f8fafc;        /* Light backgrounds */
--slate-100: #f1f5f9;       /* Alternate sections */
--slate-600: #475569;       /* Body text */
--slate-800: #1e293b;       /* Headings */
--slate-900: #0f172a;       /* Dark sections */
```

### Semantic
```css
--success: #10b981;         /* Green - positive indicators */
--white: #ffffff;
```

---

## Typography

### Font Stack
```css
--font-sans: 'Inter', system-ui, -apple-system, sans-serif;
```

### Scale
| Element | Size | Weight | Line Height |
|---------|------|--------|-------------|
| Hero H1 | 4rem (64px) | 700 | 1.1 |
| H2 | 2.5rem (40px) | 700 | 1.2 |
| H3 | 1.5rem (24px) | 600 | 1.3 |
| Body | 1.125rem (18px) | 400 | 1.6 |
| Small | 0.875rem (14px) | 400 | 1.5 |

### Responsive
- Mobile H1: 2.5rem (40px)
- Mobile H2: 2rem (32px)
- Mobile body: 1rem (16px)

---

## Spacing

### Section Padding
- Desktop: py-24 (96px)
- Mobile: py-16 (64px)

### Container
- Max width: 1280px (max-w-7xl)
- Padding: px-4 sm:px-6 lg:px-8

### Component Spacing
- Card gap: gap-8 (32px)
- Text spacing: space-y-4 to space-y-6

---

## Components

### Buttons

**Primary CTA**
```css
bg-gradient-to-r from-indigo-600 to-cyan-500
text-white font-medium
px-8 py-4 rounded-xl
hover: shadow-lg shadow-indigo-500/25
transition-all duration-200
```

**Secondary CTA**
```css
border border-slate-300
bg-white text-slate-700
px-8 py-4 rounded-xl
hover: bg-slate-50 border-slate-400
```

### Cards

**Service Card**
```css
bg-white rounded-2xl
p-8 border border-slate-200
shadow-sm
hover: shadow-md border-indigo-200
transition-all duration-200
```

### Stats

**Stat Item**
```css
text-5xl font-bold
bg-gradient-to-r from-indigo-400 to-cyan-400
bg-clip-text text-transparent
```

---

## Section Styles

### Hero (Dark)
```css
bg-gradient-to-br from-slate-900 via-slate-800 to-indigo-900
text-white
min-h-screen or min-h-[80vh]
```

### Light Sections
```css
bg-white or bg-slate-50
text-slate-800 (headings)
text-slate-600 (body)
```

### Alternating Pattern
1. Hero - Dark gradient
2. Problem/Solution - White
3. Services - Slate-50
4. Stats - Dark gradient
5. About - White
6. Process - Slate-50
7. Contact - White
8. Footer - Slate-900

---

## Visual Elements

### Icons
- Source: Heroicons (outline style)
- Size: w-8 h-8 for service cards
- Color: Indigo-500 or gradient

### Images
- Tommi photo: rounded-2xl, subtle shadow
- Aspect ratio: maintain natural
- Treatment: slight desaturation for cohesion

### Logos
- Partner logos: grayscale, opacity-60
- Hover: full color, opacity-100
- Height: h-8 to h-12

### Decorative
- Subtle gradient orbs in hero
- Grid pattern overlay (optional)
- Gradient border accents

---

## Animations

### Scroll Animations
- Fade up on enter: opacity-0 -> opacity-100, translateY(20px) -> translateY(0)
- Duration: 600ms
- Easing: ease-out

### Stat Counters
- Count up animation on scroll into view
- Duration: 2000ms
- Easing: ease-out

### Hover States
- All interactive elements: transition-all duration-200
- Buttons: scale(1.02) on hover
- Cards: translateY(-4px) + shadow

### Navigation
- Smooth scroll: scroll-behavior: smooth
- Active section highlight in nav

---

## Responsive Breakpoints

```css
sm: 640px   /* Small tablets */
md: 768px   /* Tablets */
lg: 1024px  /* Small desktop */
xl: 1280px  /* Desktop */
```

### Mobile Considerations
- Stack columns on mobile
- Reduce padding/margins
- Smaller typography
- Full-width buttons
- Hamburger menu
