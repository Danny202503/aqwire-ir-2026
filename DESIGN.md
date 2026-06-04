---
name: Cinematic Sovereign
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c3c6d7'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8d90a0'
  outline-variant: '#434655'
  surface-tint: '#b4c5ff'
  primary: '#b4c5ff'
  on-primary: '#002a78'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#0053db'
  secondary: '#b9c8de'
  on-secondary: '#233143'
  secondary-container: '#39485a'
  on-secondary-container: '#a7b6cc'
  tertiary: '#ddb7ff'
  on-tertiary: '#490080'
  tertiary-container: '#943fe2'
  on-tertiary-container: '#faecff'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#d4e4fa'
  secondary-fixed-dim: '#b9c8de'
  on-secondary-fixed: '#0d1c2d'
  on-secondary-fixed-variant: '#39485a'
  tertiary-fixed: '#f0dbff'
  tertiary-fixed-dim: '#ddb7ff'
  on-tertiary-fixed: '#2c0051'
  on-tertiary-fixed-variant: '#6900b3'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
  emerald-success: '#10b981'
  rose-error: '#f43f5e'
  glass-surface: rgba(20, 25, 35, 0.6)
  glass-border: rgba(255, 255, 255, 0.08)
typography:
  display-hero:
    fontFamily: hankenGrotesk
    fontSize: 72px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: hankenGrotesk
    fontSize: 48px
    fontWeight: '900'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: hankenGrotesk
    fontSize: 32px
    fontWeight: '900'
    lineHeight: '1.2'
  card-title:
    fontFamily: hankenGrotesk
    fontSize: 20px
    fontWeight: '700'
    lineHeight: '1.4'
  body-main:
    fontFamily: hankenGrotesk
    fontSize: 18px
    fontWeight: '500'
    lineHeight: '1.6'
  label-caps:
    fontFamily: hankenGrotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.3em
  caption:
    fontFamily: hankenGrotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-margin: 1.5rem
  section-gap: 5rem
  card-gap: 1.5rem
  stack-sm: 0.5rem
  stack-md: 1rem
---

## Brand & Style

The design system is engineered for the high-stakes environment of Investor Relations, where clarity meets prestige. The brand personality is **Professional, Innovative, and Secure**, aiming to evoke a sense of "Command Center" authority. It positions the user as a sophisticated observer of real-time financial energy.

The aesthetic follows a **Cinematic Glassmorphism** style. It leverages deep, ink-black foundations to make financial data appear as if it is projected light. High-fidelity visual depth is achieved through translucent layers, soft-focus background blurs, and neon accents that simulate "live" data streams. The interface should feel like a premium physical device—tactile yet digital—combining the weight of institutional finance with the velocity of modern technology.

## Colors

The palette is optimized for OLED displays, utilizing a true-black background (`#050505`) to maximize contrast and energy efficiency. 

- **Primary (Electric Blue):** Used for interaction points, active states, and brand-identifying accents. It represents the "spark" of data.
- **Secondary (Slate):** Reserved for metadata and supporting text to maintain a clear hierarchy.
- **Status Colors:** Emerald is used exclusively for profit and success metrics, while Rose denotes costs, fees, or critical alerts.
- **Surface Strategy:** Layers are defined not by solid colors but by transparency. Use `glass-surface` for all container backgrounds to allow background mesh gradients to subtly bleed through, creating a sense of unified space.

## Typography

This design system uses **Hanken Grotesk** for its sharp, modern geometric qualities which mirror the "tech-forward" fintech aesthetic. 

- **Hierarchy:** High contrast in weight is essential. Use `900` weight for headlines to create an impactful, editorial feel.
- **Emphasis:** Key financial figures should use the `display-hero` or `headline-lg` styles. 
- **Labels:** Technical labels and overlines must always be in uppercase with heavy letter-spacing (`0.3em`) to enhance the "interface" look.
- **Gradients:** Apply a linear gradient (135deg, White to Slate) to large headings to simulate light reflecting off a metallic surface.

## Layout & Spacing

The layout is a **fluid-to-fixed** model optimized for mobile-first consumption but scaling gracefully for IR presentations. 

- **Grid:** On mobile, use a single-column layout with a 24px (`1.5rem`) margin. On larger presentation screens, allow content to span a 12-column grid within a max-width of 1600px.
- **Visual Rhythm:** Generous vertical spacing (`section-gap`) is used to separate distinct investment narratives, ensuring the user is not overwhelmed by data.
- **Safe Areas:** Adhere to strict device safe areas for mobile interactions, especially for floating glass navigation bars.

## Elevation & Depth

Hierarchy is established through "Optical Z-index" rather than simple shadows.

- **Layer 0 (Background):** Deep black with subtle, slow-moving radial mesh gradients in Blue and Emerald.
- **Layer 1 (Glass Panels):** `16px` backdrop-blur with a `1px` white border at 8% opacity. These panels should appear to float.
- **Layer 2 (Interaction):** Upon touch or focus, elements do not move "up"; instead, they emit a soft neon glow (outer shadow) in the primary accent color.
- **Motion:** Transitions use a `0.4s` cubic-bezier (Quart) for a weighted, luxury feel. Use parallax effects on the glass panels to create a 3D perspective during scroll.

## Shapes

The shape language combines structural stability with organic tech cues. 

- **Main Containers:** Use `rounded-xl` (24px) for all primary glass panels to soften the technical edge.
- **Interactive Elements:** Buttons and badges use the "Pill" shape (full roundedness) to signify they are interactive "objects" within the interface.
- **Internal Elements:** Nested inputs or smaller cards use `rounded-lg` (12px) to maintain visual nesting logic.
- **Borders:** Use hairline `1px` borders consistently to maintain a crisp, high-definition appearance.

## Components

- **Glass Buttons:** Full-pill shape. Primary buttons use a solid Electric Blue fill with a subtle inner glow. Secondary buttons use a transparent fill with a glass-border and backdrop-blur.
- **Data Cards:** These are the core units. Each card must have a `1px` hairline border and `16px` backdrop-blur. The title should be in `label-caps` at the top.
- **Neon Viz:** Data visualizations (charts, pipelines) should use glowing lines instead of solid fills. Use CSS filters to add a `blur(4px)` glow to active data paths.
- **Status Chips:** Small, pill-shaped labels with a 20% opacity background of the status color (Emerald/Rose) and 100% opacity text for high legibility.
- **Energy Pipeline:** A custom component representing data flow. Use a linear gradient animation that moves across a pill-shaped track to simulate "live" liquidity or investor interest.
- **Input Fields:** Minimalist. Only a bottom border or a very subtle glass-filled container. Focus state triggers a primary blue glow.