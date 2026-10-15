# Project Bootstrap for Kimi Code

[![Release](https://img.shields.io/github/v/release/Quattro-Commas/project-bootstrap)](https://github.com/Quattro-Commas/project-bootstrap/releases/latest)

A Kimi Code plugin that helps every session start oriented.

It adds a `bootstrap` skill that runs at session start to classify the current directory, plus three slash commands for managing project memory:

- `/project-bootstrap:resume` — re-orient on an existing repo and refresh `.kimi-code/PROJECT.md`
- `/project-bootstrap:newproject <idea>` — scope and scaffold a new project
- `/project-bootstrap:wrapup` — update `PROJECT.md` status, decisions, and next steps at the end of a session

It also includes skills for planning monetization, go-to-market, and pricing for devtools and plugins.

## Install

In Kimi Code, run:

```
/plugins install https://github.com/Quattro-Commas/project-bootstrap
```

Then run `/reload` or start a new session.

## Quick start

Open any project folder and the `bootstrap` skill will orient the session automatically.

To update project memory by hand:

```
/project-bootstrap:resume
```

To plan a new project:

```
/project-bootstrap:newproject "a CLI that turns JSON into SQL"
```

To wrap up a session:

```
/project-bootstrap:wrapup
```

## Privacy and security

- All memory stays local in `.kimi-code/PROJECT.md` inside each repo.
- The plugin makes no network requests and collects no telemetry.
- See [SECURITY.md](./SECURITY.md) for how to report vulnerabilities.

## Supported versions

Tested with Kimi Code CLI 2.2.0.

## License

MIT
