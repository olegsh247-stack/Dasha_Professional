# Project Status

**Repository:** `olegsh247-stack/Dasha_Professional`  
**Current approved source:** `main`  
**Current approved release:** v1.1.0  
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
| Core | 1.1.0 | Approved | Includes the canonical-source and evidence-governance standard adopted in PR #11. |
| Professional Learning System | 1.1.0 | Approved | Includes source-authority checks, independent Learning State and E0–E5 dimensions, provenance and strict project-local record boundaries. |
| Universal Learning Skill | 1.1.0 | Approved | Aligned with the approved v1.1.0 manifest; exact-ref verification and dual-axis evidence rules are included. |
| Startup and progress protocol | 1.1.0 | Approved | Aligned with the approved v1.1.0 manifest; canonical-source, provenance and project-local record rules are included. |
| Risk Management profession module | — | Not established on `main` | A historical source pointer is listed below. Its professional content and approval status are not assessed by this repository audit; verify them in the profession's own authoritative workflow before use. |
| Other profession modules | — | Not started | No other approved modules are indexed on `main`. |
| Integrations registry | 1.0 | Active | Reference-only index at [integrations/README.md](integrations/README.md). No live technical connections or automatic synchronization are configured. |
| Project-local Learning Log | — | Active | Records only learning events created within this repository. No cross-project history is included. |
| Project-local Competency Register | — | Active | Initialized; tracks only competencies evidenced within this repository. |
| Repository quality checks | — | Active | Markdown lint and link validation run on pushes, pull requests and manual dispatch. |
| `main` branch protection | — | Not enabled by design | No mandatory branch protection/ruleset is configured. This is an intentional usability decision: avoid restrictive controls that previously disrupted the owner's workflow. CI continues to run on pushes and pull requests; PRs are the preferred change path, not a technical requirement. |

## v1.1.0 release record

Approved on 2026-11-10. The release incorporates the cross-cutting knowledge and evidence governance architecture merged in PR #11 (commit `27d219f6e798c62c05bd1bc098bb3bf32d40748b`).

Included:
- canonical-source authority rules;
- independent Learning State and E0–E5 Evidence Level dimensions;
- evidence attribution and provenance requirements;
- project-local Learning Log and Competency Register boundaries;
- aligned Core, Professional Learning System, Skill, startup prompt, progress protocol and local record templates.

No records or competency evidence from independent projects are included. No cross-project migration or synchronization is supported by this repository's recordkeeping policy. Independent projects retain their own records and sources of truth.

## Profession module discovery pointers

These are navigation pointers only, not approvals or permission to access or copy learning records:

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
3. A profession module's approval must be established in its own source and must not be inferred from this repository's general architecture approval. Its project-specific learning history remains in that project.
4. Independent projects remain authoritative for their own content, learning records and competency evidence.
5. When the current source or version cannot be verified, stop short of claiming it is current; report the uncertainty.

## Change control

1. Use a dedicated branch and pull request as the preferred path for planned changes to approved architecture.
2. Direct changes to `main` remain permitted when the owner considers them necessary; no branch rule blocks them.
3. CI runs on pushes and pull requests. Both Markdown lint and link validation should pass before a change is considered complete. Investigate and rerun transient external-service failures rather than silently disabling checks.
4. A PR must identify scope, affected files, verification performed and any exclusions. Merging requires explicit user authorization when the assistant is carrying out the merge.
5. No production deployment is implied by repository approval.
