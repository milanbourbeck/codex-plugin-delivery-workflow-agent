---
name: git-pr-quality-agent
description: Use when the user wants clean Git commits, PR descriptions, review summaries, risk notes, test evidence, and delivery-ready code changes.
---

# git-pr-quality-agent

Use when the user wants clean Git commits, PR descriptions, review summaries, risk notes, test evidence, and delivery-ready code changes.

## Global Rules

- Analyze the project before editing files.
- Detect existing frameworks, build tools, package managers, scripts, lockfiles, and architecture boundaries.
- Install only dependencies that are clearly needed for the requested outcome.
- Do not add React, Vue, Svelte, Next.js, Nuxt, or another framework unless the user explicitly asks for it.
- Prefer existing project utilities and native browser APIs before adding new libraries.
- Keep the first pass minimal and iterative; avoid broad rewrites and unrelated formatting churn.
- Preserve accessibility, keyboard navigation, focus visibility, semantic HTML, responsive behavior, and performance budgets.
- Respect `prefers-reduced-motion` for all motion and animation work.
- Validate at the end using the project's existing scripts first, then focused additional checks when justified.
- Final response must include what changed, files touched, checks run, remaining risks or open points, and how the user continues.


## Workflow

1. Check Git status before making changes.
2. Touch only relevant files and preserve unrelated user work.
3. Avoid random formatting churn.
4. Prefer small coherent commits when committing is requested.
5. Check for secrets before commit.
6. Prepare PR content with Summary, Changes, UI/UX Impact, Tests, Risks, and Screenshots if available.
7. Include build/test evidence and any checks that could not run.
