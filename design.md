---
name: ProDashboard Light
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e8eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#5c3f3e'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#916f6d'
  outline-variant: '#e6bdba'
  surface-tint: '#be0525'
  primary: '#bb0023'
  on-primary: '#ffffff'
  primary-container: '#e22336'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb3b0'
  secondary: '#5d5e61'
  on-secondary: '#ffffff'
  secondary-container: '#e0dfe3'
  on-secondary-container: '#616265'
  tertiary: '#595c5f'
  on-tertiary: '#ffffff'
  tertiary-container: '#727578'
  on-tertiary-container: '#fcfcff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad8'
  primary-fixed-dim: '#ffb3b0'
  on-primary-fixed: '#410006'
  on-primary-fixed-variant: '#930019'
  secondary-fixed: '#e2e2e5'
  secondary-fixed-dim: '#c6c6c9'
  on-secondary-fixed: '#1a1c1e'
  on-secondary-fixed-variant: '#45474a'
  tertiary-fixed: '#e1e2e6'
  tertiary-fixed-dim: '#c4c7ca'
  on-tertiary-fixed: '#191c1f'
  on-tertiary-fixed-variant: '#44474a'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 28px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  stack-gap: 0.75rem
  container-padding: 1rem
  element-padding: 1.25rem
  grid-gutter: 1rem
---

## Brand & Style

The brand identity is approachable, professional, and optimistic, specifically tailored for young entrepreneurs and small business owners. It utilizes a **Corporate Modern** aesthetic with a subtle "soft-touch" feel to reduce the friction of complex data management.

The design emphasizes high clarity and friendly interactions. It balances the utility of a SaaS product with the warmth of a consumer-facing app, utilizing soft pastel backgrounds, vibrant primary accents, and smooth micro-interactions to create an environment that feels organized yet inviting.

## Colors

The palette is built on a "Fidelity" variant of a deep crimson red, used strategically for primary actions and active states. 

- **Primary & Containers:** The primary red (#bb0023) is used for high-impact elements like the Floating Action Button (FAB) and active navigation states. `primary-container` provides a softer background for these elements.
- **Surfaces:** The system uses a blue-tinted neutral scale for surfaces (starting at #f9f9ff) to keep the interface feeling fresh and clean rather than sterile grey.
- **Support Colors:** Secondary and tertiary tones are kept as neutral desaturated greys to ensure that the red primary color remains the focal point for all critical user pathways.

## Typography

The system exclusively uses **Plus Jakarta Sans**, a modern geometric sans-serif with a friendly, open aperture. 

- **Headlines:** Use Bold (700) or SemiBold (600) weights. Mobile headlines are scaled down by ~15% to maintain a comfortable reading rhythm.
- **Body:** Standard body text is kept at 14px or 16px to ensure high legibility against the light background.
- **Labels:** Small labels use a slightly increased letter spacing (0.02em) and SemiBold weight to remain legible at 12px.

## Layout & Spacing

The layout utilizes a **Fixed Grid** approach for larger screens (max-width: 2xl) and a **Fluid Grid** for mobile devices.

- **Grid Logic:** A 2-column or 3-column "Bento" grid is used for dashboard navigation.
- **Vertical Rhythm:** A base unit of 4px is used, with most components utilizing `0.75rem` (12px) or `1rem` (16px) for spacing.
- **Mobile Adjustments:** Side margins are locked to `1rem` (16px) on mobile, with a top header padding of `1.25rem` to accommodate status bars and system UI.

## Elevation & Depth

Visual hierarchy is established through a combination of **Tonal Layering** and **Ambient Shadows**.

- **Shadows:** Use a very soft, low-opacity shadow (`rgba(0, 0, 0, 0.04)`) for base cards to suggest depth without creating clutter.
- **Interaction Depth:** Buttons and active cards utilize a `scale-95` transform on click to provide tactile feedback.
- **App Bar:** The top bar uses a `backdrop-blur-md` with 80% opacity to maintain context of the content scrolling beneath it while remaining elevated.
- **Borders:** Subtle `outline-variant` borders at 30% opacity are used on white cards to define edges against the slightly-blue surface background.

## Shapes

The design follows a **Rounded** shape language, leaning towards a "squishy" and friendly aesthetic.

- **Standard Cards:** Use `rounded-xl` (0.75rem) to soften the layout.
- **Selection Pills:** Segmented controls and buttons use `rounded-lg` (0.5rem) to distinguish them from larger containers.
- **Avatars & Icons:** Circular elements are strictly `rounded-full`.
- **Primary Action (FAB):** Uses a specific `rounded-2xl` for a more prominent, "chunky" physical appearance.

## Components

- **Buttons:** Primary buttons use the `primary` red background with `on-primary` white text. Active states include a `shadow-sm`.
- **Cards (Bento Style):** Centered icons with labels below. Use a background of `surface-container-lowest` (pure white) with a soft shadow and subtle border.
- **Segmented Control:** A container of `secondary-container/50` holding `rounded-lg` buttons. The active state is indicated by a full background color swap (Red) rather than just a tint.
- **Bottom Navigation:** Fixed to the bottom with an extra `pb-6` for safe area compliance. The center element is an offset FAB.
- **Analytics Charts:** Simple bar charts using `primary/20` for historical data and solid `primary` for the current/highlighted data point.
- **Icons:** Use **Material Symbols Outlined** with a weight of 400 and optical size of 24.