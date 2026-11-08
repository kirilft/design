# Accessibility

Follow WCAG 2.2 AA.

- Contrast: see [color.md](color.md).
- Text size: set in rem. The page works when text is enlarged to 200%.
- Focus: every interactive element has a visible focus indicator (`:focus-visible`), at least 3:1 contrast.
- Touch targets: at least 44×44px, at least 8px apart.
- Keyboard: everything works with the keyboard alone, in a logical order.
- Semantic HTML: use `header`, `nav`, `main`, `footer`, `button`, `a`, and headings in order (H1 → H2 → H3). One H1 per page.
- ARIA: only where HTML has no element for it. Icon-only buttons get an `aria-label`.
- Images: meaningful images get `alt` text. Decorative images get `alt=""`.
- Errors: say what went wrong and how to fix it, next to the field.
- Motion: respect `prefers-reduced-motion`.
