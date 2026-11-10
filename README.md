# Dasha_Professional

**Purpose:** shared architecture and universal learning infrastructure for Dasha's professional development.

## Start here

1. [Project status](PROJECT-STATUS.md) — approved, draft and planned components.
2. [Version manifest](manifest.json) — current release, source branch and file fingerprints.
3. [Core](core/README.md) — Dasha's general identity, principles, methodology and governance.
4. [Professional Learning System](learning-system/README.md) — reusable learning workflow.
5. [Shared learning records](records/README.md) — cross-profession progress index.

## Project boundaries

- Professional modules live in `professions/` and define profession-specific knowledge and curricula.
- Independent projects such as Psychology and Crypto remain their own sources of truth; this repository may link to them but does not copy their content.
- Integrations are planned; no integrations registry is currently implemented.
- A profession module is not considered available or approved merely because it exists on an old or separate branch. Check [PROJECT-STATUS.md](PROJECT-STATUS.md) and [manifest.json](manifest.json).

## Quality checks

Pull requests and pushes to `main` run automated checks:

- **Markdown lint:** `markdownlint-cli2` checks repository Markdown against the shared configuration in `.markdownlint-cli2.jsonc`.
- **Link validation:** Lychee checks Markdown links, including relative repository paths and reachable external URLs.

Both checks must pass before a change is considered ready for approval. A transient external-service failure should be investigated and rerun; do not silently disable link validation to make a check green.

## Working rules

- Use the current approved version on `main`, unless a project instruction explicitly names another ref.
- Make changes on a dedicated branch and review them through a pull request.
- Never claim that chats, GitHub, Library or plugins synchronize automatically.
- Verify every repository write by reading the saved content back.
- Do not make production, destructive or externally consequential changes without explicit authorization.

## Current release

See [PROJECT-STATUS.md](PROJECT-STATUS.md) for component lifecycle and [manifest.json](manifest.json) for version metadata.
