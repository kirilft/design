# Typography

## Fonts
- Use at most 2 fonts: 1 title font and 1 content font.
- The title font is for display text: page title, hero, website section headings. Use it sparingly. If every heading uses it, it stops standing out.
- Everything else uses the content font: article headings (H1–H5 in long text), body text, navigation, buttons, labels.
- Default content font: Inter. Use it when the user gives no font.
- Find fonts on Google Fonts (fonts.google.com), Fontshare (fontshare.com), or Bunny Fonts (fonts.bunny.net).
- Self-host fonts (see [gdpr.md](gdpr.md)).
- Use WOFF2 files.
- Set `font-display: swap;` in every `@font-face`.
- Set all font sizes in `rem`.
- The font must contain every character the site uses: special characters of the language (ä, ö, ü, ß, „ “, –, —) and every weight and style used (bold, italic). If the site uses emoji, the font must contain them.
- No fake bold or italic (`font-synthesis: none;`).
- Use at most 3 weights. Weights follow the golden ratio (see [golden-ratio.md](golden-ratio.md)).
- Fonts and icons follow [licensing.md](licensing.md).

## Base CSS
```css
html {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  -webkit-text-size-adjust: 100%;
  text-size-adjust: 100%;
  font-variant-numeric: proportional-nums;
  text-rendering: optimizeLegibility;
  font-synthesis: none;
}
table, .price, .timer, .counter {
  font-variant-numeric: tabular-nums;
}
```
Use `tabular-nums` for tables, prices, timers, counters, and any numbers that change or line up in columns.

## Scale
There are two heading sets:
- **Website headings** (sections, hero): golden ratio, built from Fibonacci numbers (see [golden-ratio.md](golden-ratio.md))
- **Text headings** (articles, long text): half steps of the golden ratio (see [golden-ratio.md](golden-ratio.md))

Website text is bigger than article text for readability. Body text is at least 1rem (16px).

## Setting text
- Line length: 45–75 characters. Use `max-width: 65ch` on text blocks.
- Line height: 1.5 for body text, 1.1–1.25 for headings.
- Align text left. Never justify. Center only short text (3 lines or fewer).
- Headings use `text-wrap: balance;`, paragraphs use `text-wrap: pretty;`.
- No all caps for sentences. Short labels in all caps get `letter-spacing: 0.05em`.
- Underline links only.
