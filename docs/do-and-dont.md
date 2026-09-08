# Do & Don't

Quick visual reference for the most common brand application decisions.

---

## Color

| Do | Don't |
|----|-------|
| Use Navy as the dominant color (65–70%) | Use Gold or Red as dominant brand color |
| Reserve Gold exclusively for evidence markers | Use Gold for buttons, backgrounds, or decoration |
| Use semantic tokens (`surface/card`) in code | Hardcode hex values (`#FFFFFF`) directly |
| Ensure all text meets WCAG AA contrast (4.5:1) | Place light text on light backgrounds |

## Typography

| Do | Don't |
|----|-------|
| Use Newsreader for Display and Heading only | Use Newsreader for body text or labels |
| Use Inter for all UI text and paragraphs | Use a fourth typeface "for variety" |
| Use IBM Plex Mono for clinical data values | Use monospace for headings or decoration |
| Maintain the defined type scale (11–64px) | Invent custom sizes (e.g., 15px, 22px, 37px) |

## Layout & Spacing

| Do | Don't |
|----|-------|
| Use 4px-based spacing tokens exclusively | Use arbitrary values like 5px, 7px, 15px |
| Maintain consistent padding within containers | Mix different paddings in sibling cards |
| Reduce border-radius on nested elements | Use the same radius on parent and child |
| Ensure 44px minimum touch targets | Make tiny tap targets (< 44px) |

## Logo

| Do | Don't |
|----|-------|
| Use provided SVG files unchanged | Recreate or redraw the logo |
| Maintain clear space (1× glyph height) | Crowd the logo with other elements |
| Use Navy logo on light, Ivory on dark | Use off-brand colors for the logo |
| Scale proportionally | Stretch, skew, or rotate the logo |

## Components

| Do | Don't |
|----|-------|
| Use component tokens (`button/primary/bg`) | Reference semantic tokens directly in components |
| Apply the Evidence Card for citations only | Use the gold-bordered card for general content |
| Use defined status colors (Sage, Blue, Gold, Red) | Invent new status colors |
| Build with existing components first | Duplicate a component and modify locally |

## Content & Copy

| Do | Don't |
|----|-------|
| Use Title Case for headers and buttons | Use ALL CAPS in running text |
| Write error messages with cause + action | Show raw error codes ("Error 401") |
| Use unambiguous date format (08 Sep 2026) | Use locale-dependent formats (09/08/26) |
| Display clinical values with units and reference | Show bare numbers without context |

## Accessibility

| Do | Don't |
|----|-------|
| Pair color with text labels for status | Encode meaning with color alone |
| Provide alt text for all meaningful images | Use "image" or file names as alt text |
| Support keyboard navigation for all controls | Make elements only accessible via mouse |
| Use the Gold focus ring on all focusable elements | Remove or hide focus indicators |

## Dark Mode

| Do | Don't |
|----|-------|
| Use semantic tokens that auto-switch | Manually override colors per mode |
| Test both modes for contrast compliance | Design only in Light mode |
| Use Navy 800 for elevated surfaces in dark | Use pure black (#000000) |
| Keep Gold evidence markers the same in both | Lighten or brighten Gold in Dark mode |
