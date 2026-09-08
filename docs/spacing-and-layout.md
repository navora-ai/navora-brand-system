# Spacing & Layout

## Spacing Scale

Base unit: **4px**

| Token      | Value | Usage                                     |
|------------|-------|-------------------------------------------|
| `space/0`  | 0px   | No gap (tight stacking)                   |
| `space/1`  | 4px   | Minimum gap — icon-to-label, tight pairs  |
| `space/2`  | 8px   | Inline spacing — between related elements |
| `space/3`  | 12px  | Compact card padding                      |
| `space/4`  | 16px  | Default content padding                   |
| `space/5`  | 20px  | Comfortable card padding                  |
| `space/6`  | 24px  | Section internal spacing                  |
| `space/8`  | 32px  | Between content groups                    |
| `space/10` | 40px  | Section dividers                          |
| `space/12` | 48px  | Major section gaps                        |
| `space/16` | 64px  | Page-level vertical rhythm               |

### Spacing Rules

1. **4px increments only** — no arbitrary values like 5px, 7px, or 15px
2. **Smaller inside, larger outside** — card content padding < card margin < section margin
3. **Consistent axis spacing** — horizontal and vertical gaps in the same container should use the same token or adjacent tokens

## Border Radius Scale

| Token        | Value  | Usage                            |
|--------------|--------|----------------------------------|
| `radius/none`| 0px    | Tables, full-bleed sections      |
| `radius/xs`  | 4px    | Tags, small badges               |
| `radius/sm`  | 6px    | Input fields, small cards        |
| `radius/md`  | 10px   | Cards, modals, dropdowns         |
| `radius/lg`  | 16px   | Large cards, panels              |
| `radius/xl`  | 24px   | Feature cards, hero elements     |
| `radius/round`| 999px | Avatars, pills, circular buttons |

### Radius Rules

1. **Nested elements reduce radius** — if a card is `md` (10px), its inner elements use `sm` (6px) or `xs` (4px)
2. **Never mix round and sharp** — a container with rounded corners should not have sharp-cornered children (except data tables)
3. **radius/round is for circular shapes only** — avatars, status dots, pill buttons

## Icon Sizes

| Token         | Value | Usage                          |
|---------------|-------|--------------------------------|
| `size/icon/sm`| 16px  | Inline icons in body text      |
| `size/icon/md`| 20px  | Default UI icons               |
| `size/icon/lg`| 24px  | Navigation, primary actions    |

## Touch Targets

| Token          | Value | Rule                                       |
|----------------|-------|--------------------------------------------|  
| `size/tap/min` | 44px  | Minimum tap target for all interactive elements (WCAG 2.5.8) |

## Stroke Weights

| Token              | Value  | Usage                          |
|--------------------|--------|--------------------------------|
| `stroke/hairline`  | 0.5px  | Subtle dividers                |
| `stroke/default`   | 1px    | Standard borders               |
| `stroke/emphasis`  | 2px    | Active states, focus indicators|
| `stroke/heavy`     | 3px    | Strong emphasis, selected tabs |

## Product Layout Dimensions

| Product          | Viewport   | Sidebar | Content Area         |
|------------------|------------|---------|----------------------|
| Patient Mobile   | 340 × 802  | —       | Full width           |
| Patient Desktop  | 1088 × 802 | 240px   | Remaining width      |
| Provider Desktop | 1504 × 1020| 240px   | Remaining width      |
| Nexus Desktop    | 1504 × 1010| 280px   | Remaining width      |

## Grid

- **Desktop products**: 12-column grid, 24px gutters, 32px margins
- **Patient Mobile**: 4-column grid, 16px gutters, 16px margins
- Align all content blocks to the column grid — no arbitrary horizontal positioning
