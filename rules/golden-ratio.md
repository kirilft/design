# Golden ratio

The golden ratio (1.6180339…) is irrational. No pixel value hits it exactly. Use Fibonacci numbers instead (1, 2, 3, 5, 8, 13, 21, 34, 55): they are whole numbers, and the ratio between neighbors approaches 1.618.

- **Type scale:** Fibonacci numbers × 2 put the scale on 16px. Fibonacci numbers themselves fill the half steps in between.

  | Steps | Values (px) | Ratio |
  |---|---|---|
  | Full steps (website headings) | 10, 16, 26, 42, 68, 110 | ≈ 1.618 |
  | Half steps (text headings) | 13, 16, 21, 26, 34, 42 | ≈ 1.27 |

  Set them in rem (px ÷ 16). Assign H1–H5 from the largest step down. Values below 16px are for labels only, never for running text.
- **Font weight:** weights come in steps of 100. Pair them with Fibonacci numbers: 300 + 500 (3 : 5) or 500 + 800 (5 : 8).
- **Not for spacing or corners.** Those use fixed values (see [layout.md](layout.md)).
