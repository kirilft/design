# Liquid glass

Liquid glass bends light. It does not blur.

- **Refraction:** the glass shifts the background behind it like a convex lens. The shift is strongest at the edge and zero in the center. Content behind the glass stays sharp.
- **No blur:** never use `backdrop-filter: blur()` to create glass. That's frosted glass, a different material.
- **Rim light:** the edge facing the light (top-left) gets a light highlight. The opposite edge gets a darker one.
- **Dispersion:** at the edge, red, green, and blue shift by slightly different amounts. Keep it subtle.
- **Tint:** a low-opacity tint from the theme: light tint in light mode, dark tint in dark mode.
- **Shape:** radii from [layout.md](layout.md), with an even rim thickness all around.
- **Where:** only on layers above content (header, navigation, controls, overlays). Never on content itself. Never glass on glass.
- **Legibility:** text on glass meets the contrast values in [color.md](color.md), over every background it can scroll over. Raise the tint opacity until it does.

Implementation on the web:
1. Build an SVG `<filter>` with a displacement map for the shape (`feImage` + `feDisplacementMap`). Displacement grows toward the edge.
2. Apply it with `backdrop-filter: url(#glass);`. Only Chromium browsers support SVG filters in `backdrop-filter`.
3. Add the rim light with inset `box-shadow` or a masked gradient border.
4. Feature-detect. Other browsers get a fallback: the tint plus the rim light, no refraction, no blur.
