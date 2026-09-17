# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Competitive and casual Beyond All Reason (BAR) RTS players executing fast-paced opening strategies, scouting adaptations, and economy planning on a secondary display or via quick alt-tabbing during active matchplay and pre-game lobbies.

## Product Purpose
Provide real-time tactical intelligence, AI-synthesized build order timelines, map topography analyses, and dynamic economic runway calculations to help players optimize opening execution, prevent energy/metal stalls, and counter opposing faction doctrines.

## Positioning
An active tactical commander console linked directly to the live game client via a low-latency local memory bridge daemon. Unlike static build guide websites, BAR StratCom dynamically detects in-game match state, computes live wind power curves, and generates context-aware build macros with one-click clipboard export.

## Operating Context
Operated alongside the active Beyond All Reason game client in dual-monitor setups or during lobby countdowns. Players operate under high APM and intense time pressure, requiring sub-second glanceable data: opening build steps with clear timestamps, unit counts, chokepoint callouts, and economic threshold warnings.

## Capabilities and Constraints
- Real-time match telemetry synchronization via local memory bridge daemon (scripts/bar_live_bridge.py).
- Automated opening queue generation powered by Gemini 1.5 Pro or local tactical ruleset fallback.
- Faction-specific support for Armada and Cortex, with dedicated tech tree logic and unit iconography.
- Map topography database with wind velocity bands, tidal energy yields, metal densities, and critical chokepoints.
- Economic runway oscilloscope visualization for metal/energy production vs expenditure.
- One-click tactical build macro export (Ctrl+C) for fast in-game team sharing.
- Strict constraint: Maintain ultra-clean high-contrast readability and compact data density for fast glancing during high-APM games without sacrificing the retro arcade aesthetic.

## Brand Commitments
- 16-bit retro arcade commander console aesthetic inspired by *Advance Wars*, *Metal Slug*, and *Dune II*.
- Stepped rigid pixel containers (.pixel-box, .pixel-box-inset) with zero border radius.
- Authentic faction palettes: Armada Cyan (#00f0ff), Cortex Flame Red (#ff2244), Energy Gold (#fbbf24), Metal Chrome (#94a3b8).
- Tactile chunky arcade buttons (.pixel-btn) with 3px shadow depression.
- Full-screen CRT scanline shader with chromatic shadow mask and tube vignette.
- Pixel typography pairing: Press Start 2P for tactical headings and VT323 for telemetry data.

## Evidence on Hand
- Live game bridge daemon scripts (scripts/bar_live_bridge.py).
- 50+ official Beyond All Reason maps scraped with wind, tidal, metal, chokepoint data, and competitive doctrines (src/lib/map-data.ts).
- Full sprite asset library for Armada and Cortex units, buildings, and commander badges (public/icons/units/, public/armada-logo.png, public/cortex-logo.png).
- Production Next.js 16 app with Tailwind CSS v4 and Framer Motion running on http://localhost:3000.

## Product Principles
1. **Glanceability Under Fire**: Information must be legible in under 500ms. Numbers, timestamps, and unit portraits must stand out against the backdrop during fast-paced RTS gameplay.
2. **Deterministic Trust First**: Real game telemetry and accurate map parameters take absolute precedence over generative embellishments.
3. **Tactile Retro Immersion**: The 16-bit arcade commander theme must feel cohesive, crunchy, and intentional, like authentic battlefield hardware.
4. **Zero-Latency Response**: Interactions, tab switches, and macro copies must be instantaneous with zero lag or disruptive layout shifts.

## Accessibility & Inclusion
- High-contrast visual modes conforming to WCAG AA for data readouts.
- Full keyboard shortcuts (Enter to generate, Ctrl+C to copy macro).
- Strict non-blocking pointer events on CRT visual shader overlays.
