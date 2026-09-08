# Typography

## Font Stack

| Role      | Family           | Source                                         |
|-----------|------------------|------------------------------------------------|
| Display   | **Newsreader**   | [Google Fonts](https://fonts.google.com/specimen/Newsreader) |
| Body      | **Inter**        | [rsms.me/inter](https://rsms.me/inter/)       |
| Data      | **IBM Plex Mono**| [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Mono) |

### Fallbacks
```css
--font-display: 'Newsreader', Georgia, 'Times New Roman', serif;
--font-body:    'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
--font-data:    'IBM Plex Mono', 'SF Mono', 'Fira Code', 'Consolas', monospace;
```

## Type Scale

### Display (Newsreader Medium)
| Token        | Size  | Line Height | Letter Spacing | Usage                    |
|--------------|-------|-------------|----------------|--------------------------|  
| Display/XL   | 64px  | 72px        | -1.2px         | Hero headlines           |
| Display/L    | 48px  | 56px        | -0.6px         | Section titles           |

### Heading (Newsreader Medium)
| Token        | Size  | Line Height | Letter Spacing | Usage                    |
|--------------|-------|-------------|----------------|--------------------------|  
| Heading/H1   | 40px  | 48px        | -0.4px         | Page titles              |
| Heading/H2   | 32px  | 40px        | -0.2px         | Section headers          |
| Heading/H3   | 24px  | 32px        | 0              | Subsection headers       |

### Body (Inter Regular)
| Token        | Size  | Line Height | Letter Spacing | Usage                    |
|--------------|-------|-------------|----------------|--------------------------|  
| Body/L       | 18px  | 28px        | 0              | Long-form reading        |
| Body/M       | 16px  | 24px        | 0              | Default UI text          |
| Body/S       | 14px  | 20px        | 0              | Secondary content        |

### Label (Inter Semi Bold / Medium)
| Token        | Size  | Line Height | Letter Spacing | Weight    | Usage               |
|--------------|-------|-------------|----------------|-----------|---------------------|
| Label/L      | 14px  | 20px        | 0.6px          | Semi Bold | Navigation, buttons |
| Label/M      | 12px  | 16px        | 0.8px          | Semi Bold | Tags, badges        |
| Label/S      | 11px  | 14px        | 1.1px          | Medium    | Overlines, captions |

### Data (IBM Plex Mono Regular)
| Token        | Size  | Line Height | Letter Spacing | Usage                    |
|--------------|-------|-------------|----------------|--------------------------|  
| Data/M       | 13px  | 18px        | 0              | Clinical values, IDs     |
| Data/S       | 11px  | 16px        | 0              | Timestamps, metadata     |

## Pairing Rules

1. **Newsreader is for headlines only** — never use it for body text, labels, or data
2. **Inter is the workhorse** — all UI text, paragraphs, labels, and interactive elements
3. **IBM Plex Mono is for clinical data only** — never use it for headings or decorative purposes
4. **Labels always have letter-spacing** — this distinguishes them from body text at the same size
5. **Never go below 11px** — minimum readable size for accessibility compliance

## Hierarchy Rules

- Each screen has **one** Display or H1 — never stack two equally weighted headings
- H2 always follows H1; H3 always follows H2 — no skipping levels
- Body text defaults to **Body/M** (16px); use Body/L (18px) only for long-form reading contexts
- Use color weight (primary vs. secondary) alongside size to reinforce hierarchy
