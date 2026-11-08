# Licensing

A website ships its code, fonts, and icons to every visitor's browser. That counts as distributing them, so their license notices must ship too.

## What to check
- Check the license of every framework, library, font, icon set, and image before using it. It must allow use on a website.
- Tell the user which license applies to each asset and what it requires.
- List everything the browser downloads: framework (Angular, React, Vue), runtime libraries (RxJS, zone.js, tslib), fonts, icon sets, images, data.
- Build tools that never reach the browser (TypeScript compiler, bundler, linter) don't need a notice on the site.

## Common licenses
| License | Examples | Requires |
|---|---|---|
| MIT | Angular, React, Vue | Copyright notice + license text |
| Apache-2.0 | RxJS, Material Symbols | License text + any NOTICE file |
| SIL OFL 1.1 | Most Google Fonts, Inter, Outfit | License text with the font files. Don't sell the font alone |
| CC BY 4.0 | Font Awesome Free icons | Visible credit to the author |
| 0BSD | tslib | Nothing |
| Unsplash, Pexels | Stock photos | Nothing required. Credit is optional |
| Apple fonts and SF Symbols | SF Pro | Not allowed on websites. Apple platforms only |

## Where to put it
1. **Licenses page:** linked from the footer of every page. One entry per asset: name, use (framework, font, icons), license, link to the license text, copyright holder.
2. **Source:** keep the same list as a comment in `index.html` and the license files next to self-hosted fonts.
3. **Generated file:** if the build tool creates one (Angular CLI: `3rdpartylicenses.txt`), publish it and link it from the Licenses page.

Entry format:
```
Outfit (font) — SIL Open Font License 1.1 — https://openfontlicense.org — © The Outfit Project Authors
```

## Your own work
State the license of the site's own code and content, with copyright year and holder (for example `© 2026 Name. Code: MIT`).
