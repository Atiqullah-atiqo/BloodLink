---
name: Blood Link Design System
colors:
  surface: '#fff8f7'
  surface-dim: '#f1d3d0'
  surface-bright: '#fff8f7'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fff0ef'
  surface-container: '#ffe9e7'
  surface-container-high: '#ffe2de'
  surface-container-highest: '#f9dcd9'
  on-surface: '#271816'
  on-surface-variant: '#5b403d'
  inverse-surface: '#3e2c2a'
  inverse-on-surface: '#ffedeb'
  outline: '#8f6f6c'
  outline-variant: '#e4beba'
  surface-tint: '#ba1a20'
  primary: '#af101a'
  on-primary: '#ffffff'
  primary-container: '#d32f2f'
  on-primary-container: '#fff2f0'
  inverse-primary: '#ffb3ac'
  secondary: '#5d5f5f'
  on-secondary: '#ffffff'
  secondary-container: '#dfe0e0'
  on-secondary-container: '#616363'
  tertiary: '#af1321'
  on-tertiary: '#ffffff'
  tertiary-container: '#d23136'
  on-tertiary-container: '#fff2f1'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad6'
  primary-fixed-dim: '#ffb3ac'
  on-primary-fixed: '#410003'
  on-primary-fixed-variant: '#930010'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#ffdad7'
  tertiary-fixed-dim: '#ffb3ae'
  on-tertiary-fixed: '#410004'
  on-tertiary-fixed-variant: '#930015'
  background: '#fff8f7'
  on-background: '#271816'
  surface-variant: '#f9dcd9'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 57px
    fontWeight: '700'
    lineHeight: 64px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  title-lg:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: '500'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.1px
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.5px
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
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

The design system is engineered for a critical healthcare environment where trust, urgency, and precision coexist. The brand personality is "Clinical Excellence meets Human Compassion." It utilizes a **Modern Corporate** aesthetic with a heavy emphasis on **Material 3 (M3)** principles—focusing on color-driven states and expressive containment.

The visual direction balances the high-stakes nature of blood donation and distribution with a calming, structured interface. By utilizing deep medical reds against expansive white space, the UI evokes a sense of professional authority. The experience is designed to be high-trust for medical professionals while remaining approachable and non-intimidating for donors.

## Colors

The palette is anchored by "Deep Medical Red," providing an immediate mental link to healthcare. 

- **Primary (#D32F2F):** Used for core actions, branding, and critical status indicators.
- **Secondary (#FFFFFF):** Acts as the primary canvas, ensuring a "clean room" aesthetic that minimizes cognitive load.
- **Accent/Tertiary (#FF5252):** A vibrant red used for high-energy call-to-actions and interactive elements that require immediate attention without the "error" connotation.
- **Gradients:** Use linear gradients (top-left to bottom-right) moving from `#D32F2F` to `#FF5252` for premium surfaces like hero cards and progress indicators.

**Color Modes:** 
- In **Light Mode**, use high-contrast text (Near Black) on white surfaces.
- In **Dark Mode**, shift the primary red to a slightly desaturated version to pass AA accessibility standards against `#121212`. Use tonal overlays for surface elevation rather than pure black.

## Typography

This design system utilizes **Inter** for its exceptional legibility in data-heavy healthcare contexts. The type scale follows a strict hierarchical progression:

1.  **Headlines:** Bold and authoritative. Use `headline-lg` for screen titles.
2.  **Body:** Optimized for reading medical instructions. `body-lg` is the default for patient or donor information.
3.  **Labels:** Used for buttons and metadata. `label-lg` is always semi-bold to ensure clarity on interactive targets.
4.  **Mobile Scaling:** On devices smaller than 600px, headlines should automatically scale down to their `-mobile` variants to maintain optimal line-wrapping.

## Layout & Spacing

The design system employs a **Fluid Grid** model based on an 8px spacing rhythm. 

- **Mobile (0-599px):** 4-column grid, 16px margins, 16px gutters.
- **Tablet (600-1023px):** 8-column grid, 24px margins, 16px gutters.
- **Desktop (1024px+):** 12-column grid, max-width 1200px, 24px gutters.

Large touch targets are a priority; all interactive elements must maintain a minimum height of 48px. Use `lg` (24px) spacing between unrelated content groups and `md` (16px) for related items within a card.

## Elevation & Depth

Hierarchy is established through **Ambient Shadows** and **Tonal Layers**, following Material 3's elevation system:

- **Level 0 (Flat):** The main background.
- **Level 1 (Default Card):** A subtle shadow (0px 1px 3px rgba(0,0,0,0.1)) or a slightly tinted surface color.
- **Level 2 (Active/Hover):** A more pronounced shadow (0px 4px 8px rgba(0,0,0,0.12)).
- **Level 3 (Modals/Overlays):** High-diffusion shadows (0px 8px 24px rgba(0,0,0,0.15)) to create a distinct physical separation from the content below.

In Dark Mode, elevation is communicated via "Surface Tint" overlays—higher elevation elements receive a higher percentage of the primary color mixed into the surface.

## Shapes

The shape language is purposefully **Rounded** to reduce the "cold" feeling of medical apps. 

- **Containers/Cards:** 16px (`rounded-lg`) is the standard corner radius for primary content containers.
- **Buttons:** Fully rounded (pill-shaped) for primary actions to distinguish them from information blocks.
- **Input Fields:** 12px corner radius to maintain a modern, friendly appearance while remaining structured.
- **Chips:** 8px corner radius for high density.

## Components

### Buttons
- **Primary:** Filled with the Primary Red or the Primary-to-Accent gradient. Use White text.
- **Secondary:** Outlined with a 1px border in Primary Red.
- **Urgent Action:** Primary Red with a subtle inner glow or pulse animation for emergency blood requests.

### Cards
Cards are the primary organizational unit. They should use `Level 1` elevation, a 16px corner radius, and 16px internal padding. Hero cards for donor stats may use the brand gradient with white text.

### Inputs & Selectors
Text fields use an "Outlined" M3 style. The border-color becomes 2px Primary Red on focus. Labels should float above the field.

### Status Chips
- **Urgent:** Red background, white text.
- **Available:** Success Green background, white text.
- **Pending:** Warning Orange background, white text.

### Specialty Components
- **The "Blood Type" Badge:** A circular, high-contrast element used in lists to show A+, B-, etc., using the Accent color to ensure it is the first thing a user sees.
- **Supply Tracker:** A thick, rounded progress bar using the gradient to show current blood inventory levels.