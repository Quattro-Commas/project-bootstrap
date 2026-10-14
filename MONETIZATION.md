# Monetization plan: Project Bootstrap for Kimi Code

## Asset and primary model

Project Bootstrap is a Kimi Code plugin that orients every session: it classifies the current directory, offers the right next step, and provides slash commands for resuming projects, scaffolding new ones, and wrapping up sessions.

Primary model: **open-source plugin + freemium team/enterprise tier**.
- The core plugin and all skills remain free and open-source under MIT.
- Revenue comes from a future cloud-hosted companion service that adds team-shared project memory, org-wide conventions, and usage analytics.
- Secondary revenue: paid support, implementation consulting, and white-glove onboarding for enterprises.

## Pricing ladder

| Tier | Who | Price | Includes | Limit | Upgrade trigger |
| --- | --- | --- | --- | --- | --- |
| **Free** | Solo developers, open-source maintainers | $0 | All plugin skills and slash commands; local `.kimi-code/PROJECT.md` | One user, local-only memory | Needs shared team memory or SSO |
| **Pro** | Small teams (2–20) | $8/seat/month or $80/seat/year | Shared project memory, team conventions, basic usage analytics, priority email support | 20 seats | Needs SSO, audit logs, or custom terms |
| **Enterprise** | Engineering orgs (21+) | Custom annual contract | SSO/SAML, audit logs, custom agents/skills, dedicated support, SLAs, on-prem option | Negotiated | Procurement / compliance requirements |

## Risks and mitigations

- **Platform dependency.** Kimi Code CLI controls plugin loading, marketplace, and slash-command syntax. *Mitigation:* keep the plugin strictly within documented APIs; build an email list and GitHub community independent of any one marketplace.
- **Copying.** The core is MIT-licensed and easy to fork. *Mitigation:* monetize the hosted service, not the local plugin; offer value through sync, governance, and support.
- **Support load.** Free users may open many issues. *Mitigation:* route free users to GitHub Discussions; reserve email support for Pro/Enterprise.
- **Enterprise sales cycle.** Long procurement. *Mitigation:* offer self-serve Pro with credit-card billing; Enterprise is inbound-only with a simple contact form.

## 30-day experiment

- **Metric:** GitHub stars + `/plugins install` invocations tracked by release downloads.
- **Channel:** Launch post on the Kimi Code community spaces and the user's personal/Quattro-Commas channels.
- **Offer:** "Install Project Bootstrap free; join the waitlist for team shared memory."
- **Success threshold:** 50 installs and 20 waitlist sign-ups in 30 days.

## Pricing page draft

```markdown
# Pricing

## Free
$0 forever
- All slash commands (`resume`, `newproject`, `wrapup`)
- All skills (bootstrap, monetization-strategy, plugin-go-to-market, plugin-pricing)
- Local `.kimi-code/PROJECT.md` memory
- GitHub Discussions support

## Pro — $8/seat/month or $80/seat/year
- Everything in Free
- Shared team project memory
- Org-wide convention syncing
- Basic usage analytics
- Priority email support

## Enterprise — contact sales
- Everything in Pro
- SSO / SAML
- Audit logs
- Custom agents and skills
- Dedicated support and SLAs
```

## Launch plan

1. Merge this monetization plan into the repo.
2. Add a `CHANGELOG.md` and tag `v1.0.0`.
3. Publish a release with the plugin zip attached.
4. Post the install command (`/plugins install https://github.com/Quattro-Commas/project-bootstrap`) to relevant communities.
5. Add a waitlist link for Pro/Enterprise in the README.
