# Workflows (Canonical Library)

Purpose: Reusable workflows, playbooks, and SOPs for AI‑human co‑development. These documents standardize how we scope, build, and validate work with AI assistance.

Structure
- Markdown guides at the repo root (see `example-workflow.md`).
- `src/`: Optional supporting files/snippets for longer guides.

Mirrored model
- Environment‑local mirror: `projects/ai-env/workflows/` is used for rapid iteration and context‑specific tweaks.
- Canonical source: Keep stable, broadly useful workflows here. Sync improvements from the mirror after validation.

Usage
- Start from `example-workflow.md` and adapt to your project.
- Prefer small, composable workflows (plan → implement → validate).
- Capture deviations and feed improvements back into this repo.

See also
- ../../START-HERE.md — Orientation and onboarding flow
- ../../README.md — Environment overview and mirrors
 - ../../docs/CO-DEV-QUADRANTS.md — Co‑dev model (normative/operative/evaluative/deliberative)

Correspondence
- Lead consumer: `projects/chirality-semantic-framework/`
- Mirror for rapid iteration: `projects/ai-env/workflows/`
- Flow: Mirror → canonical → consumer (framework), keeping workflows aligned with semantic method.

## How to PR

- Branch: `git checkout -b feat/<short-scope>` or `docs/<short-scope>`
- Validate: ensure clear “Intent” and “Steps”; specify outcomes/acceptance
- Scope: keep guides concise; split long flows and link related guides
- Describe PR: intent, entry points, expected artifacts; mention integrations
- See sync guide: `SYNC.md` for mirror → canonical steps
