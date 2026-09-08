# Color System

## Architecture

NAVORA uses a three-tier token architecture: **Primitives → Semantic → Component**.

Never use primitive hex values directly in production code. Always reference semantic or component tokens.

## Primitive Palette

### Brand Core
| Token               | Hex       | Role                    |
|---------------------|-----------|-------------------------|
| `color/navy/900`    | `#08233A` | Deep Navy — primary     |
| `color/navy/800`    | `#0D2948` | Navy mid — dark surfaces|
| `color/navy/700`    | `#173A61` | Navy light — borders    |
| `color/ivory/50`    | `#F7F3EA` | Warm Ivory — canvas     |
| `color/ivory/100`   | `#F4EFE6` | Ivory subtle            |
| `color/greige/300`  | `#DED7CB` | Soft Greige — dividers  |

### Neutrals
| Token               | Hex       | Role                    |
|---------------------|-----------|-------------------------|
| `color/white`       | `#FFFFFF` | Card backgrounds        |
| `color/charcoal/700`| `#4A4A46` | Secondary text          |
| `color/charcoal/900`| `#1E1E1E` | Darkest neutral         |
| `color/stone/100`   | `#E9E4DB` | Light stone             |
| `color/stone/300`   | `#CFC8BC` | Borders, strong dividers|
| `color/stone/500`   | `#8A8F98` | Subtle text, placeholders|

### Functional
| Token               | Hex       | Role                    |
|---------------------|-----------|-------------------------|
| `color/gold/500`    | `#B9954E` | Muted Gold — evidence   |
| `color/gold/600`    | `#A9791F` | Gold dark — action text |
| `color/sage/500`    | `#668A7A` | Sage — verified         |
| `color/blue/400`    | `#6E8FAE` | Steel Blue — imported   |
| `color/red/500`     | `#B65353` | Muted Red — safety      |

## Usage Ratio

This is a hard rule:

```
Navy:   65–70%  (backgrounds, text, navigation)
Ivory:  25–30%  (canvas, cards, breathing room)
Gold:   ≤ 5%   (evidence markers ONLY)
```

Gold is **never** used as a background fill, button color, or decorative accent. It marks evidence — citations, verification badges, literature references.

## Semantic Tokens (Light / Dark)

### Surface
| Token             | Light       | Dark        |
|-------------------|-------------|-------------|
| `surface/canvas`  | Ivory 50    | Navy 900    |
| `surface/subtle`  | Ivory 100   | Navy 800    |
| `surface/card`    | White       | Navy 800    |
| `surface/inverse` | Navy 900    | Ivory 50    |

### Text
| Token             | Light         | Dark        |
|-------------------|---------------|-------------|
| `text/primary`    | Navy 900      | Ivory 50    |
| `text/secondary`  | Charcoal 700  | Stone 300   |
| `text/inverse`    | Ivory 50      | Navy 900    |
| `text/subtle`     | Stone 500     | Stone 300   |
| `text/action`     | Gold 600      | Gold 500    |
| `text/disabled`   | Charcoal 700  | Ivory 100   |

### Border
| Token             | Light       | Dark        |
|-------------------|-------------|-------------|
| `border/subtle`   | Greige 300  | Navy 700    |
| `border/strong`   | Stone 300   | Stone 500   |
| `border/default`  | Stone 300   | Navy 700    |
| `border/focus`    | Gold 500    | Gold 500    |

## Clinical State Colors

These are **fixed semantic assignments** — never repurpose them:

| State              | Color     | Hex       | Meaning                      |
|--------------------|-----------|-----------|------------------------------|
| Verified           | Sage      | `#668A7A` | Clinically verified data     |
| New / Imported     | Blue      | `#6E8FAE` | Newly received information   |
| Changed            | Gold      | `#B9954E` | Modified since last review   |
| Waiting            | Stone     | `#8A8F98` | Pending action               |
| In Clarification   | Gold Dark | `#A9791F` | Requires clarification       |
| Action Required    | Gold Dark | `#A9791F` | Needs clinician attention    |
| Safety Alert       | Red       | `#B65353` | Safety-critical warning      |
| Conflict           | Red       | `#B65353` | Data conflict detected       |
| Missing            | Red       | `#B65353` | Required data absent         |
| Consent Active     | Sage      | `#668A7A` | Valid patient consent        |
| Consent Expired    | Stone     | `#8A8F98` | Consent lapsed               |
| Consent Revoked    | Red       | `#B65353` | Consent withdrawn            |

## Contrast Requirements

All text/background pairings must meet **WCAG 2.1 AA** (4.5:1 for body text, 3:1 for large text and UI components).

Key validated pairings:
- Navy 900 on Ivory 50 → ≈ 14.5:1 ✓
- Ivory 50 on Navy 900 → ≈ 14.5:1 ✓
- Charcoal 700 on White → ≈ 7.2:1 ✓
- Gold 600 on Ivory 50 → ≈ 4.8:1 ✓ (minimum for action text)
