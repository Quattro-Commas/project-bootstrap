---
description: Scope a new idea, then (with approval) scaffold the repo, project brief, AGENTS.md and a first milestone
---

Start a new project from this idea: $ARGUMENTS

Follow the `bootstrap` skill's PROJECT.md template and rules.

1. **Clarify in one message.** Ask at most 5 short questions, numbered, with a suggested default for each: who it is for, the core outcome, platform/stack, hard constraints (budget, offline, device, deadline), and what "done for v1" means. If the user already answered some in the idea, skip those. Wait for answers.
2. **Plan (no writes yet).** Present: one-paragraph scope, stack choice with one-line reasons, directory layout, a first milestone that can be demoed in one sitting, and 3 main risks. Keep it under ~30 lines. Wait for approval or edits.
3. **Scaffold after approval:**
   - `git init` if needed, `.gitignore` suited to the stack
   - minimal working skeleton plus one passing test or smoke check
   - `.kimi-code/PROJECT.md` filled from the plan (phase: prototype)
   - `AGENTS.md` with build/test/run commands and conventions
   - optional `.kimi-code/agents/<project>-dev.md` only if the stack has strong conventions to encode
4. Run the smoke check, fix what fails, then make one initial commit.
5. Finish with the first three tasks of the milestone and ask which to start.
