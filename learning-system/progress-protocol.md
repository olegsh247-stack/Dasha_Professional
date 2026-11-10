# Progress Protocol — continuity across learning chats

## 1. Purpose

Preserve learning continuity across separate chats and professions without repeatedly asking the user for information already recorded. This protocol defines what to read, where facts live, how progress is evidenced and how updates are saved.

## 2. Governing rules and source-of-truth hierarchy

The Dasha charter and Cross-Project Learning System in Library, together with the approved Core in this repository, govern general identity, learning conduct, knowledge transfer and recordkeeping. They are governing instructions, not substitutes for project facts or professional evidence.

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
2. the two governing Library documents, if available;
3. `core/README.md` and only the Core documents relevant to the current lesson;
4. `learning-system/SKILL.md` and this protocol;
5. the selected profession's current README, approved curriculum and profession-specific Skill;
6. relevant profession-specific records and the latest relevant entries in the shared Learning Log and Competency Register.

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
- **Learning outcome:**
- **Evidence or artifact:**
- **Assessment and result:**
- **Corrections / open questions:**
- **Next step:**
- **Saved at / source reference:**

The log is chronological. Do not rewrite old entries merely to make the history look cleaner; record corrections as new events and preserve provenance.

## 6. Competency Register format

Maintain one row per competency and participant, where appropriate:

- **Competency ID and name**
- **Profession/module**
- **Participant**
- **State:** not started / studied / in progress / practiced / demonstrated achievement / open question / future direction
- **Evidence references**
- **Assessment method and date**
- **Confidence/limitations**
- **Next development step**
- **Last reviewed**

The register is a current snapshot, not a second narrative journal. Every demonstrated achievement must point to evidence and criteria.

## 7. Evidence rules

Distinguish reading, explanation, guided exercise, independent application, repeated performance under varied conditions, and external or independent assessment. A higher level requires stronger evidence. Keep Dasha's learning evidence separate from the user's.

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

## 11. Synchronization and versioning

No automatic synchronization is assumed between chats, GitHub, Library or plugins. Every saved update should identify the target branch or source, date and relevant file. Preserve historical entries and use version control for changes. Do not overwrite profession-specific sources from the shared system.
