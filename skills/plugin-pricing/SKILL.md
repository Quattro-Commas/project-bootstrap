---
name: plugin-pricing
description: Draft a pricing page and tier structure for a Kimi Code plugin or devtool, anchored to value and support cost.
---

# Plugin pricing

Use this when the user needs concrete prices and a pricing-page draft for a plugin or devtool.

## Anchors

- **Free:** enough for a solo developer to get recurring value and tell others.
- **Pro / Team:** paid per seat or per workspace; unlocks collaboration, shared memory, or higher limits.
- **Enterprise:** paid annually; unlocks SSO, audit logs, priority support, custom terms.

## Rules

- Show annual and monthly prices. Annual is usually 10× monthly, not 12×.
- List limits as concrete numbers (projects, seats, invocations, storage).
- Put the most popular tier in the middle and visually highlight it.
- Include a "Compare all features" table only if it stays under 10 rows.
- Always note what happens at a limit (hard stop vs pay-as-you-go).

## Pricing-page template

```markdown
# Pricing

## Free
$0 forever
- <limit 1>
- <limit 2>
- Community support

## Pro — $X/month or $Y/year
- Everything in Free
- <paid feature 1>
- <paid feature 2>
- Email support

## Enterprise — contact sales
- Everything in Pro
- SSO / SAML
- Audit logs
- Dedicated support
```

Ask the user for their cost assumptions and desired average revenue per user before finalizing numbers.
