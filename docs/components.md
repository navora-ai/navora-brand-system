# Component System

## Token Mapping

Every component references semantic tokens through a component-level alias layer.

```
Primitive (raw)  →  Semantic (intent)  →  Component (specific)
#08233A             surface/inverse        button/primary/bg
```

## Component Token Prefixes

| Prefix    | Components                                  |
|-----------|---------------------------------------------|
| `button/` | Primary, Secondary, Quiet, Focus, Disabled  |
| `card/`   | Default, Evidence, Waiting                  |
| `tag/`    | Neutral, Evidence, Verified, Safety         |
| `nav/`    | Default, Active                             |
| `input/`  | Default, Focus, Error, Disabled             |
| `status/` | New, Waiting, Action, Verified, Safety, Conflict |

## Button Variants

### Primary (CTA)
- Background: `button/primary/bg` → Navy 900 (Light) / Ivory 50 (Dark)
- Text: `button/primary/text` → Ivory 50 (Light) / Navy 900 (Dark)
- Use for: primary actions — "Submit", "Save", "Confirm"

### Secondary
- Background: `button/secondary/bg` → White (Light) / Navy 800 (Dark)
- Border: `button/secondary/border` → Stone 300 (Light) / Navy 700 (Dark)
- Use for: secondary actions — "Cancel", "Back", "Edit"

### Quiet
- Background: transparent (matches canvas)
- Use for: tertiary actions, inline text buttons

### States
- **Focus**: Gold ring (3px spread)
- **Disabled**: Subtle bg + subtle text

## Card Variants

- **Default**: White background, subtle border, card elevation shadow
- **Evidence**: Ivory-tinted background + gold border — exclusive for citations

## Tags

- `tag/neutral` — general categorization
- `tag/evidence` — evidence-related labels
- `tag/verified` — clinically verified (sage text)
- `tag/safety` — safety-critical (red text)

## Navigation

- Sidebar: Navy 900 background, ivory text
- Desktop sidebar width: 240px (Patient/Provider), 280px (Nexus)

## Status Indicators

| Status     | Text Color        | Background          |
|------------|-------------------|---------------------|
| New        | Blue `#6E8FAE`    | Subtle surface      |
| Waiting    | Stone `#8A8F98`   | Subtle surface      |
| Action     | Gold Dark `#A9791F`| Subtle surface      |
| Verified   | Sage `#668A7A`    | Subtle surface      |
| Safety     | Red `#B65353`     | Subtle surface      |
| Conflict   | Red `#B65353`     | Subtle surface      |

## Icon Library

25 custom icons (8 generic + 17 clinical domain-specific).
