# Layout

## Layers
Stack layers in this order, back to front:
1. Background (`background`)
2. Container (`surface`)
3. Header/Footer (`surface-elevated`)
4. Overlays above everything: cookie banner, modal, toast

In dark mode, higher layers are lighter. Glass layers follow [liquid-glass.md](liquid-glass.md).

## Spacing
- Law of proximity: space inside a group is smaller than space between groups.
- Define one spacing scale and use only its values. Set them in rem.
- Check layouts at mobile, tablet, and desktop widths.

## Corners
A squircle (continuous curvature) can't be built with CSS `border-radius`. `border-radius` draws circular arcs. Don't fake squircles with SVG masks or `clip-path`: they break borders, shadows, and `backdrop-filter`.

- **Web:** `border-radius` only.
- **Figma:** corner smoothing 60%.
- **iOS/macOS:** `RoundedRectangle(cornerRadius:style: .continuous)`.

- Define one radius per element type (container, button, input, badge). Use only those values.
- Nested radius = outer radius − gap between them.
- Fully round (`50%`) only for circles: avatars, round icon buttons.
