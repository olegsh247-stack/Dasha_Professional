# Progress Protocol — continuity across learning chats

## 1. Purpose

Preserve learning continuity across separate chats and professions without repeatedly asking the user for information already recorded. This protocol defines what to read, where facts live, how progress is evidenced and how updates are saved.

## 2. Governing rules and source-of-truth hierarchy

The Dasha charter and Cross-Project Learning System govern identity and cross-project learning only at their exact approved revisions. Verify repository/system, path, ref, version, status and fingerprint; Library/plugin copies are mirrors unless explicitly designated canonical. Approved Core and [Knowledge & Evidence Governance](../core/knowledge-and-evidence-governance.md) govern shared recordkeeping. If copies conflict or no approved ref is identifiable, record the conflict and pause only dependent actions; do not silently choose the newest copy.

For factual claims, project decisions and learning evidence, use the most specific authoritative source:

1. **Profession/project source of truth** — approved curriculum, professional decisions, detailed cases and project-specific evidence.
2. **Profession-specific learning artifacts** — lesson records, exercises, assessments and casebooks.
3. **Shared Competency Register** — current cross-profession view of competency states and evidence pointers.
4. **Shared Learning Log** — chronology of significant learning events and corrections.
5. **Current chat** — provisional context until a durable record is saved.
6. **Assistant recollection or inference** — never stronger than a recorded source; label as unverified.

If two authoritative sources conflict, surface the conflict and do not silently overwrite either one.

## 3. What to load at session start

Load the compact orientation set first:

1. current `PROJECT-STATUS.md` and `manifest.json`;
2. Appendix A of `core/knowledge-and-evidence-governance.md`;
3. the exact approved revisions of the Dasha charter and Cross-Project Learning System, using the register and fingerprint; compare Library/plugin mirrors and report any mismatch;
4. `core/knowledge-and-evidence-governance.md`;
5. `core/README.md` and only the Core documents relevant to the current lesson;
6. `learning-system/SKILL.md` and this protocol;
7. the selected profession's current README, approved curriculum and profession-specific Skill;
8. relevant profession-specific records and the latest relevant entries in the shared Learning Log and Competency Register.

Load detailed lessons, source packs, casebooks and additional Core documents only when needed to teach, verify evidence or resolve a conflict. Never omit the authoritative curriculum or records that establish the continuation point.

## 4. Recovery when progress records are incomplete or inconsistent

Do not restart a program or repeat a lesson merely because one record is missing. Recover the continuation point systematically:

1. Identify the latest authoritative approved curriculum and its version.
2. Search the profession-specific lesson, casebook and assessment records for the latest completed activity and its evidence.
3. Compare that evidence with the shared Learning Log and Competency Register. Use the records for their defined roles: the log is chronological, the register is a current snapshot, and profession-specific artifacts hold detailed evidence.
4. Check the current chat for additional material, but label unsaved information as provisional.
5. Build a short recovery snapshot with three explicit categories:
   - **Confirmed** — directly supported by an accessible authoritative record or artifact.
   - **Inferred** — plausible from partial evidence but not independently confirmed.
   - **Unknown / conflicting** — missing, inaccessible or inconsistent information.
6. Resume from the latest confirmed point. Do not repeat confirmed completed work. If the next activity depends on an unresolved conflict or an unconfirmed prerequisite, pause only that dependent step and ask one focused question; otherwise continue while clearly marking the limitation.
7. If no reliable completion point can be established, do not invent one or silently restart. Explain the narrow uncertainty and offer the smallest diagnostic check or recap needed to establish the next step.

Never promote an inferred or provisional activity into a completed lesson, assessment result or competency achievement without evidence.

## 5. Shared Learning Log format

Append one concise entry for each meaningful milestone:

- **Event ID:**
- **Date:**
- **Profession/module:**
- **Lesson or activity:**
- **Participant:** user / Dasha / joint
- **Learning State:** if applicable
- **Evidence Level before → after:** E0–E5 or Not mapped
- **Learning outcome:**
- **Evidence or artifact:**
- **Assessment and result:**
- **Corrections / open questions:**
- **Next step:**
- **Saved at / source reference:** exact repository/path/ref/version/fingerprint where available
- **Original event ID / migration batch:** if imported

The log is chronological. Do not rewrite old entries merely to make the history look cleaner; record corrections as new events and preserve provenance.

## 6. Competency Register format

Maintain one row per competency and participant, where appropriate:

- **Competency ID and name**
- **Profession/module**
- **Participant**
- **Learning State:** Not started / Studied / In progress / Practiced / Demonstrated achievement / Open question / Future direction
- **Evidence Level:** E0 / E1 / E2 / E3 / E4 / E5 (or Not mapped)
- **Evidence references and exact source provenance**
- **Assessment method and date**
- **Confidence/limitations**
- **Next development step**
- **Last reviewed**

The register is a current snapshot, not a second narrative journal. Every demonstrated achievement must point to evidence and criteria.

## 7. Evidence rules

Learning State and Evidence Level are independent dimensions. Apply the E0–E5 minimum evidence criteria in `core/knowledge-and-evidence-governance.md`. Distinguish reading, explanation, guided exercise, independent application, repeatability and external review. Keep Dasha's evidence separate from the user's. Ratings, attendance, confidence and lesson counts do not promote an E-level.

## 8. End-of-session update

At the end of a meaningful lesson or milestone:

1. summarize the learning outcome;
2. capture answers, practical artifacts and assessment;
3. record corrections and unresolved questions;
4. update only affected competency entries;
5. append a Learning Log event;
6. identify the next lesson or unfinished task;
7. save to the authorized source and read the saved content back.

### Required fallback when repository write access is unavailable

Do not stop at saying that saving failed. Produce a complete, copy-ready update in the conversation using this structure:

```text
LEARNING RECORD — NOT SAVED
Event ID:
Date:
Profession / module / version:
Lesson or activity:
Participant: user / Dasha / joint
Learning objective:
Learning outcome:
Evidence / artifact:
Assessment and result:
Corrections / open questions:
Competency changes (ID, participant, old state → new state, evidence):
Next step:
Intended destination:
Reason not saved:
```

Include the actual lesson outcome and evidence, not placeholders, whenever that information is available. If a field is genuinely unknown, mark it `unknown` rather than inventing it. Clearly state that the record has not been written to GitHub or Library. The user should be able to transfer this record without reconstructing the lesson.

## 9. Avoiding repeated questions

Before asking the user to restate a preference, background detail, prior decision or completed lesson, search relevant records and current project files. Ask only if information is absent, conflicting, outdated or materially ambiguous.

## 10. Cross-profession transfer

Transfer a competency only when its meaning and evidence genuinely apply to the destination profession. Record the source profession, original evidence, limits and any additional validation required.

## 11. Synchronization, provenance and historical migration

No automatic synchronization is assumed between chats, GitHub, Library or plugins. Every saved update identifies exact target/source system, path, ref, version, date and fingerprint where available. Compare mirrors before claiming synchronization; preserve destination-only content.

Historical imports must follow `core/knowledge-and-evidence-governance.md`: freeze source snapshots; inventory every record; preserve original IDs, event dates, authorship, participant, exact path/ref/fingerprint and artifact lineage; classify originals, supporting evidence, summaries, reconstructions, superseded items, duplicates and conflicts; map Learning State and Evidence Level independently; import only after explicit batch review; verify counts, IDs, links and source integrity. Do not rewrite source originals, silently deduplicate, or retroactively promote evidence. A missing historical record in the shared system is not evidence that the learning never occurred.
