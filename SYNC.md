# Mirror → Canonical Sync Checklist (Workflows)

Source (mirror): `projects/ai-env/workflows/`
Destination (canonical): this repo (`projects/workflows/`)

Use this checklist to upstream environment‑local workflow improvements into the canonical library.

## 1) Prepare
- Identify changed files in mirror: `git -C ../../ai-env status -- workflows/`
- Optional: quick overview via status helper
  - From canonical repo: `bash ../scripts/src/mirror-status.sh --repo-root ../ai-env --areas workflows`
  - Or from mirror: `bash ../ai-env/scripts/mirror-status.sh`
- Gather related context: README updates, ADRs, and usage examples.

## 2) Validate Workflow Quality
- Generality: Remove environment‑specific names/paths; keep steps broadly applicable.
- Structure: Keep guides concise; use clear “Intent” and “Steps” sections.
- Composability: Split long flows; link sub‑workflows rather than nesting deeply.
- Outcomes: Specify verifiable artifacts or acceptance criteria.

## 3) Sync Steps
- Create a branch here: `git checkout -b chore/sync-workflows-<date>`
- Port changes from mirror, adjusting links to canonical paths.
- Cross‑link related guides and examples (e.g., `example-workflow.md`).

## 4) Review
- Ensure cross‑links exist:
  - `../../START-HERE.md`
  - `../../README.md`
- Check for overlap with existing guides; deduplicate or reference instead of duplicating.

## 5) Submit
- PR description: intent, entry point(s), and expected outputs.
- Note downstream integrations (scripts, prompts, projects).

Notes
- Keep the canonical set lean; archive niche variants in the mirror.
- Prefer links over duplication to avoid drift.
