# Learning Log — entry-by-entry reconciliation

**Status:** Working reconciliation report; not an approved migration baseline.  
**Audit date:** 2026-11-10  
**Scope:** Learning Log only. Competency Register and lesson source files are outside this pass.

## 1. Exact snapshots examined

| Copy | Location | Version | Exact identifier / size |
|---|---|---:|---|
| GitHub archive candidate | `olegsh247-stack/Dasha`, branch `docs/restore-module-iii-archive-2026-11-06-current`, `docs/learning/LEARNING-LOG.md` | 5.0 | Blob `81c28c3acb22c40c467e193ecd309ede60806efa`; 263,927 characters; 1,323 lines |
| Library current copy | `Dasha-Learning-Log.md` | 5.0 | Last modified 2026-11-10 19:33:48 UTC; 202,720 extracted characters; 1,000 extracted lines |
| GitHub main | `olegsh247-stack/Dasha`, `main`, same path | 3.1 | Blob `72c90dba1b539857b913c56a6c13ee39764fd73f`; older snapshot, not used as the current comparison candidate |

The archive-branch and Library copies are both labelled v5.0, but they are **not identical**. A normalized nonblank-line set comparison found 239 distinct lines only in GitHub and 14 only in Library. This is a mechanical difference count, not a semantic merge or proof that either copy is complete. The Library extraction is capped at 1,000 lines by the readback surface; its reported character count and the visible content were used for this comparison.

## 2. Entry inventory: MI-01 through MI-33

“Log entry” below means a distinct Learning Log record, not the presence or absence of the full standalone lesson file. The current archive-status sections in both copies state that all 33 full Module III original lesson files are present in GitHub and Library. That statement is treated as a recorded archive-status claim; this pass did not independently re-fetch all 33 standalone lesson files.

| Entry | GitHub archive log | Library log | Reconciliation finding / handling |
|---|---|---|---|
| MI-01 | Included in Module III completion summary | Same summary | No standalone MI-01 log entry in either copy. Preserve the shared completion summary; do not fabricate a separate lesson record. |
| MI-02 | Referenced inside the 2026-11-03 motivational-interviewing learning record; canonical source pointer present | Same | Log coverage exists in both, embedded in a broader entry rather than a standalone MI heading. Preserve the shared entry and source pointer. |
| MI-03 | Standalone archive entry | Same; identical section | No content reconciliation needed. |
| MI-04 | Standalone archive entry with three additional evidence-boundary / rating / competency-clarification lines | Same entry, shorter | Preserve the Library text and add the three GitHub-only clarifications only after confirming they remain supported by the original lesson and existing register state. No competency promotion. |
| MI-05 | Standalone archive entry | No separate MI-05 log entry | GitHub-only log history. Retain it as a candidate entry; do not infer that the Library lacks the lesson source file. |
| MI-06 | Standalone archive entry | No separate MI-06 log entry | Same handling as MI-05. Includes a research correction and explicit source limitations; preserve those details. |
| MI-07 | Standalone archive entry | No separate MI-07 log entry | GitHub-only log history. Retain user rating as qualitative feedback only; no competency promotion. |
| MI-08 | Standalone archive entry | No separate MI-08 log entry | GitHub-only log history. Preserve the professional-boundary and source-interpretation caveats. |
| MI-09 | Standalone archive entry | No separate MI-09 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-10 | Standalone archive entry | No separate MI-10 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-11 | Standalone archive entry | No separate MI-11 log entry | GitHub-only log history; retain source/regulator distinction and professional-boundary limitations. |
| MI-12 | Separate top-level section dated 2026-11-08; source pointer and archive details recorded | No MI-12 mention found in the Library log | GitHub-only log entry. The Library current archive-status section claims all 33 full originals are present, but that does not replace the missing Learning Log record. Preserve the GitHub entry as a candidate. |
| MI-13 | Standalone archive entry | No separate MI-13 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-14 | Standalone archive entry | No separate MI-14 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-15 | Standalone archive entry | No separate MI-15 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-16 | Standalone archive entry | No separate MI-16 log entry | GitHub-only log history; retain as a candidate entry. |
| MI-17 | Standalone archive entry, including follow-up learning correction | No separate MI-17 log entry | GitHub-only log history. Preserve the correction as part of provenance, not as an independent competency claim. |
| MI-18 | Shared entry, with slightly different canonical-source and archive-correction wording | Shared entry includes two Library-specific sentences about the full original replacing the concise reconstruction | Text differs, but both describe the same original and same no-promotion outcome. Retain Library's explicit provenance and GitHub's “preserved verbatim” wording in the reconciled record; do not discard either wording. |
| MI-19 | Shared historical-reconstruction entry, with slightly different wording | Shared entry contains Library-specific detail naming the full canonical source in both repositories and explicitly preserving the superseded file for provenance | Preserve Library's more explicit source-path/provenance details and GitHub's confirmation that the original is preserved in full. This entry is explicitly marked as a historical reconstruction superseded on 2026-11-08. |
| MI-20 | Shared entry; identical section | Same | No content reconciliation needed. |
| MI-21 | Shared entry; identical section | Same | No content reconciliation needed. |
| MI-22 | Earlier concise learning entry plus a separate 2026-11-08 full-original recovery entry | Earlier entry only; it includes a fuller canonical-source statement and contextual note about the *Billions* reference | Keep both dated GitHub events as separate provenance. Preserve the Library's fuller contextual clarification. Do not replace the earlier learning record with the later recovery note; the latter records an archive event, not a second lesson. |
| MI-23 | Earlier 2026-11-04 learning entry plus 2026-11-09 full-original restoration entry | No MI-23 entry | GitHub-only history includes both the original learning summary and the later supersession/restoration event. Preserve both chronologies; the earlier summary is historical, not the current canonical lesson. |
| MI-24 | Earlier 2026-11-04 learning entry plus 2026-11-09 full-original restoration entry | No MI-24 entry | Same as MI-23. Preserve both events and the qualitative 10/10 feedback as feedback only. |
| MI-25 | Earlier 2026-11-04 learning entry plus 2026-11-09 full-original restoration entry | No MI-25 entry | Same as MI-23. Preserve both events; do not infer managerial intent or competency promotion from the simulation. |
| MI-26 | 2026-11-09 entry titled “Наследник и хранитель капитала” | 2026-11-04 entry titled “family succession, loyalty, and professional boundaries” | **Material identity/content conflict.** The Library entry describes an earlier Pavel case and records substantial case formulation, source provenance and unknowns. GitHub records a later full-original restoration under the same MI number. Do not merge, overwrite, or assume these are textually identical versions until the two standalone original files and their source chronology are compared. Preserve both snapshots. |
| MI-27 | Shared 2026-11-04 summary plus a separate 2026-11-09 complete-original restoration entry | 2026-11-04 summary only | Preserve the Library summary and GitHub restoration event as distinct chronology. No competency promotion. |
| MI-28 | Shared 2026-11-04 summary plus a separate 2026-11-09 full-original entry | 2026-11-04 summary only | Preserve both. The later entry records the full original and flags an unresolved spouse/gender inconsistency in the supplied case; do not silently edit the source. |
| MI-29 | Shared 2026-11-04 summary plus a separate 2026-11-09 full-original entry | 2026-11-04 summary only | Preserve both. Later entry adds autonomy, legal/financial boundary and medical-referral caveats; no competency promotion. |
| MI-30 | Shared 2026-11-04 summary plus a separate 2026-11-10 full-original replacement/archive entry | 2026-11-04 summary only | Preserve both. Later entry documents replacement of the short reconstruction by the full original and states that no competency promotion was justified. |
| MI-31 | Shared 2026-11-10 entry | Same; identical section | No content reconciliation needed. |
| MI-32 | Shared 2026-11-04 summary plus a separate 2026-11-10 full-original archive entry | 2026-11-04 summary only | Preserve both. Later entry records a full original and self-review; no competency promotion. |
| MI-33 | Shared 2026-11-04 integration entry and Module III completion summary | Same; identical sections | No content reconciliation needed. Preserve the explicit limits: simulated exercise, not real-client practice, supervision or standardized MI assessment. |

## 3. Library-specific information that must not be lost

The following information appears in the Library copy but is absent or less explicit in the GitHub archive snapshot:

1. **MI-18:** the Library explicitly says the complete user-supplied consultation and self-review replace the earlier concise reconstruction, and that the prior Casebook/Archive Status description is superseded.
2. **MI-19:** the Library names both canonical source paths, identifies the older reconstructed file as superseded and retained for historical provenance, and states that no numeric user rating was supplied.
3. **MI-22:** the Library retains the fuller statement that the complete original and structured self-review are archived, plus the user's clarification that Wendy Rhoades in *Billions* is a useful professional working-model example, not a person or role to copy. The show is explicitly not scientific evidence or a professional template.
4. **MI-26:** the Library retains a detailed earlier case record: the 72-year-old founder, 38-year-old daughter, 51-year-old manager, dual informal/formal authority, caregiving context, manager's chosen boundary, unknowns, and the earlier source path. This must not be overwritten by the newer GitHub MI-26 record without a source-level identity check.

These are not disposable wording differences. They carry chronology, source provenance, or case-specific content.

## 4. GitHub-only Learning Log history to preserve

The GitHub archive contains additional log records not present as separate entries in Library:

- MI-05…MI-11;
- MI-12 as a separate top-level section;
- MI-13…MI-17;
- the MI-22 full-original recovery event;
- the MI-23…MI-25 original learning summaries and later restoration events;
- later full-original/restoration events for MI-27…MI-30 and MI-32.

These records must be preserved as dated evidence of learning and archive work. Their absence as standalone entries in the Library Learning Log does **not** prove that the corresponding lesson files are absent from Library.

## 5. Proposed reconciliation treatment — not yet applied

1. Keep the exact GitHub archive and Library v5.0 snapshots immutable as comparison inputs.
2. Use GitHub archive v5.0 as the **working candidate** for the chronological Learning Log because it contains later dated archive/recovery events. This is not approval of it as the sole source of truth.
3. Preserve all Library-only details from MI-18, MI-19, MI-22 and MI-26 in a reconciled working copy.
4. Preserve multiple dated archive events where GitHub records both the original learning entry and a later full-source restoration. Do not deduplicate these as though they were duplicate lessons.
5. Resolve MI-26 against the actual full original files and their source history before deciding whether the records describe one revised case or two distinct source states.
6. Before calling the reconciliation complete, verify the full originals for MI-01…MI-33 against their GitHub and Library paths, including MI-26. The current pass compared the Learning Log snapshots, not all 33 lesson files.
7. Only after the line-by-line reconciliation and MI-26 source check, produce a reconciled snapshot with a new fingerprint and ask the owner to approve the exact repository, branch, path, version and blob SHA.

## 6. Explicit exclusions

- No Learning Log content was edited in the separate `olegsh247-stack/Dasha` repository or in Library.
- No historical entry was imported, deleted, overwritten, merged or deduplicated.
- No standalone lesson file was changed.
- No Competency Register entry or evidence level was changed.
- No competency was promoted.
- No historical migration or source-of-truth approval is implied by this report.

**Current conclusion:** the two Learning Log v5.0 copies are not interchangeable mirrors. GitHub has materially more dated archive history; Library preserves unique provenance and case details. A safe reconciled copy must preserve both sets of evidence and explicitly resolve MI-26 before it can be approved.
