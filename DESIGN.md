---
version: alpha
name: Obsidian Veil
description: A desaturated graphite editorial-operating system inspired by futuristic dashboard interfaces, industrial minimalism, and tactile monochrome UI. The visual language centers around layered graphite surfaces, ultra-soft depth, translucent frosted panels, and warm mineral accents. Instead of vibrant SaaS chroma, the system uses restrained material tones — ash gray, oxidized green, clay red, faded bronze, and parchment beige. Typography is restrained, geometric, and calm, emphasizing silence, spacing, and interface hierarchy over marketing energy. Surfaces feel machined rather than decorative.

author: Clement-ccy

colors:
  primary: "#47645f"
  primary-active: "#2d3f3f"
  primary-disabled: "#89867a"

  ink: "#111111"
  body: "#3e3e3c"
  body-strong: "#1e1e1c"
  muted: "#6f6c66"
  muted-soft: "#9a978f"

  canvas: "#d9d7d3"
  canvas-soft: "#e2dfdb"

  surface-base: "#cfcac4"
  surface-soft: "#d8d4cf"
  surface-card: "#e5e1dc"

  surface-dark: "#1f2124"
  surface-dark-elevated: "#2a2d31"
  surface-dark-soft: "#35393d"

  glass: "rgba(255,255,255,0.08)"
  glass-strong: "rgba(255,255,255,0.14)"

  hairline: "#beb9b2"
  hairline-soft: "#d6d1cb"

  on-primary: "#f4f1ec"
  on-dark: "#ece8e1"
  on-dark-soft: "#a8a39c"

  accent-sand: "#f0e2d1"
  accent-stone: "#c9b4a2"
  accent-bronze: "#bd9b88"
  accent-rust: "#b84b3d"
  accent-earth: "#7a483c"

  success: "#47645f"
  warning: "#bd9b88"
  error: "#b84b3d"

typography:
  display-xl:
    fontFamily: "Satoshi, Inter, sans-serif"
    fontSize: 64px
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: -2px

  display-lg:
    fontFamily: "Satoshi, Inter, sans-serif"
    fontSize: 48px
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: -1.5px

  display-md:
    fontFamily: "Satoshi, Inter, sans-serif"
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -1px

  display-sm:
    fontFamily: "Satoshi, Inter, sans-serif"
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.18
    letterSpacing: -0.5px

  title-lg:
    fontFamily: "Inter, sans-serif"
    fontSize: 22px
    fontWeight: 500
    lineHeight: 1.3
    letterSpacing: -0.2px

  title-md:
    fontFamily: "Inter, sans-serif"
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0

  title-sm:
    fontFamily: "Inter, sans-serif"
    fontSize: 15px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0

  body-md:
    fontFamily: "Inter, sans-serif"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: 0

  body-sm:
    fontFamily: "Inter, sans-serif"
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0

  caption:
    fontFamily: "Inter, sans-serif"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.4px

  caption-uppercase:
    fontFamily: "Inter, sans-serif"
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 2px

  code:
    fontFamily: "JetBrains Mono, monospace"
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0

  button:
    fontFamily: "Inter, sans-serif"
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1
    letterSpacing: 0

  nav-link:
    fontFamily: "Inter, sans-serif"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.2px

rounded:
  xs: 6px
  sm: 10px
  md: 14px
  lg: 20px
  xl: 28px
  pill: 9999px
  full: 9999px

spacing:
  xxs: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  xxl: 48px
  section: 96px

elevation:
  shadow-soft: "0 8px 24px rgba(0,0,0,0.08)"
  shadow-medium: "0 12px 32px rgba(0,0,0,0.12)"
  shadow-panel: "0 20px 60px rgba(0,0,0,0.18)"
  inner-highlight: "inset 0 1px 0 rgba(255,255,255,0.08)"

blur:
  panel: 24px
  overlay: 40px

components:
  app-shell:
    backgroundColor: "{colors.canvas}"
    borderColor: "{colors.hairline-soft}"
    rounded: "{rounded.xl}"
    shadow: "{elevation.shadow-panel}"

  sidebar-rail:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    width: 76px
    rounded: "{rounded.lg}"

  sidebar-panel:
    backgroundColor: "{colors.surface-soft}"
    borderColor: "{colors.hairline-soft}"
    rounded: "{rounded.xl}"
    shadow: "{elevation.shadow-soft}"

  floating-toolbar:
    backgroundColor: "{colors.glass}"
    blur: "{blur.panel}"
    borderColor: "{colors.glass-strong}"
    rounded: "{rounded.lg}"

  navigation-item:
    backgroundColor: transparent
    textColor: "{colors.body}"
    typography: "{typography.nav-link}"
    rounded: "{rounded.md}"
    padding: 10px 14px

  navigation-item-active:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    borderColor: "{colors.hairline-soft}"
    rounded: "{rounded.md}"
    shadow: "{elevation.shadow-soft}"

  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: 12px 18px
    height: 40px

  button-primary-active:
    backgroundColor: "{colors.primary-active}"
    textColor: "{colors.on-primary}"

  button-secondary:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    borderColor: "{colors.hairline}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: 12px 18px
    height: 40px

  button-ghost:
    backgroundColor: transparent
    textColor: "{colors.muted}"
    typography: "{typography.button}"

  icon-button:
    backgroundColor: "{colors.surface-dark-elevated}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.full}"
    size: 40px

  glass-card:
    backgroundColor: "{colors.glass}"
    blur: "{blur.panel}"
    borderColor: "{colors.glass-strong}"
    rounded: "{rounded.lg}"
    shadow: "{elevation.shadow-medium}"

  dashboard-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    borderColor: "{colors.hairline-soft}"
    typography: "{typography.title-md}"
    rounded: "{rounded.lg}"
    padding: 28px
    shadow: "{elevation.shadow-soft}"

  dashboard-card-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    typography: "{typography.title-md}"
    rounded: "{rounded.lg}"
    padding: 28px

  metric-panel:
    backgroundColor: "{colors.surface-soft}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: 24px

  search-input:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.body}"
    borderColor: "{colors.hairline}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 44px

  search-input-focused:
    backgroundColor: "{colors.surface-card}"
    borderColor: "{colors.primary}"
    glow: "0 0 0 3px rgba(71,100,95,0.12)"

  panel-divider:
    color: "{colors.hairline-soft}"

  badge-neutral:
    backgroundColor: "{colors.surface-soft}"
    textColor: "{colors.body}"
    typography: "{typography.caption}"
    rounded: "{rounded.pill}"
    padding: 4px 10px

  badge-accent:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.caption-uppercase}"
    rounded: "{rounded.pill}"
    padding: 4px 12px

  status-success:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"

  status-warning:
    backgroundColor: "{colors.accent-bronze}"
    textColor: "{colors.ink}"

  status-error:
    backgroundColor: "{colors.accent-rust}"
    textColor: "{colors.on-primary}"

  modal-panel:
    backgroundColor: "{colors.surface-card}"
    borderColor: "{colors.hairline-soft}"
    rounded: "{rounded.xl}"
    padding: 40px
    shadow: "{elevation.shadow-panel}"

  command-palette:
    backgroundColor: "{colors.glass}"
    blur: "{blur.overlay}"
    borderColor: "{colors.glass-strong}"
    rounded: "{rounded.xl}"
    padding: 20px

  footer:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark-soft}"
    typography: "{typography.body-sm}"
    padding: 64px
---

# Overview

Obsidian Veil is a low-saturation graphite interface system designed around silence, density, and material depth. The interface language is influenced by industrial operating systems, monochrome hardware surfaces, architectural renders, and tactile desktop tooling rather than colorful SaaS products.

The dominant atmosphere is built from:
- graphite black structural rails
- fog-gray workspaces
- frosted translucent overlays
- warm mineral accent tones
- soft ambient shadows
- oversized spacing
- restrained typography

The interface should feel:
- tactile
- quiet
- engineered
- cinematic
- minimal
- spatially layered

No single surface is pure white or pure black. Everything sits inside a controlled grayscale spectrum with warm undertones.

## Key Characteristics

- Ultra-low saturation palette with warm mineral undertones
- Frosted translucent panels with soft blur
- Graphite navigation rails contrasted against pale workspace surfaces
- Large-radius containers and floating segmented layouts
- Minimal iconography with thin-line symbols
- Sparse accent usage via oxidized green and rust clay tones
- Soft shadows instead of high-contrast borders
- Geometric sans-serif typography with strong spacing discipline
- Dense dashboard compositions with calm visual pacing

# Surface Philosophy

The system uses five depth layers:

1. Graphite structural shell
2. Elevated dark controls
3. Neutral soft workspace panels
4. Frosted translucent overlays
5. Floating active states

Depth is communicated through:
- blur
- contrast compression
- ambient shadow
- edge highlights
- spacing

Never through strong borders or neon glow.

# Color Language

## Primary Accent

`{colors.primary}` (#47645f) is the core interaction color:
- active navigation
- focused controls
- selected graphs
- positive system state
- subtle glow accents

The darker `{colors.primary-active}` (#2d3f3f) is used for:
- pressed states
- structural dark controls
- dense interaction surfaces

## Warm Mineral Palette

The supporting accents are intentionally earthy:
- `{colors.accent-sand}` → parchment warmth
- `{colors.accent-stone}` → muted ceramic
- `{colors.accent-bronze}` → aged bronze
- `{colors.accent-rust}` → industrial oxide
- `{colors.accent-earth}` → deep clay shadow

These tones should appear sparingly:
- charts
- status indicators
- notification chips
- avatars
- illustrations
- data highlights

# Typography

Typography is quiet and controlled.

Display typography uses:
- Satoshi
- Inter
- SF Pro Display

Body typography stays:
- compact
- readable
- neutral

The system avoids:
- serif typography
- excessive boldness
- aggressive tracking
- marketing-style contrast

Headlines rely on scale and spacing rather than decorative styling.

# Layout

The interface follows a modular desktop-dashboard structure:
- fixed left rail
- expandable navigation panel
- central workspace
- floating cards
- isolated information islands

Spacing should remain generous even in dense data layouts.

Preferred rhythm:
- large outer margins
- compact inner density
- floating separation between groups

# Interaction Style

Motion should feel:
- inertial
- smooth
- quiet
- physical

Recommended timings:
- hover: 120ms
- panel expansion: 240ms
- modal transitions: 320ms
- blur fade: 280ms

Avoid:
- elastic bounce
- overscaled hover transforms
- saturated hover glows
- dramatic parallax

## Dynamic Surface & Theme Controls

Interactive surfaces should use the shared dashboard vocabulary rather than bespoke shadows:
- `ov-panel-surface` for large frosted panels and cards
- `ov-control-surface` for links, row cards, rail buttons, and clickable tiles
- `ov-inset-surface` for grouped read-only interiors and recessed metric wells
- `ov-switch` for compact rail-level theme controls

Depth ratios should stay tactile but restrained:
- the logical light source is the upper-right corner: highlights collect on top/right edges, while cast shadows fall toward the lower-left
- elongated pills and row controls should use a top-right to bottom-left diagonal sheen, not a side-mounted radial glow
- small controls around 36–60px may use 6–10px soft offset shadows, roughly 15–18% of the control size
- medium cards should use 12–18px ambient lift with a 1px inner highlight
- large shell/panel surfaces should keep highlight thickness at 1–2px while spreading shadow softly across 40–80px
- pressed states invert into inset shadow instead of adding glow

Theme switching happens through root-level `html[data-theme="light|dark"]` token swaps. The switch thumb moves in exact slot steps and may compress only subtly; theme colors retint through token transitions, not through saturated overlays.

Reduced-motion users should keep the color/token swap while removing meaningful translate, squash, or animated shadow travel.

# Do's

- Use grayscale dominance with restrained warm accents
- Keep shadows soft and wide
- Prefer translucency over opacity
- Use rounded-xl surfaces for primary workspace panels
- Maintain visual silence through spacing
- Use blur as a structural layer
- Let typography breathe

# Don'ts

- Don't use pure white
- Don't use saturated blue gradients
- Don't use hard black borders
- Don't use aggressive neumorphism
- Don't use colorful icon systems
- Don't use excessive glow
- Don't stack too many accent colors together
- Don't overanimate panels

# Responsive Behavior

## Mobile
- Sidebar rail collapses into floating bottom dock
- Panels become full-width stacked cards
- Blur intensity reduces for performance
- Dashboard grids collapse to single-column

## Tablet
- Workspace remains split-view
- Sidebar becomes icon-only
- Floating overlays become anchored sheets

## Desktop
- Full layered layout enabled
- Maximum depth and translucency active
- Multi-panel compositions preserved

# Known Gaps

- Chart styling tokens are undefined
- Dock behavior is conceptual only
- Glass blur rendering depends on browser GPU acceleration
- Dynamic lighting adaptation is outside current scope
