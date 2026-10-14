---
description: Re-orient on this repo, report state and next steps, then (with approval) create or refresh the project brief
---

Resume work on this project. Optional focus from the user: $ARGUMENTS

Follow the `bootstrap` skill's PROJECT.md template and rules.

1. **Orient (read-only).** Use the `explore` sub-agent if the repo is large. Gather:
   - `.kimi-code/PROJECT.md`, `AGENTS.md`, README (if present)
   - `git status -sb`, current branch, `git log -20 --oneline`, `git diff --stat`
   - build/test/run commands from the manifests (package.json, pyproject.toml, Cargo.toml, Makefile, ...)
   - `rg -n "TODO|FIXME|HACK" --max-count 30` (respect ignores)
   - what changed most recently (`git log -5 --stat --format='%h %s'`)
2. **Report** (max ~15 lines): what the project is, current state, in-flight work, risks, and the 3 best next steps. If a focus was given, rank steps by it.
3. **Propose specialisation.** List exactly what you would create or change: PROJECT.md (new or refreshed), AGENTS.md edits, and at most one project agent and one skill if clearly justified. Wait for approval before writing anything.
4. After approval, write the files, then run the project's test or build command once if it is cheap, and record the result under Status.
5. End by asking which next step to start.
