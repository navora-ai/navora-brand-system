# Accessibility

NAVORA targets **WCAG 2.1 Level AA** compliance.

## Color Contrast

### Minimum Ratios
| Context              | Ratio Required | Standard     |
|----------------------|----------------|--------------|  
| Body text            | 4.5:1          | WCAG 1.4.3   |
| Large text (≥24px)   | 3:1            | WCAG 1.4.3   |
| UI components        | 3:1            | WCAG 1.4.11  |
| Focus indicators     | 3:1            | WCAG 1.4.11  |

### Validated Pairings
| Foreground     | Background   | Ratio    | Pass |
|----------------|-------------|----------|------|
| Navy 900       | Ivory 50    | ~14.5:1  | AAA  |
| Ivory 50       | Navy 900    | ~14.5:1  | AAA  |
| Charcoal 700   | White       | ~7.2:1   | AAA  |
| Gold 600       | Ivory 50    | ~4.8:1   | AA   |
| Sage 500       | White       | ~4.1:1   | AA   |
| Red 500        | White       | ~4.3:1   | AA   |

### Color Independence
- Never encode information with color alone
- Status indicators combine color + text label + optional icon

## Typography
- Minimum font size: 11px (Label/S, Data/S)
- Default readable size: 16px (Body/M)
- Line height ≥ 1.4× for body text

## Touch Targets
- Minimum tap target: 44×44px
- If the visible element is smaller, the touch area must extend to 44px

## Focus Indicators
- Focus ring: 3px Gold spread
- Must be visible on all interactive elements via keyboard

## Keyboard Navigation
- All interactive elements reachable via Tab
- Logical tab order follows visual layout
- Enter/Space for activation, Escape for dismissal

## Screen Reader Support
- All images have descriptive alt text
- Icons as buttons have aria-label describing the action
- Form inputs have associated label elements
- Status changes announced via aria-live regions

## Motion
- Respect prefers-reduced-motion
- Transitions ≤ 200ms for UI state changes

## Clinical-Specific
- Patient-facing: minimum Body/L (18px)
- Clinical values: always in Data/M monospace, never truncated
- Medication names: never abbreviated without tooltip
- Dates: unambiguous format (08 Sep 2026)
- Color-blind safety: Red vs. Sage plus text labels
