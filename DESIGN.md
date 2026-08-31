---
name: Kinetic Engineering
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c1c6d7'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8b90a0'
  outline-variant: '#414755'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e69'
  primary-container: '#4b8eff'
  on-primary-container: '#00285c'
  inverse-primary: '#005bc1'
  secondary: '#c0c1ff'
  on-secondary: '#1000a9'
  secondary-container: '#3131c0'
  on-secondary-container: '#b0b2ff'
  tertiary: '#ffb595'
  on-tertiary: '#571e00'
  tertiary-container: '#ef6719'
  on-tertiary-container: '#4c1a00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb595'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7c2e00'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  display-lg:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Geist
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0em
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '450'
    lineHeight: '1.5'
    letterSpacing: 0em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1280px
  gutter: 24px
  section-gap: 120px
  element-gap: 16px
---

## Brand & Style

The design system is built on a **Tech-Forward Minimalist** aesthetic, specifically tailored for a software engineering portfolio. The brand personality is precise, innovative, and highly professional, mirroring the quality of the code it showcases. It balances the rigor of engineering with the elegance of modern SaaS products.

The visual style utilizes a high-end **Glassmorphism** approach. It avoids heavy, solid containers in favor of translucent layers, subtle backdrop blurs, and "light-leak" border glows that suggest depth without clutter. The interface feels lightweight and fluid, emphasizing content through generous white space and rhythmic motion.

## Colors

The palette is optimized for a sophisticated dark mode experience. The primary colors utilize a gradient spectrum between **Electric Blue (#007AFF)** and **Indigo (#6366F1)** to represent energy and logic.

- **Primary:** Used for actionable elements, progress indicators, and syntax highlighting.
- **Surface:** Deep Navy and Slate tones provide a stable foundation.
- **Glass:** Semi-transparent layers use a subtle blur (20px+) to create a sense of physical layering.
- **Accents:** Use the secondary indigo for hover states and supplemental data visualizations to maintain a technical "dashboard" feel.

## Typography

This design system uses a triple-font stack to differentiate between high-level messaging, content, and technical data.

1. **Geist (Headlines):** Chosen for its geometric precision and technical "developer" aesthetic. Use tight letter-spacing for large displays.
2. **Inter (Body):** Ensures maximum readability for project descriptions and technical essays.
3. **JetBrains Mono (Labels/Code):** Specifically for technical tags, metadata, and code snippets, reinforcing the engineering context.

Headlines should be set in high contrast to body text (SemiBold or Bold) to establish a clear information hierarchy.

## Layout & Spacing

The layout follows a **Fluid Grid** model with a maximum container width of 1280px. 

- **Vertical Rhythm:** Large "section-gaps" (120px on desktop, 80px on mobile) ensure the portfolio feels premium and uncrowded.
- **Internal Spacing:** Use a base-8 scale (8px, 16px, 24px, 32px) for all internal component margins.
- **Adaptation:** On mobile devices, the 12-column desktop grid collapses to a 4-column layout. Horizontal margins should increase from 24px (tablet) to 48px (ultra-wide desktop) to maintain focus.

## Elevation & Depth

Depth is conveyed through **Backdrop Filtering** rather than traditional drop shadows.

- **Level 1 (Base):** Dark slate background.
- **Level 2 (Cards):** 70% opacity surface with a `backdrop-filter: blur(20px)`. Includes a 1px solid border at 10% white opacity.
- **Level 3 (Hover/Modals):** Increased brightness on the surface and a subtle "border-glow" effect using a linear gradient stroke that tracks with the mouse movement or stays fixed at the top-left corner.
- **Glows:** Use low-opacity radial gradients (Primary color at 5-10% opacity) positioned behind key sections to create an atmospheric, luminous environment.

## Shapes

The shape language is modern and approachable, utilizing a consistent **Rounded (0.5rem - 1.5rem)** logic.

- **Cards & Sections:** Use `rounded-xl` (1.5rem / 24px) to create a soft, friendly frame for technical content.
- **Buttons & Inputs:** Use `rounded-lg` (1rem / 16px) for a balanced, modern feel.
- **Tags/Chips:** Use pill-shapes (3rem) to contrast against the more structural card shapes.

## Components

- **Glass Navigation:** A fixed top bar with `backdrop-filter: blur(12px)`. Links should use a subtle underline animation that expands from the center on hover.
- **Project Cards:** Feature an "Entrance Animation" (Fade-in + Slide-up). On hover, the 1px border should transition from gray to the Primary Electric Blue, and the card should scale slightly (1.02x).
- **Code Snippets:** Stored in a rounded container with a custom scrollbar. Use a dark theme (one-dark or similar) that matches the primary/secondary accent colors.
- **Buttons:** 
  - **Primary:** Solid Electric Blue with a subtle white inner-glow on the top edge.
  - **Ghost:** 1px border-glow with no fill, becoming semi-transparent on hover.
- **Tech Stack Chips:** Small, monospaced text with a 5% white background and a 1px border. Include the technology's monochrome icon.
- **Interactive Timeline:** A vertical line for experience, using the primary blue for nodes. Nodes should "pulse" when in the viewport.