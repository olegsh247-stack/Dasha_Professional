# Dasha_Professional

**Purpose:** shared architecture and universal learning infrastructure for Dasha's professional development.

## Start here

1. [Project status](PROJECT-STATUS.md) — approved, draft and planned components.
2. [Version manifest](manifest.json) — current release, source branch and file fingerprints.
3. [Core](core/README.md) — Dasha's general identity, principles, methodology and governance, including [Knowledge & Evidence Governance](core/knowledge-and-evidence-governance.md).
4. [Professional Learning System](learning-system/README.md) — reusable learning workflow.
5. [Shared learning records](records/README.md) — cross-profession progress index.
6. [Independent project integrations](integrations/README.md) — reference-only links and source-of-truth boundaries.

## Project boundaries

- Approved profession modules are stored in `professions/` when added; each module defines profession-specific knowledge and curricula. The directory may be absent while no approved modules are maintained on `main`.
- Independent projects such as Psychology and Crypto remain their own sources of truth; this repository links to them without copying their content.
- The [integrations registry](integrations/README.md) is a navigation and governance index, not a live synchronization layer.
- A profession module is not considered available or approved merely because it exists on an old or separate branch. Check [PROJECT-STATUS.md](PROJECT-STATUS.md) and [manifest.json](manifest.json).

## Quality checks

Pushes to branches and pull requests run automated checks:

- **Markdown lint:** `markdownlint-cli2` checks repository Markdown against the shared configuration in `.markdownlint-cli2.jsonc`.
- **Link validation:** Lychee checks Markdown links, including relative repository paths and reachable external URLs.

Both checks should pass before a change is considered complete. A transient external-service failure should be investigated and rerun; do not silently disable link validation to make a check green.

## Working rules

- Use the current approved version on `main`, unless a project instruction explicitly names another ref.
- Prefer a dedicated branch and pull request for planned changes. Direct changes to `main` remain permitted; branch protection is intentionally not enabled.
- CI runs on pushes and pull requests; it is a quality signal, not a technical merge lock.
- Never claim that chats, GitHub, Library or plugins synchronize automatically.
- Verify every repository write by reading the saved content back.
- Do not make production, destructive or externally consequential changes without explicit authorization.

## Current release

See [PROJECT-STATUS.md](PROJECT-STATUS.md) for component lifecycle and [manifest.json](manifest.json) for version metadata.
