# Design

Design rules for AI agents building websites: color, typography, copy (English, German), components, layout, golden ratio, liquid glass, licensing, GDPR, accessibility, and tone of voice.

The agent uses them to build websites and to review existing ones: point it at a site and ask what's wrong, and it reports every rule the site breaks, with a fix.

`SKILL.md` is the entry point. It stays short and points to the files in `rules/`, which the agent reads only when it needs them.

## Use

**Claude Code**

```bash
git clone <repo-url> ~/.claude/skills/design
```

**Claude.ai:** download the repo as a ZIP and upload it under Settings → Capabilities → Skills.

**Any other chatbot:** paste the repo link or the contents of `SKILL.md` and tell it to follow the rules.
