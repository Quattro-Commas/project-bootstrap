---
name: plugin-go-to-market
description: Launch and distribute a Kimi Code plugin: README, marketplace listing, install instructions, and first-week promotion.
---

# Plugin go-to-market for Kimi Code

Use this when a plugin is ready to share and the user wants users to discover, install, and trust it.

## Launch checklist

1. **README essentials** (keep under 120 lines)
   - One-sentence value proposition
   - Animated GIF or static screenshot of a slash command in action
   - Install command: `/plugins install <github-url>`
   - Quick-start example
   - Supported CLI versions
   - License and contribution note
2. **Marketplace entry**
   - If submitting to a marketplace, include `kimi.plugin.json` fields: `interface.displayName`, `shortDescription`, `longDescription`, `developerName`, `websiteURL`, `keywords`.
   - Provide a 512×512 icon if the marketplace requires one.
3. **Trust signals**
   - Changelog
   - Version tags
   - CI status badge
   - Security / data-privacy statement (no remote calls, no telemetry, etc.)
4. **Distribution channels**
   - Kimi Code `/plugins install <repo-url>`
   - GitHub releases with attached zip
   - Personal or org blog / social post
   - Relevant Discord/Slack/Reddit communities (no spam; disclose authorship)
5. **First-week metrics**
   - Installs
   - Enabled vs installed ratio
   - Slash command invocations (if observable)
   - Issues opened

## Pitch template

```markdown
<I built> <plugin name> because <specific pain>.

It adds <commands/skills> to Kimi Code so you can <outcome>.

Install: `/plugins install <url>`
Repo: <url>
```

Use this to draft the launch post. Ask the user which channels they want to target before posting anything.
