---
name: Clinical Clarity
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#464554'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#767586'
  outline-variant: '#c7c4d7'
  surface-tint: '#494bd6'
  primary: '#4648d4'
  on-primary: '#ffffff'
  primary-container: '#6063ee'
  on-primary-container: '#fffbff'
  inverse-primary: '#c0c1ff'
  secondary: '#006591'
  on-secondary: '#ffffff'
  secondary-container: '#39b8fd'
  on-secondary-container: '#004666'
  tertiary: '#8127cf'
  on-tertiary: '#ffffff'
  tertiary-container: '#9c48ea'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#07006c'
  on-primary-fixed-variant: '#2f2ebe'
  secondary-fixed: '#c9e6ff'
  secondary-fixed-dim: '#89ceff'
  on-secondary-fixed: '#001e2f'
  on-secondary-fixed-variant: '#004c6e'
  tertiary-fixed: '#f0dbff'
  tertiary-fixed-dim: '#ddb7ff'
  on-tertiary-fixed: '#2c0051'
  on-tertiary-fixed-variant: '#6900b3'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 30px
    fontWeight: '600'
    lineHeight: '1.3'
  title-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  arabic-body:
    fontFamily: Tajawal
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.8'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  container-max: 1440px
  gutter: 24px
---

## Brand & Style

This design system centers on a "Clinical Clarity" aesthetic, specifically tailored for a high-end pediatric SaaS. The brand personality is authoritative yet empathetic, replacing typical pediatric whimsy with professional sophistication. The target audience—healthcare providers and discerning parents—requires a UI that evokes trust, precision, and calm.

The style is a hybrid of **Minimalism** and **Glassmorphism**. It utilizes heavy whitespace to reduce cognitive load and integrates subtle, translucent layers to create a sense of lightness. By avoiding cartoon mascots in favor of high-quality iconography and soft abstract organic shapes, the design system maintains a premium, scientific feel that respects the importance of developmental data.

## Colors

The palette is anchored in a pristine "Medical White" and "Soft Slate" base to ensure the interface feels sterile but inviting. The primary identity is driven by a sophisticated gradient transition from **Indigo Blue** to **Deep Purple**, symbolizing growth and intelligence.

- **Primary:** A vibrant Purple-Blue used for calls to action and progress indicators.
- **Secondary:** A calming Sky Blue used for informational accents and supportive UI elements.
- **Neutral:** A range of cool grays (Slate) to define hierarchy without introducing visual noise.
- **Accent:** Soft lavender tints are used for background washes to differentiate sections.

## Typography

The typography system is dual-language optimized for RTL (Arabic) and LTR (English) contexts. **Plus Jakarta Sans** provides a modern, slightly rounded geometric feel for English text, echoing the softness of pediatric care while maintaining high legibility. For Arabic, **Tajawal** is utilized for its clean, low-contrast strokes that harmonize perfectly with the Latin weights.

Hierarchies are established through weight rather than just size. Headlines use a Bold weight with tighter letter spacing, while body text uses a Regular weight with generous line height (1.6x-1.8x) to ensure readability of medical terminology and data.

## Layout & Spacing

The design system employs a **Fixed Grid** model for desktop (12 columns) and a **Fluid Grid** for mobile. The layout is strictly RTL-first, ensuring that the visual "weight" starts from the right. A 8px base unit drives all spacing decisions, creating a rhythmic and predictable flow.

Margins are intentionally generous (48px+) to create a "Premium Light" feel, allowing data-heavy growth charts and clinical tables to "breathe." Sections are separated by soft whitespace rather than harsh dividing lines.

## Elevation & Depth

Depth is conveyed through **Glassmorphism** and **Ambient Shadows**. Instead of traditional solid cards, top-level containers use a semi-transparent white background (`rgba(255, 255, 255, 0.7)`) with a high-saturation `backdrop-filter: blur(20px)`.

Shadows are extremely diffused and tinted with the primary purple-blue hue to avoid "dirty" gray aesthetics. 
- **Level 1 (Base):** Flat or subtle 1px border (#E2E8F0).
- **Level 2 (Cards):** 20px blur, 4% opacity indigo shadow.
- **Level 3 (Modals/Popovers):** 40px blur, 8% opacity indigo shadow, often combined with a thin white inner-border to simulate glass thickness.

## Shapes

The shape language is "Rounded Professional." Rectilinear elements are softened to appear approachable, but not so circular as to appear juvenile. 

Standard components (Cards, Inputs) use a **16px (1rem)** radius. Smaller components like chips or tags use a **pill-shape** to provide a visual contrast against the structured grid. Abstract background shapes should use organic, "blob" geometry with low-opacity gradients to add depth without distracting from the data.

## Components

### Buttons
Primary buttons use the Indigo-to-Purple gradient with white text and a soft shadow that expands on hover. Secondary buttons use a "Glass" style: white semi-transparent background with a thin purple border.

### Cards
Cards are the primary container. They must feature a `backdrop-filter: blur` and a 1px white border at 50% opacity to define the "Glass" edge. They should never have a heavy stroke.

### Input Fields
Inputs are minimal: a light gray background (#F1F5F9) that transitions to a white background with an indigo border glow on focus. Labels are always positioned above the field, right-aligned for Arabic.

### Growth Charts
Charts should use the primary gradient for the "Main Growth Curve" and soft gray for "Percentile Ranges." Data points should be represented by soft glowing circles rather than sharp dots.

### Abstract Icons
Avoid literal medical icons where possible. Use "Line-and-Dot" icons that suggest connectivity and growth. All icons should have a consistent 2px stroke width with rounded caps.