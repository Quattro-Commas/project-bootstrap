# 30-day launch experiment

## Goal

Validate that developers find Project Bootstrap useful enough to install and that teams are interested in a future Pro tier.

## Dates

- Start: 2026-10-15
- End: 2026-11-14

## Metrics

| Metric | Source | Target |
| ------ | ------ | ------ |
| Installs | GitHub release download count on `v1.0.0` | ≥ 50 |
| Waitlist sign-ups | Reactions + comments on [Pro waitlist discussion](https://github.com/Quattro-Commas/project-bootstrap/discussions/7) | ≥ 20 |
| Stars | GitHub repo stars | ≥ 10 |
| Issues / feedback | GitHub issues | any, with labels |

## How to measure

Installs (release asset downloads):

```bash
GH_CONFIG_DIR=$HOME/.config/gh-codespace gh release view v1.0.0 --repo Quattro-Commas/project-bootstrap --json assets
```

Waitlist sign-ups (discussion engagement):

```bash
GH_CONFIG_DIR=$HOME/.config/gh-codespace gh api repos/Quattro-Commas/project-bootstrap/discussions/7 --jq '{reactions: .reactions.total_count, comments: .comments.totalCount}'
```

Stars:

```bash
GH_CONFIG_DIR=$HOME/.config/gh-codespace gh repo view Quattro-Commas/project-bootstrap --json stargazerCount
```

## Success

- If installs ≥ 50 and waitlist ≥ 20: proceed to design the hosted-service MVP and open a paid pilot.
- If installs ≥ 50 but waitlist < 20: keep the plugin free and refine the Pro pitch before building.
- If installs < 50: review distribution channels and README clarity, then run a second experiment.

## Baseline (2026-10-15)

| Metric | Value |
| ------ | ----- |
| Installs (release downloads) | 1 |
| Waitlist sign-ups | 0 |
| Stars | 0 |

## Week 0 check (2026-10-15)

| Metric | Value | Notes |
| ------ | ----- | ----- |
| Installs (release downloads) | 1 | Internal test/verification download |
| Waitlist sign-ups | 0 | Discussion created, no organic reach yet |
| Stars | 0 | Repo announcement just posted |

## Week 1 check (2026-10-18)

| Metric | Value | Notes |
| ------ | ----- | ----- |
| Installs (release downloads) | 2 | One additional download; likely the reinstall test from 2026-10-15 |
| Waitlist sign-ups | 0 | Still no organic reach |
| Stars | 0 | No stars yet |

## Channels

- Kimi Code community spaces
- Personal / Quattro-Commas social channels
- Relevant developer communities (no spam; disclose authorship)
