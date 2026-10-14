---
name: monetization-strategy
description: Plan a sustainable revenue model for a developer tool, plugin, or AI agent extension without locking out solo users.
---

# Monetization strategy for devtools and plugins

Use this when the user wants to turn a Kimi Code plugin, CLI tool, agent skill, or other developer-facing product into a paid or sponsored offering.

## Principles

- Default to generosity. A free tier that solves real problems builds trust and word-of-mouth.
- Charge for things that scale with value: teams, usage, automation, governance, or support — not for basic access.
- Keep self-hosting and local-first options open unless there is a strong, disclosed reason not to.
- Never promise revenue. Produce models, pricing drafts, and a launch experiment plan.

## Workflow

1. **Clarify the asset.** What exactly is being sold? (plugin, skill, SaaS wrapper, support contract, audit service, training, hosted fleet)
2. **Map value to user type.**
   - Solo developer / hobbyist
   - Small team (2–10)
   - Enterprise (compliance, SSO, audit logs, dedicated support)
3. **Choose a model.** Pick one primary and one secondary:
   - Open source + sponsored/paid support
   - Dual license (AGPL/proprietary)
   - Freemium (free tier + paid seats or usage)
   - Usage-based (API calls, compute, storage)
   - Marketplace revenue share
   - Consulting / implementation services
4. **Draft a pricing ladder.** For each tier list: who, what they get, price anchor, limit, and upgrade trigger.
5. **Identify risks.** Common ones: dependency on a host platform (Kimi, Claude, Codex), copying, support load, tax/jurisdiction complexity, enterprise sales cycle.
6. **Define the launch experiment.** Pick one metric, one channel, one offer, and a 30-day check.

## Output format

Return a concise plan:

```markdown
# Monetization plan: <product name>

## Asset and primary model
<one paragraph>

## Pricing ladder
| Tier | Who | Price | Includes | Limit | Upgrade trigger |
| --- | --- | --- | --- | --- | --- |

## Risks and mitigations
- Risk: ... Mitigation: ...

## 30-day experiment
- Metric:
- Channel:
- Offer:
- Success threshold:
```

Keep the whole output under 60 lines unless the user asks for detail.
