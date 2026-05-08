---
name: e2e
description: Orchestrate frontend work from idea to implementation, QA, polish, and PR-ready delivery.
---

# e2e

Use when the user wants Codex to take a frontend task from idea to implemented, tested, audited, polished, and PR-ready delivery. This skill coordinates other installed skills but must avoid installing unnecessary dependencies.

## Handle Migration

Canonical skill handle: `$e2e`. Legacy internal name: `end-to-end-project-orchestrator -> e2e`.

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

1. Interpret the task and define the smallest useful delivery slice.
2. Analyze project architecture, scripts, dependencies, and active changes.
3. Choose only relevant skills: premium HTML integration, design system work, frontend audit, visual QA, accessibility, performance, or PR delivery.
4. Create a plan for substantial work.
5. Execute in phases and validate after each large phase.
6. Split scope when the work grows beyond a coherent delivery unit.
7. Finish with changed files, checks, risks, and next actions.
