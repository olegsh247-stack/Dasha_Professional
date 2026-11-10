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
| Risk Management profession module | — | Not established on `main` | Historical files were observed on older feature branches and deliberately excluded from the approved Core and Learning System baseline. Their professional content and approval status are not assessed here. Verify in the profession's own workflow before use. |
| Other profession modules | — | Not started | No approved modules are indexed on `main`. |
| Integrations registry | 1.0 | Active | Reference-only index at [integrations/README.md](integrations/README.md). No live technical connections or automatic synchronization are configured. |
| Shared Learning Log | — | Active | Baseline program decision recorded; detailed historical lesson records have not been imported. |
| Competency Register | — | Active | Initialized; no imported or assessed competency entries yet. |
| Repository quality checks | — | Active | Markdown lint and link validation run on pushes, pull requests and manual dispatch. |
| `main` branch protection | — | Not enabled by design | No mandatory branch protection/ruleset is configured. This is an intentional usability decision: avoid restrictive controls that previously disrupted the owner's workflow. CI continues to run on pushes and pull requests; PRs are the preferred change path, not a technical requirement. |

## Source-of-truth rules

1. Use `main` and the release metadata in `manifest.json` as the default current source.
2. A branch is not an approved release merely because it contains files or was used in an earlier chat.
3. A profession module's approval must be established in its own source and must not be inferred from this repository's general architecture approval.
4. Independent projects remain authoritative for their own content.
5. When the current source or version cannot be verified, stop short of claiming it is current; report the uncertainty.

## Change control

1. Use a dedicated branch and pull request as the preferred path for planned changes to approved architecture.
2. Direct changes to `main` remain permitted when the owner considers them necessary; no branch rule blocks them.
3. CI runs on pushes and pull requests. Both Markdown lint and link validation should pass before a change is considered complete. Investigate and rerun transient external-service failures rather than silently disabling checks.
4. A PR must identify scope, affected files, verification performed and any exclusions. Merging requires explicit user authorization when the assistant is carrying out the merge.
5. No production deployment is implied by repository approval.
