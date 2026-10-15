# Hosted-service MVP scope

This document defines the minimum viable hosted companion service for Project Bootstrap. The core plugin remains local, open-source, and free. The hosted service is the paid Pro/Enterprise layer.

## Problem

Solo users can keep `.kimi-code/PROJECT.md` and `AGENTS.md` files in each repo, but teams need:

- Shared project memory across repos in an org.
- Consistent org-wide conventions that propagate to every project.
- Basic usage analytics so team leads can see adoption.

## MVP scope

1. **Shared project memory**
   - Sync `.kimi-code/PROJECT.md` files to a per-team workspace.
   - Read-only sync from the plugin; writes stay local by default.
   - Optional two-way sync for team-owned conventions.

2. **Org-wide conventions**
   - A team-level `AGENTS.md` template that new projects can inherit.
   - Versioned convention updates with a changelog.

3. **Basic analytics**
   - Number of active projects using the plugin.
   - Slash-command invocation counts (anonymized, aggregated).
   - Seat count per workspace.

## Out of scope for MVP

- SSO/SAML (Enterprise v2).
- Audit logs (Enterprise v2).
- Custom agents or skills (Enterprise v2).
- On-prem deployment (Enterprise v2).
- Real-time collaboration / locking.

## Architecture sketch

- Backend: stateless API + database per workspace.
- Auth: GitHub OAuth, scoped to org membership.
- Plugin: opt-in sync via a new `/project-bootstrap:sync` command.
- Hosting: start with a single small VM or container; scale only after paid demand.

## Success criteria

- 5 teams on the Pro waitlist are willing to run a paid pilot.
- Pilot users can sync at least one project and one org convention within one hour of signup.
- No unplanned downtime during the 30-day pilot.
