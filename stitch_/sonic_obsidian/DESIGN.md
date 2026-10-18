---
name: Sonic Obsidian
colors:
  surface: '#0f131d'
  surface-dim: '#0f131d'
  surface-bright: '#353944'
  surface-container-lowest: '#0a0e18'
  surface-container-low: '#171b26'
  surface-container: '#1b1f2a'
  surface-container-high: '#262a34'
  surface-container-highest: '#313540'
  on-surface: '#dfe2f0'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#dfe2f0'
  inverse-on-surface: '#2c303b'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#cdbdff'
  on-secondary: '#370096'
  secondary-container: '#5203d5'
  on-secondary-container: '#c0acff'
  tertiary: '#a8ffd2'
  on-tertiary: '#003824'
  tertiary-container: '#5be9ad'
  on-tertiary-container: '#006645'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#e8deff'
  secondary-fixed-dim: '#cdbdff'
  on-secondary-fixed: '#20005f'
  on-secondary-fixed-variant: '#4f00d0'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#0f131d'
  on-background: '#dfe2f0'
  surface-variant: '#313540'
typography:
  headline-xl:
    fontFamily: Rubik
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Rubik
    fontSize: 26px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Rubik
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Rubik
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
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
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '600'
    lineHeight: 18px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
    letterSpacing: 0.04em
  technical-data:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.08em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-desktop: 1.5rem
  margin: 1rem
  margin-desktop: 2.5rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

This design system defines an audiophile-grade, ultra-refined digital listening environment. Engineered for power users, critical listeners, and modern music purists, it merges the relentless organizational utility of Musicolet with the luminous, tactile polish of bespoke luxury electronics.

### Design Language & Influences
- **OLED Surface Architecture:** The UI is rooted in layered deep charcoal and true black surfaces, minimizing light emission while maximizing contrast and power efficiency.
- **Luminescent Glass & Precision Glow:** Interfaces employ subtle frosted glass sheens, micro-diffused ambient glows behind active playback components, and hairline translucent borders that clearly demarcate functional zones without adding visual mass.
- **Technical Pragmatism:** Aesthetic choices prioritize dense audio telemetry—sampling rates, bitrate indicators, dynamic parametric EQ bars, and complex multi-queues—without feeling cluttered.
- **Emotional Cadence:** Precision-engineered, immersive, nocturnal, and unapologetically focused on the acoustic medium.

## Colors

The palette operates on pure chromatic contrast against a layered obsidian substrate. Light emission is strictly reserved for playback status, audio resolution badges, active states, and user interaction feedback.

### Palette Architecture
- **Primary (`#00E5FF` - Cyan Surge):** Core interactive focal points, active scrubbers, play/pause state halos, and lossless stream badges.
- **Secondary (`#7C4DFF` - Electric Violet):** Multi-queue navigation chips, secondary playback parameters, and auxiliary audio modes (e.g., crossfade, reverb).
- **Tertiary (`#10B981` - Emerald Resonance):** Direct audio indicators, bit-perfect playback confirmation, sample rate metrics (e.g., 24-bit / 192kHz), and volume safety headrooms.
- **Neutral Base (`#0B0D13` to `#121620`):** Pitch black canvas for zero battery waste on OLED panels, ascending to `#1A202C` for floating sheets and dynamic queue decks.
- **Glass & Borders:** `rgba(255, 255, 255, 0.08)` for borders and micro-separators; `rgba(0, 229, 255, 0.15)` for focused states.
- **Typography Colors:** `#F1F5F9` (Primary track titles/metrics), `#94A3B8` (Artist names/secondary data), `#475569` (Inactive icons/timestamps).

## Typography

Typography prioritizes extreme clarity under motion, varying light conditions, and dense data environments. 

### Implementation Rules
- **Display & Headings (Rubik):** Softened geometric terminals inject warmth into an otherwise technical layout. Used for track titles, album names, modal headlines, and queue designations. Fully supports bidirectional scripts (RTL/LTR).
- **Body & Metadata (Inter):** Highly legible grotesque sans-serif with tall x-height and open apertures. Retains clarity even when displaying micro-telemetry (e.g., `FLAC · 9216 kbps · 192 kHz / 24-bit`).
- **Tabular Numerals:** Always enforce `font-feature-settings: "tnum" 1` on playback duration timers, millisecond displays, and parametric EQ band readouts to eliminate horizontal jitter during playback.
- **Badge Casing:** Audio profile tags (`HI-RES`, `DSD`, `MQA`, `LOSSLESS`) strictly use `technical-data` in uppercase with expanded tracking.

## Layout & Spacing

The layout is built upon an 8pt base grid with a 4pt sub-grid for high-density audio controls and equalizer parameters.

### Screen Adaptations
- **Mobile Handheld (Below 768px):** Single-column layout. Sticky persistent bottom mini-player (64px height) with full swipe-up gesture reveal for the full-screen player deck. Outer margins are fixed at `space-md` (1rem). Touch targets are kept strictly to a 44x44px minimum bounding box despite compact visual icons.
- **Tablet & Split-View (768px - 1024px):** 8-column layout. Dual pane mode: persistent queue on the left (35% width), rich artwork and controls on the right (65% width).
- **Desktop / Studio View (Above 1024px):** 12-column system with outer margins at `margin-desktop` (2.5rem). Three distinct visual modules: Queue & Tag Navigator, Stage View / Waveform visualizer, and Master DSP / Equalizer Dock.

### Spatial Rhythm
- Components use `space-xs` and `space-sm` for internal metadata packaging (e.g., track artist and audio badge gap).
- `space-lg` and `space-xl` are reserved for structural breaks between master transport controls, waveform progress bars, and metadata decks.

## Elevation & Depth

Visual depth is achieved through translucent material hierarchy and luminance emission rather than traditional drop shadows.

### Surface Tiers
- **Canvas Base (`#0B0D13`):** Zero elevation. Deep pitch black background.
- **Surface Level 1 (`#121620` at 85% opacity with `backdrop-filter: blur(16px)`):** List items, track tiles, and persistent side navigation.
- **Surface Level 2 (`#1A202C` at 70% opacity with `backdrop-filter: blur(24px)`):** Popover equalizer modules, dynamic multi-queue management cards, and active track drawers.
- **Surface Level 3 (`#242D3D` at 90% opacity):** Tooltips, lossless format inspectors, and menu modals.

### Edge Illumination & Glow
- **Translucent Edge Lines:** Containers use a 1px top-to-bottom subtle gradient border (`rgba(255, 255, 255, 0.12)` fading to `rgba(255, 255, 255, 0.02)`) that mimics physical beveled glass.
- **Acoustic Luminescence:** Active primary components (e.g., glowing scrub head, playing track row) project a concentrated ambient glow: `box-shadow: 0 0 24px rgba(0, 229, 255, 0.22), 0 0 4px rgba(0, 229, 255, 0.45)`.

## Shapes

The design system adopts a balanced roundedness (Level 2), projecting modern ergonomic comfort without sacrificing the precision feel of professional audio gear.

### Corner Radius System
- **Base (0.5rem / 8px):** Interactive buttons, track list row hover states, audio metric chips, and standard text fields.
- **Large (1rem / 16px):** Album artwork wrappers, mini-player floating bar, parametric EQ graph containers, and full-screen drawer sheets.
- **Extra-Large (1.5rem / 24px):** Primary dialogs, DSP configuration popovers, and contextual action trays.
- **Full Pill (`9999px`):** Playback scrubber track, volume sliders, multi-queue switch tabs, and primary action buttons (e.g., "Shuffle All").

## Components

### Buttons
- **Primary Play/Pause Button:** Circular (56px or 64px), filled with `#00E5FF` gradient (`to bottom right, #00E5FF, #00B4D8`), content tinted `#0B0D13` for contrast. Elevated by a 16px diffuse cyan glow.
- **Secondary Transport (Skip, Previous, Repeat, Shuffle):** Ghost button style, 40x40px touch zone, icon colored `#94A3B8`. Switches to `#7C4DFF` with a micro-dot indicator beneath when active.
- **Tactile Toggle:** Audio FX toggles possess a recessed physical feel: inset `1px` translucent border with active state shifting surface fill from `#121620` to `#10B981` at 15% opacity.

### Queue Chips & Tags
- Compact height (28px) with full pill radius. 
- Inactive state: `rgba(255, 255, 255, 0.05)` surface with `#94A3B8` label.
- Multi-queue state (Queue 1–Queue 4): Colored indicator dot tinted with `#7C4DFF`, highlighting currently playing queue vs. backgrounded queues.

### Lists & Track Items
- Single row height: 60px.
- Track index / drag handle positioned on the start edge. High-resolution album thumbnail (44x44px, 8px radius) with subtle inner border.
- Now-Playing row treatment: Background transitions to `linear-gradient(90deg, rgba(0, 229, 255, 0.08) 0%, transparent 100%)`. Text becomes `#00E5FF`, accompanied by an animated three-bar equalizer graphic.

### Sliders, Seekers & Waveform Scrubbers
- **Waveform Seeker:** Visualizes discrete audio amplitude bars. Unplayed region rendered in `#334155`; played region illuminated in `#00E5FF`. The scrubber handle is an illuminated pill showing exact millisecond offset on drag.
- **Volume & EQ Sliders:** Dual-tone fill line with tactile knurled thumb indicator (`16px` diameter, `#F1F5F9` with inner dark core).

### Badges & Technical Indicators
- **Hi-Res Audio Badges:** Border-only badges (`1px` solid `rgba(16, 185, 129, 0.4)`) with text `#10B981`. Displayed adjacent to track title.
- **Bitrate Pill:** Ultra-compact chip containing monospace audio format details (`FLAC · 24b/96k`), styled in `technical-data` typography.

### Input Fields & Search
- Low-profile inputs (40px) with frosted glass background (`#121620` at 60%), subtle border, and integrated instant-filter icon for real-time tag and folder search across Musicolet-style directory structures.