# Anti-Vibecoding Architectural & Design Rules

This project enforces strict rejection of the **20 "Vibecoded" Design Anti-Patterns** identified by Michael Ly (@millee.md). All UI elements, AI prompts, and styles must uphold authentic 16-bit arcade CRT tactical craft rather than generic AI-generated template clichés.

---

## The 20 Vibecoded Anti-Patterns & Theory-App Enforcement

### 1. No Purple-to-Blue Gradients
- **Anti-pattern**: Lazy `bg-gradient-to-r from-indigo-500 to-purple-600` backgrounds or buttons.
- **Enforcement**: Deep arcade charcoal and obsidian palettes (`#0a0c14`, `#0c0e18`, `#12131a`) with authentic faction accents:
  - Armada: `#449bed` (Electric Tactical Blue)
  - Cortex: `#e63946` (Combustion Red)
  - Legion: `#2ec4b6` (Cyber Teal)

### 2. No Gradient Hero Text
- **Anti-pattern**: `bg-clip-text text-transparent bg-gradient-to-r...` on headlines.
- **Enforcement**: Solid, crisp text colors (`text-white`, `text-amber-300`, `text-[#449bed]`) with optional hard pixel drop shadows (`shadow-[2px_2px_0px_#000]`).

### 3. No Emojis in Headings & Tactical Statuses
- **Anti-pattern**: Decorating section headers with emojis like `⚡ Macro:`, `🎯 Execution:`, `⚔️ 1v1 DUEL`, `🚨 PUSH:`.
- **Enforcement**: Military bracket indicators and retro arcade tags:
  - `### [MACRO DISCIPLINE]`
  - `### [EXECUTION PHASES]`
  - `[1v1 DUEL]`, `[MAP]: ...`, `[PUSH]: ...`, `[TACTICAL ADVICE]:`

### 4. No "Inter Font Everywhere"
- **Anti-pattern**: Defaulting every single paragraph and heading to generic Inter.
- **Enforcement**: Purposeful typography stack:
  - Headings & Badges: `var(--font-pixel-heading)` (Press Start 2P)
  - Body & Telemetry: `var(--font-pixel-body)` (VT323)
  - Monospace Data: `font-mono`

### 5. No Lazy Colored Left-Border Cards
- **Anti-pattern**: Plain card with only `border-l-2 border-indigo-500` to fake design effort.
- **Enforcement**: Complete 2px solid borders (`border-2 border-black` or `border border-zinc-800`), crisp pixel inset wells (`pixel-box-inset`), or pixel boxes with hard corner notches.

### 6. No Glassmorphism Cards
- **Anti-pattern**: `backdrop-blur-sm` or `backdrop-blur-md` on dark mode cards.
- **Enforcement**: High-opacity solid panels (`bg-black/90` or `bg-[#0d101a]`). Glassmorphism breaks the 16-bit CRT aesthetic and degrades frame rendering.

### 7. No Low-Contrast Dark Mode
- **Anti-pattern**: Subdued dark gray text on black (`text-zinc-600` or `text-zinc-700` for readable labels).
- **Enforcement**: Minimum contrast floor of `text-zinc-400` on dark obsidian backgrounds. Primary copy is `text-zinc-200` or `text-white`.

### 8. No Generic "3 Icon Boxes in a Row"
- **Anti-pattern**: 3 equal cards in a row with a centered icon in a colored circle and generic marketing copy.
- **Enforcement**: Dense tactical HUD layouts, live telemetry streams, unit breakdown counters, and split-screen operational panes.

### 9. No Generic Pill Badges Above Headlines
- **Anti-pattern**: `rounded-full` pill with `✨ What's New` floating above every title.
- **Enforcement**: Sharp rectangular arcade tags (`rounded-none border border-black font-pixel-heading text-[8px] uppercase tracking-wider`).

### 10. No Overused Stock Icons Without Context
- **Anti-pattern**: Generic spark, lightning bolt, or zap icon plopped on every button.
- **Enforcement**: Specialized SVG silhouettes (e.g. `BarIcon` rendering authentic Beyond All Reason factory, solar, wind, and commander silhouettes).

### 11. No Untouched Shadcn UI Defaults
- **Anti-pattern**: Stock `rounded-xl` cards, `rounded-4xl` pills, and blurry `focus-visible:ring-3`.
- **Enforcement**: Overhauled primitives in `src/components/ui/` with `rounded-none`, `border-2 border-black`, and tactile 2px offset button presses (`active:translate-y-0.5`).

### 12. No Fade-In on Scroll
- **Anti-pattern**: Everything opacity-fading into view as the page scrolls.
- **Enforcement**: Immediate, punchy arcade rendering. Scanline flicker and CRT power-on effects instead of smooth SaaS fades.

### 13. No Cursor-Following Beam / Spotlight
- **Anti-pattern**: Radial gradient spotlight following mouse cursor across the screen.
- **Enforcement**: CRT scanline overlay (`.crt-scanlines`) and authentic arcade border styling.

### 14. No Floating Button Fade on Hover
- **Anti-pattern**: `transition-all duration-300 hover:opacity-80`.
- **Enforcement**: Instantaneous tactile state changes: `transition-none active:translate-y-0.5 active:shadow-none`.

### 15. No Inconsistent Spacing
- **Anti-pattern**: Random mixing of `gap-3`, `gap-7`, `p-5`, `p-9`.
- **Enforcement**: Strict 4px/8px modular grid spacing (`p-2`, `p-3`, `p-4`, `p-6`, `gap-2`, `gap-3`, `gap-4`).

### 16. No Em Dashes Everywhere
- **Anti-pattern**: Flooding copy and titles with em dashes (`—` and `–`).
- **Enforcement**: Tactical delimiters (`//`, `::`, `▸`, `|`, or concise hyphenation).

### 17. No Generic Buzzword Copy
- **Anti-pattern**: Words like "seamlessly", "supercharge", "unleash", "revolutionary", "elevate".
- **Enforcement**: Precise, domain-expert RTS language ("direct metal reclaim", "guaranteed +60E launchpad", "nanofabrication throughput", "radar choke coverage").

### 18. No Serif Italic Accents on Headlines
- **Anti-pattern**: Mixing a modern sans-serif with a random *italic serif* word to fake luxury.
- **Enforcement**: Bold, uncompromising 8-bit / 16-bit pixel typography with retro-tactical telemetry formatting.

### 19. No Space Grotesk + Instrument Serif Clichés
- **Anti-pattern**: The trendy "AI portfolio / landing page font pairing".
- **Enforcement**: `Press Start 2P` + `VT323`.

### 20. No Fake Grain Texture Overlays
- **Anti-pattern**: High-contrast noisy SVG grain faking vintage texture.
- **Enforcement**: Scanlines and phosphor CRT styling tailored specifically for arcade RTS simulation.
