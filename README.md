# Project Bootstrap for Kimi Code

A Kimi Code plugin that helps every session start oriented.

It adds a `bootstrap` skill that runs at session start to classify the current directory, plus three slash commands for managing project memory:

- `/project-bootstrap:resume` — re-orient on an existing repo and refresh `.kimi-code/PROJECT.md`
- `/project-bootstrap:newproject <idea>` — scope and scaffold a new project
- `/project-bootstrap:wrapup` — update `PROJECT.md` status, decisions, and next steps at the end of a session

It also includes skills for planning monetization, go-to-market, and pricing for devtools and plugins.

## Install

```
/plugins install https://github.com/Quattro-Commas/project-bootstrap
```

Then run `/reload` or start a new session.

## Supported versions

Tested with Kimi Code CLI 2.2.0.

## License

MIT
