# NAVORA Brand Design System

**Version 1.2** — Premium Clinical Intelligence Infrastructure

NAVORA is a healthcare product family providing evidence-based clinical intelligence across three products: **Patient**, **Provider**, and **Nexus**.

---

## Repository Structure

```
navora-brand-system/
├── README.md                          ← You are here
├── NAVORA_Brand_System_v1.2.pdf       ← Complete brand document (export from Figma)
├── assets/
│   ├── logos/
│   │   └── svg/
│   │       ├── master-lockup-tagline.svg   ← Primary logo with tagline
│   │       ├── wordmark.svg                ← NAVORA wordmark (all variants)
│   │       ├── wordmark-navy.svg           ← Wordmark, navy fill
│   │       ├── glyph.svg                   ← N-glyph mark (all variants)
│   │       ├── glyph-navy.svg              ← Glyph, navy fill
│   │       ├── glyph-ivory.svg             ← Glyph, ivory fill (for dark backgrounds)
│   │       ├── monochrome.svg              ← Monochrome lockup (all variants)
│   │       └── horizontal-transparent.svg  ← Horizontal logo, transparent bg
│   └── app-icon/
│       └── app-icon-1024.png               ← App icon at 1024×1024
├── tokens/
│   ├── colors.json          ← Primitive + semantic color tokens (Light/Dark)
│   ├── typography.json      ← Typography scale & font stack
│   ├── dimensions.json      ← Spacing, radius, icon sizes, strokes
│   ├── components.json      ← Component-level token aliases
│   └── effects.json         ← Elevation & focus ring shadows
└── docs/
    ├── brand-constitution.md    ← Core brand principles
    ├── color.md                 ← Color palette & usage rules
    ├── typography.md            ← Type scale & pairing rules
    ├── spacing-and-layout.md    ← Grid, spacing, radius system
    ├── logo-usage.md            ← Logo system & clear space rules
    ├── components.md            ← Component inventory & token mapping
    ├── accessibility.md         ← WCAG compliance checklist
    ├── writing-system.md        ← Voice, tone & copy guidelines
    └── do-and-dont.md           ← Visual do/don't reference
```

## Quick Start

### For Designers
Open the [Figma source file](https://www.figma.com/file/ckQOi3oKtUlAW5U9Ajp0xb) and enable the NAVORA library to access all components, styles, and variables.

### For Developers
1. Import tokens from `tokens/` into your build pipeline (compatible with [Style Dictionary](https://amzn.github.io/style-dictionary/), [Tokens Studio](https://tokens.studio/), and the [W3C Design Tokens](https://design-tokens.github.io/community-group/format/) spec)
2. Reference `docs/` for implementation rules
3. Use SVGs from `assets/logos/svg/` — all logos are production-ready vector files

### Exporting the Brand PDF
The complete 28-chapter brand document should be exported directly from Figma:
1. Open the NAVORA Brand Design System file
2. Navigate to the **"27 — EXPORT PAGE"** page
3. Use **File → Export frames to PDF**

---

## Core Palette

| Role         | Hex       | Usage                          |
|--------------|-----------|--------------------------------|
| Deep Navy    | `#08233A` | Primary brand — 65–70% of UI  |
| Warm Ivory   | `#F7F3EA` | Canvas/background — 25–30%    |
| Soft Greige  | `#DED7CB` | Borders, dividers             |
| Muted Gold   | `#B9954E` | Evidence markers — max 5%     |
| Sage Green   | `#668A7A` | Verified/success states       |
| Steel Blue   | `#6E8FAE` | New/imported data states      |
| Muted Red    | `#B65353` | Safety alerts, conflicts      |

## Font Stack

| Role      | Family         | Usage                                    |
|-----------|----------------|------------------------------------------|
| Display   | Newsreader     | Headlines, hero text (Display/XL–H3)     |
| Body      | Inter          | UI text, labels, paragraphs (Body/L–S)   |
| Data      | IBM Plex Mono  | Clinical values, timestamps (Data/M–S)   |

## Products

| Product   | Platform  | Description                                |
|-----------|-----------|--------------------------------------------|  
| Patient   | Mobile    | Patient-facing health record (340×802)     |
| Patient   | Desktop   | Patient portal — expanded view (1088×802)  |
| Provider  | Desktop   | Clinician workspace (1504×1020)            |
| Nexus     | Desktop   | Coordination hub — cross-patient (1504×1010)|

---

## Design Token Architecture

```
Primitives  →  Semantic  →  Component
(raw values)   (intent)     (specific usage)
```

**4 Variable Collections, 133 tokens total:**
- `NAVORA/Primitives` — 17 COLOR (raw hex values)
- `NAVORA/Semantic` — 31 COLOR (Light + Dark modes)
- `NAVORA/Dimensions` — 26 FLOAT (spacing, radius, sizes, strokes)
- `NAVORA/Component` — 50 COLOR (Light + Dark modes)

All semantic and component tokens support **Light** and **Dark** modes.

---

## License

Proprietary — NAVORA brand assets are not licensed for external use without written permission.
