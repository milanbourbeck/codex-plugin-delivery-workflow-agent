# Delivery Workflow Agent Instructions

## Repository Focus

- Maintain the @ship plugin for Git hygiene, PR quality, safe dependency changes, delivery summaries, risk notes, and test evidence.
- Prefer small, focused commits.
- Do not include secrets.
- Preserve unrelated user changes.

## Quality Priorities

- PR summaries should include what changed, why, UI/UX impact, accessibility, performance, checks, risks, and screenshots when available.
- Dependency guidance should respect package managers, lockfiles, existing tools, and bundle impact.
- End-to-end orchestration should coordinate design, build, QA, polish, and delivery without overinstalling dependencies.
- Risk notes should be concrete and tied to files, checks, or unknowns.

## Validation

- Keep .codex-plugin/plugin.json valid with canonical handle @ship.
- Keep skill folders and frontmatter names aligned: $pr, $e2e, $deps.
- Run scripts/validate-plugin.mjs when possible.
