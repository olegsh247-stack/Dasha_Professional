# Project Status

**Repository:** `olegsh247-stack/Dasha_Professional`  
**Current approved source:** `main`  
**Current release:** v1.0.2  
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
| Professional Learning System | 1.0.2 | Approved | Includes readiness and authority-verification consistency refinements merged through PRs #8 and #9 on 2026-11-10. |
| Universal Learning Skill | 1.0.1 | Approved | Requires explicit verification of a profession module's source, lifecycle status and approval before use; no profession-specific curriculum is embedded in the Skill. |
| Startup and progress protocol | 1.0.1 | Approved | Current-source guidance, compact two-level loading and complete unsaved-record fallback. |
| Risk Management profession module | — | Not established on `main` | A historical source pointer is listed below. Its professional content and approval status are not assessed by this repository audit; verify them in the profession's own authoritative workflow before use. |
| Other profession modules | — | Not started | No other approved modules are indexed on `main`. |
| Integrations registry | 1.0 | Active | Reference-only index at [integrations/README.md](integrations/README.md). No live technical connections or automatic synchronization are configured. |
| Shared Learning Log | — | Active | Baseline program decision recorded; detailed historical lesson records have not been imported. |
| Competency Register | — | Active | Initialized; no imported or assessed competency entries yet. |
| Repository quality checks | — | Active | Markdown lint and link validation run on pushes, pull requests and manual dispatch. |
| `main` branch protection | — | Not enabled by design | No mandatory branch protection/ruleset is configured. This is an intentional usability decision: avoid restrictive controls that previously disrupted the owner's workflow. CI continues to run on pushes and pull requests; PRs are the preferred change path, not a technical requirement. |

## Profession module discovery pointers

These are explicit lookup locations, not approvals:

| Profession | Source | Classification | Required handling |
|---|---|---|---|
| Risk Management | Branch `feat/risk-management-learning-kit` in this repository | Historical source; not approved by this repository's main baseline | Verify the module's own status, owner approval, current curriculum and progress records in its designated workflow before teaching from it. Do not infer approval from the branch name. |

Discovery rules:

1. Check `main` first for an approved profession module.
2. If absent, consult only the exact alternative-source pointers listed in this section and any explicit source named by the user or the profession's own project status.
3. Treat a historical branch or external project as a location to investigate, not as evidence of approval or currency.
4. If the pointer is stale, inaccessible or ambiguous, report that fact. Do not search arbitrary branches and do not guess.
5. If no authoritative module can be verified, prepare a proposed module from `learning-system/profession-template.md` and request user approval before treating it as active.

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
