# Delivery Workflow Agent

## Purpose

Safe Git, PR, dependency, release, and end-to-end delivery workflows for Codex-driven frontend work.

## Included Skills

- `git-pr-quality-agent`
- `end-to-end-project-orchestrator`
- `safe-dependency-manager`

## When To Use

- The user wants delivery-ready commits or PR text.
- A frontend task should be taken from idea to tested delivery.
- Dependencies need to be added, removed, updated, or rationalized.

## When Not To Use

- No repository exists and the user only wants a conceptual answer.
- The task is a tiny single-file answer with no Git workflow.
- The user explicitly asks not to touch Git.

## Installation

Install this plugin from the Premium Codex Workflows marketplace, or add this repository directly as a Git-backed plugin source.

Repository: `https://github.com/milanbourbeck/codex-plugin-delivery-workflow-agent.git`

## Example Prompts

- `@premium-html-uiux integriere den Premium HTML UI/UX Stack in dieses Vanilla HTML Projekt. Installiere nur, was wirklich gebraucht wird.`
- `$modernize-existing-html-ui analysiere diese Website und verbessere UI, Responsiveness, Semantik und Fokuszustände minimal-invasiv.`
- `$visual-qa-playwright prüfe die Seite in Desktop, Tablet und Mobile, dokumentiere Layout-Probleme und behebe die wichtigsten.`
- `$accessibility-optimizer prüfe Navigation, Formulare, Dialoge, Fokuszustände und reduced-motion.`
- `$performance-optimizer finde unnötige Bundle-Kosten, Bildprobleme, Layout Shifts und schwere Animationen.`
- `$build-design-system-foundation erstelle eine konsistente Designsystem-Basis für dieses HTML/Tailwind Projekt.`
- `$end-to-end-project-orchestrator bringe diese Landingpage von Ist-Zustand zu polished, tested und PR-ready.`

## Maintenance

- Keep skills narrow and descriptions explicit.
- Bump `.codex-plugin/plugin.json` version for meaningful releases.
- Run `node scripts/validate-plugin.mjs` before pushing.
- Add dependencies to templates only when they are the default for that plugin's workflow.
