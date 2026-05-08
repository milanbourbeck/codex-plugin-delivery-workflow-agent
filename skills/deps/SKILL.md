---
name: deps
description: Manage frontend dependencies safely and avoid unnecessary packages.
---

# deps

Use when the user wants to add, remove, update, or rationalize frontend dependencies safely.

## Handle Migration

Canonical skill handle: `$deps`. Legacy internal name: `safe-dependency-manager -> deps`.

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

1. Inspect `package.json`, lockfiles, imports, build tooling, and package manager.
2. Detect redundant libraries, conflicting tools, unneeded UI stacks, and bundle-cost risks.
3. Add dependencies only when the project need is clear.
4. Respect the existing lockfile and package manager.
5. Run install/build checks when possible.
6. Suggest no-dependency alternatives when a package is unnecessary.
