# Reviewing a website

Use this when the user points you at an existing website (code, URL, or screenshots) and asks what's wrong.

## How
1. Read every file in `rules/`.
2. Look at the rendered page at mobile, tablet, and desktop widths, in light and dark mode. Read the code for values (colors, sizes, fonts, spacing).
3. Check the page against every rule. Then check the points below.
4. Report every violation. Don't fix anything until the user says so.

## Also check
- **First impression:** what draws the eye first? It must be the most important element. The purpose of the page is clear within 2 seconds.
- **Hierarchy:** there is one clear reading order. Size, weight, and color emphasize the right things and nothing else.
- **Usability:** navigation is obvious. Interactive elements look interactive. No unnecessary steps.
- **Consistency:** the same element looks and behaves the same everywhere. No one-off colors, sizes, spacing, or radii.

## Report format

### Findings
| # | Where | Problem | Rule | Severity | Fix |
|---|---|---|---|---|---|
| 1 | Hero heading | Uses the title font for all 6 headings | typography.md: title font sparingly | 🟡 Moderate | Keep it on the hero only, content font elsewhere |

Severity:
- 🔴 Critical: breaks accessibility or blocks the user.
- 🟡 Moderate: breaks a rule visibly.
- 🟢 Minor: polish.

### What works
List what already follows the rules.

### Priorities
The 3 changes with the biggest effect, in order.
