---
name: Aero-Sail
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#20201f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353535'
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
  secondary: '#bdf4ff'
  on-secondary: '#00363d'
  secondary-container: '#00e3fd'
  on-secondary-container: '#00616d'
  tertiary: '#c6c6c6'
  on-tertiary: '#2f3131'
  tertiary-container: '#090a0b'
  on-tertiary-container: '#79797a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c9c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#9cf0ff'
  secondary-fixed-dim: '#00daf3'
  on-secondary-fixed: '#001f24'
  on-secondary-fixed-variant: '#004f58'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353535'
typography:
  display-lg:
    fontFamily: JetBrains Mono
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.02em
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.4'
    letterSpacing: 0em
  data-readout:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
  container-max: 1440px
---

## Brand & Style

This design system is engineered for elite offshore racing, where split-second decisions rely on high-density data visualization. The aesthetic is a fusion of **Glassmorphism** and **Technical Minimalism**, mimicking the heads-up display (HUD) of a high-performance carbon fiber vessel.

The brand personality is precise, cold, and hyper-functional. It evokes the feeling of a "Tactical Command Center," utilizing translucent layers to maintain a sense of depth and spatial awareness. Vector-line motifs—inspired by aerodynamic flow and isobaric maps—should be used as subtle background textures to imply movement and wind dynamics. The goal is to provide a "cockpit" experience that feels both futuristic and mission-critical.

## Colors

The palette is strictly functional, optimized for low-light marine environments and high-glare daytime conditions.

- **Primary Background:** Carbon Black (#0A0A0A) is used for the base environment to minimize eye strain and maximize the contrast of data overlays.
- **Data Highlights & AI:** Electric Blue (#00E5FF) is the primary "action" and "insight" color. Use this for active routes, AI-suggested maneuvers, and critical sensor peaks.
- **Secondary UI:** Metallic Silver (#C0C0C0) provides structure for labels, borders, and inactive states.
- **Tonal Accents:** Use dark grey variations (#1A1A1A) for surface containers to create a layered "stack" effect without losing the deep-black aesthetic.

## Typography

This design system utilizes a dual-font strategy to balance legibility with technical character.

- **Technical Readouts:** JetBrains Mono is used for all numerical data and primary headers. Its monospaced nature ensures that rapidly changing telemetry values do not cause layout "jitter."
- **Interface & Content:** Inter is used for descriptions, settings, and general UI text to provide high legibility in stressful conditions.
- **Styling:** Use all-caps with increased tracking for labels to mimic engineering blueprints. Data readouts should be sized aggressively for immediate recognition from a distance.

## Layout & Spacing

The layout follows a **Rigid Technical Grid** based on a 4px baseline.

- **Desktop (Racing Terminal):** A 12-column fluid grid. Components should snap to the grid to maintain a "panel-mount" look. Gutters are kept tight (16px) to maximize data density.
- **Tablet (Handheld):** An 8-column grid focused on touch-targets for wet environments. Large margins (24px) prevent accidental edge-touches.
- **Philosophy:** Information density is prioritized over whitespace. Related data points should be clustered into logical "Instrument Clusters."

## Elevation & Depth

Depth is achieved through **Glassmorphism** rather than traditional shadows. This maintains the "heads-up display" metaphor.

- **Base Layer:** Pure Carbon Black (#0A0A0A).
- **Instrument Panels:** Semi-transparent Metallic Silver (8-12% opacity) with a 20px backdrop blur. 
- **Borders:** Every panel must have a 1px solid border in Metallic Silver at 20% opacity to define the edge against the dark background.
- **Active Elevation:** When a panel is "focused" or "alerting," the border-color shifts to Electric Blue with a subtle 4px outer glow (0 0 8px rgba(0, 229, 255, 0.3)).

## Shapes

The shape language is **Sharp and Industrial**. 

- **Primary Geometry:** 0px border radius for all main containers and panels to reflect the precision of carbon fiber construction and structural ribs.
- **Functional Elements:** Subtle 45-degree "dog-ear" or chamfered corners can be used on primary action buttons to distinguish them from data containers.
- **Internal Elements:** Gauges and compasses remain perfectly circular, but are encased in square frames to maintain grid integrity.

## Components

- **Telemetry Cards:** Utilize glassmorphism backgrounds. The top-left corner should feature a small "label-caps" identifier, while the center features a large "data-readout."
- **Action Buttons:** Ghost-style buttons with 1px Metallic Silver borders. On hover/active, the background fills with a 10% Electric Blue tint and the border glows.
- **Toggle Switches:** Rectangular and binary. Use Electric Blue for the "On" state, resembling a physical cockpit toggle light.
- **AI Suggestion Overlay:** Panels with a distinct Electric Blue left-accent bar (3px width) to indicate they are generated by the tactical engine.
- **Gauges:** Vector-line circular gauges with "needle" indicators in Electric Blue. Use fine-line increments (0.5px) for the metallic scale.
- **Input Fields:** Bottom-border only (1px Silver), moving to Electric Blue on focus. Use monospaced font for all numeric entry.