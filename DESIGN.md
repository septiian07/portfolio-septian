---
name: Ethereal Monolith
colors:
  surface: '#141313'
  surface-dim: '#141313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2b2a2a'
  surface-container-highest: '#353434'
  on-surface: '#e5e2e1'
  on-surface-variant: '#c4c7c7'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c9c6c5'
  primary: '#c9c6c5'
  on-primary: '#313030'
  primary-container: '#0a0a0a'
  on-primary-container: '#7b7979'
  inverse-primary: '#5f5e5e'
  secondary: '#c6c6cf'
  on-secondary: '#2f3037'
  secondary-container: '#45464e'
  on-secondary-container: '#b4b4bd'
  tertiary: '#cac6c3'
  on-tertiary: '#32302f'
  tertiary-container: '#0b0a09'
  on-tertiary-container: '#7c7977'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c9c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#e2e1eb'
  secondary-fixed-dim: '#c6c6cf'
  on-secondary-fixed: '#1a1b22'
  on-secondary-fixed-variant: '#45464e'
  tertiary-fixed: '#e6e1df'
  tertiary-fixed-dim: '#cac6c3'
  on-tertiary-fixed: '#1d1b1a'
  on-tertiary-fixed-variant: '#484645'
  background: '#141313'
  on-background: '#e5e2e1'
  surface-variant: '#353434'
typography:
  headline-xl:
    fontFamily: Playfair Display
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.8'
    letterSpacing: 0.01em
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  section-gap: 160px
  element-gap: 32px
  margin-safe: 5vw
  max-width: 1100px
---

## Brand & Style
The design system is anchored in a "Philosophical Minimalist" aesthetic, specifically tailored for a software engineer who views code as craft. The atmosphere is quiet, deep, and intentional. It utilizes a dark, monochromatic foundation to allow technical content and high-level thinking to breathe.

The style avoids the "gamer" or "cyberpunk" tropes often associated with dark themes, instead opting for a sophisticated, editorial feel. It relies on extreme negative space, typographic hierarchy, and a single ethereal accent to guide the eye. Interactions are characterized by slow, graceful fades and subtle opacity shifts rather than mechanical movements.

## Colors
The palette is intentionally restricted to maintain a focus on content. The primary background (#0a0a0a) provides a "void" that gives weight to the elements placed upon it. 

- **Primary:** The deep black background creates a canvas of infinite depth.
- **Secondary:** A soft slate gray used for long-form reading to reduce eye strain and establish a hierarchy below the pure white headings.
- **Accent:** An ethereal indigo-to-violet gradient used only for high-impact moments—such as active states, scroll indicators, or code category markers.
- **Contrast:** Pure white is reserved strictly for headings and critical UI triggers, ensuring maximum legibility against the dark void.

## Typography
The typography strategy pairs editorial elegance with technical precision. **Playfair Display** provides a sophisticated, human touch to headings, suggesting a deeper narrative behind the code. **Inter** handles the body copy with a generous line-height (1.8) to ensure readability in a dark environment.

**Geist** is used sparingly for labels, metadata, and code snippets, grounding the system in the engineer's technical reality. Scale typography aggressively; headers should feel like statements, while body text feels like a quiet conversation.

## Layout & Spacing
The layout follows a "No-Grid" philosophy that prioritizes vertical rhythm and safe margins over rigid columns. 

- **Verticality:** Use massive gaps (160px+) between major sections to signal a transition in thought.
- **Center-Aligned Focus:** Content should often be centered with significant horizontal margins to create a focused, "monolithic" reading experience.
- **Responsive Adaptivity:** On mobile, margins reduce to 24px, and typography scales down, but the vertical "breathing room" must be preserved to maintain the brand's philosophical tone.

## Elevation & Depth
This design system rejects traditional drop shadows. Depth is achieved through **Tonal Layers** and **Luminance**.

1.  **Level 0 (Base):** The primary #0a0a0a background.
2.  **Level 1 (Surface):** A subtle shift to #141414 for cards or containers, with no border.
3.  **Luminous Depth:** Use the accent gradient as a "glow" behind certain elements (blur radius 100px+, low opacity) to create an ethereal, floating effect rather than a physical shadow.
4.  **Glassmorphism:** For navigation bars or floating menus, use a 12px backdrop-blur with a 5% white tint to maintain context of the content underneath.

## Shapes
Shapes are disciplined and architectural. A subtle "Soft" (0.25rem) radius is applied to standard UI components like inputs and buttons to prevent the interface from feeling sharp or aggressive. Large containers (like project cards) should remain "Sharp" (0px) to mimic the look of high-end editorial layouts or physical art gallery plinths.

## Components

- **Buttons:** Primary buttons use the accent gradient as a background with white text. Secondary buttons are text-only with a white underline that expands from the center on hover.
- **Input Fields:** Minimalist "bottom-border only" style. The border glows with a 1px accent gradient line when focused.
- **Cards:** No borders or shadows. Cards are defined by a slightly lighter background color (#141414). On hover, the opacity of the card increases from 0.8 to 1.0.
- **Chips/Tags:** Small, Geist-font labels with a 1px slate-gray border and high letter spacing.
- **Micro-interactions:** All state changes (hover, focus, transition) must use a minimum 400ms "ease-in-out" curve. Rapid snapping is prohibited; elements should feel like they are emerging from or receding into the darkness.
- **Progress Indicators:** Use thin (2px) lines with the accent gradient, appearing only at the very top of the viewport or within the specific component context.