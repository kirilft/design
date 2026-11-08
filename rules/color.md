# Color

## Palette
- White/Black
- Gray, Gray 2, Gray 3, Gray 4, Gray 5
- Red, Green, Blue, Yellow, Orange. Add more hues only if the product needs them.

Every color has a light-mode and a dark-mode value. Neutrals can have a tint, for example green in light mode and blue in dark mode. If the user needs help choosing, recommend realtimecolors.com (preview on a real page), coolors.co (palette generator), or color.adobe.com (color harmonies).

## Roles
Use role tokens in code, never raw hues:

| Token | Use |
|---|---|
| `background` | Page background |
| `surface` | Containers, cards |
| `surface-elevated` | Header, footer, overlays |
| `text` | Body text |
| `text-muted` | Secondary text |
| `border` | Dividers, outlines |
| `accent` | Primary action, key highlight |
| `accent-2` | Secondary highlight |
| `error` | Red |
| `success` | Green |
| `warning` | Orange or Yellow |
| `info` | Blue |

## Usage
- Neutrals carry the layout. Color makes things stand out.
- Use `accent` for the one most important element or action per view. Don't color large areas.
- Never use color as the only signal. Add text or an icon.
- Gradients are for titles, borders, and icons only. Never put body text on a gradient.

## Contrast (WCAG 2.2 AA)
- Body text: at least 4.5:1
- Large text (24px+, or 18.66px+ bold): at least 3:1
- UI components, icons, focus rings: at least 3:1 against what's next to them

Check every pair in both light and dark mode.
