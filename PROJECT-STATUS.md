# Project Status

**Repository:** `olegsh247-stack/Dasha_Professional`  
**Current approved source:** `main`  
**Current release:** v1.0.1  
**Approved:** 2026-11-10

## Lifecycle definitions

- **Draft** — work in progress; not approved for operational use.
- **Pending approval** — submitted for explicit review/approval; do not treat as approved.
- **Approved** — explicitly accepted baseline.
- **Active** — approved and currently in operational use.
- **Deprecated** — superseded; retained only for traceability.
- **Archived** — historical; not an active source.

## Component status

| Component | Version | Status | Notes |
|---|---:|---|---|
| Core | 1.0.0 | Approved | First edition approved 2026-11-10 and merged to `main` in PR #2. |
| Professional Learning System | 1.0.1 | Approved | v1.0.0 baseline plus operational consistency refinements merged through PR #3 on 2026-11-10. |
| Universal Learning Skill | 1.0.0 | Approved | No profession-specific curriculum is embedded in the Skill. |
| Startup and progress protocol | 1.0.1 | Approved | Current-source guidance, compact two-level loading and complete unsaved-record fallback. |
| Risk Management profession module | — | Not established on `main` | Historical files were observed on `feat/universal-learning-system`, deliberately excluded from PR #2 and PR #3. Their professional content and approval status are not assessed here. Verify in the profession's own workflow before use. |
| Other profession modules | — | Not started | No approved modules are indexed on `main`. |
| Integrations registry | — | Planned | No `integrations/` directory or registry currently exists. |
| Shared Learning Log | — | Active | Baseline program decision recorded; detailed historical lesson records have not been imported. |
| Competency Register | — | Active | Initialized; no imported or assessed competency entries yet. |

## Source-of-truth rules

1. Use `main` and the release metadata in `manifest.json` as the default current source.
2. A branch is not an approved release merely because it contains files or was used in an earlier chat.
3. A profession module's approval must be established in its own source and must not be inferred from this repository's general architecture approval.
4. Independent projects remain authoritative for their own content.
5. When the current source or version cannot be verified, stop short of claiming it is current; report the uncertainty.

## Change control

Changes to approved architecture are proposed on a dedicated branch and reviewed through a pull request. The PR must identify scope, affected files, verification performed and any exclusions. Merging requires explicit user authorization. No production deployment is implied by repository approval.
