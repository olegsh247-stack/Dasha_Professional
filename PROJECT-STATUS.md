# Project Status

**Repository:** `olegsh247-stack/Dasha_Professional`  
**Current approved source:** `main`  
**Current approved release:** v1.0.2  
**Approved:** 2026-11-10  
**Candidate architecture update:** `feat/knowledge-evidence-governance-v1` — pending review; not approved for operational use.

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
| Core | 1.0.0 | Approved | Current approved baseline; proposed knowledge/evidence governance addition is pending review on `feat/knowledge-evidence-governance-v1`. |
| Professional Learning System | 1.0.2 | Approved | Current approved baseline; proposed source-authority and dual-axis progress refinements are pending review. |
| Universal Learning Skill | 1.0.1 | Approved | Current approved baseline; proposed exact-ref verification and dual-axis evidence rules are pending review. |
| Startup and progress protocol | 1.0.1 | Approved | Current approved baseline; proposed canonical-source, provenance and migration rules are pending review. |
| Risk Management profession module | — | Not established on `main` | A historical source pointer is listed below. Its professional content and approval status are not assessed by this repository audit; verify them in the profession's own authoritative workflow before use. |
| Other profession modules | — | Not started | No other approved modules are indexed on `main`. |
| Integrations registry | 1.0 | Active | Reference-only index at [integrations/README.md](integrations/README.md). No live technical connections or automatic synchronization are configured. |
| Shared Learning Log | — | Active | Baseline program decision recorded; detailed historical lesson records have not been imported. |
| Competency Register | — | Active | Initialized; no imported or assessed competency entries yet. |
| Repository quality checks | — | Active | Markdown lint and link validation run on pushes, pull requests and manual dispatch. |
| `main` branch protection | — | Not enabled by design | No mandatory branch protection/ruleset is configured. This is an intentional usability decision: avoid restrictive controls that previously disrupted the owner's workflow. CI continues to run on pushes and pull requests; PRs are the preferred change path, not a technical requirement. |

## Proposed architecture update — not yet approved

The branch `feat/knowledge-evidence-governance-v1` contains a proposed cross-cutting update:
- `core/knowledge-and-evidence-governance.md` — canonical-source control, separate Learning State and E0–E5 Evidence Level, and a staged historical-migration protocol;
- Appendix A of `core/knowledge-and-evidence-governance.md` — exact external source bindings, fingerprints and known discrepancies;
- aligned Core, Skill, startup prompt, progress protocol and shared record templates.

The proposal does not import historical records, change competency levels, alter the separate Dasha repository or Library, or designate an unresolved external record as an approved migration baseline. The Dasha charter itself is verified on the separate repository's `main` at version 2; its Library mirror is stale. See Appendix A of `core/knowledge-and-evidence-governance.md`. Current approved release remains v1.0.2 on `main` until review and an explicit merge.

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
