# Source Authority Register

**Status:** Proposed operational register; changes become active only when the governance proposal is approved.
**Last verified:** 2026-11-10
**Scope:** Cross-project governing documents and shared learning/evidence records used by Dasha_Professional.

This register records exact source identity and known discrepancies. It does not approve another project's content or override its owner.

## 1. Dasha identity and development charter

| Field | Verified value |
|---|---|
| Owner repository | `olegsh247-stack/Dasha` |
| Canonical path | `docs/dasha-personality-development-and-competencies.md` |
| Canonical ref | `main` |
| Document version | 2 |
| Git blob SHA | `d231f2e203ce512876c2f00cfa5f5526e58b0c08` |
| Authority designation | Canonical charter, explicitly identified by the Dasha Cross-Project Learning System and Dasha Archive Index |
| Lifecycle/release approval | The canonical role is designated; no separate release tag/approval record was identified in this audit |
| Library mirror | `dasha-personality-development-and-competencies.md`, version 1 |
| Mirror status | **Stale / content differs**; do not use as the current charter |
| Required action | Reconcile the Library mirror to the GitHub main v2 source through the owning project's approved sync workflow; verify exact content after transfer |

The version 2 file was fetched from both GitHub `main` and the archive branch `docs/restore-module-iii-archive-2026-11-06-current`; both returned the same blob SHA. The branch is 332 commits ahead of main, but this does not affect the charter's main-branch status because the same exact blob is present on main. Do not claim that version 2 exists only on the archive branch.

The plugin core skill is a portable runtime mirror at `skills/dasha-core/SKILL.md` in the private Dasha Assistant plugin. Its exact current content was not compared in this audit; do not claim it is synchronized.

## 2. Cross-Project Learning System

| Field | Verified value |
|---|---|
| Library item | `LEARNING-SYSTEM.md` |
| Latest identified Library revision | 2026-11-05 |
| Authority role | Listed as current operating rules in the Dasha Archive Index |
| Stated source policy | Its text says GitHub is the source of truth for verified documentation and Library is a planned mirror |
| Matching GitHub source | **Not confirmed**; the expected GitHub path was not located during this audit |
| Fingerprint/version | No Git blob SHA or explicit document version established |
| Status | **Authority binding unresolved** |
| Required action | Owning Dasha project must designate the exact canonical repository/path/ref/version/fingerprint or explicitly designate the Library item as canonical until a GitHub source exists |

Do not treat the 2026-11-05 date alone as proof of canonical authority. Use only non-conflicting instructions while the exact source binding remains unresolved.

## 3. Central Learning Log and Competency Register

| Field | Learning Log | Competency Register |
|---|---|---|
| GitHub repository | `olegsh247-stack/Dasha` | `olegsh247-stack/Dasha` |
| Current detailed revision observed | v5.0 | v3.0 |
| GitHub ref observed | `docs/restore-module-iii-archive-2026-11-06-current` | `docs/restore-module-iii-archive-2026-11-06-current` |
| GitHub blob SHA | `acbf537c15fa9efb1d37756a484c09ec7d64c32c` | `6f610c9d31f829fefa1c6dbba7553577a0063799` |
| Library revision | v5.0 | v3.0 |
| Comparison | **Differs**; GitHub contains later entries including MI-32 not present in the Library copy read during audit | **Exact text match** with GitHub branch copy in the comparison performed |
| Main branch baseline | v3.1, blob `72c90dba1b539857b913c56a6c13ee39764fd73f` | v2.5, blob `93ee6374897b188028fea6057381703ae2be51e4` |
| Status | **Authority/synchronization unresolved** | **Authority/synchronization unresolved** |

The archive branch is 332 commits ahead of `main`. The existence of v5.0/v3.0 on that branch and in Library does not by itself establish a released/approved cross-project baseline. The Learning Log Library/GitHub difference must be reconciled before migration. Preserve both copies and their unique entries.

## 4. Rules for consumers

1. Read this register and the owning project's source records before loading cross-project instructions or migrating evidence.
2. Use a source only when its exact authority binding is verified and its status permits the intended use.
3. A stale mirror is not a fallback canonical source.
4. An unresolved source may be consulted for non-conflicting context, but not used to settle a disputed rule or authorize a migration.
5. Re-verify refs and fingerprints at the start of a material migration or release; this register is a dated snapshot, not a live sync.
6. Update this register only after readback verification and record the evidence for each status change.

## 5. Migration gate

No historical Learning Log or Competency Register import into Dasha_Professional is approved by this register. Before a migration batch can start, the owning Dasha project must identify the authoritative record snapshots, reconcile unique Library-only/GitHub-only entries, and approve the exact source refs and inventory. Follow [Knowledge & Evidence Governance](knowledge-and-evidence-governance.md).
