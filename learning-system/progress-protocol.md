# Progress Protocol — continuity across learning chats

## 1. Purpose

Preserve continuity across learning chats for professions maintained in `Dasha_Professional`, without repeatedly asking the user for information already recorded. This protocol defines what to read, where local facts live, how progress is evidenced and how updates are saved.

## 2. Project boundary and sources of truth

This protocol applies only to learning programs and records maintained in `olegsh247-stack/Dasha_Professional`.

The Learning Log and Competency Register in this repository contain only learning events and competency evidence created here. They are not cross-project records. Never load another project's journal or competency register into these local records; never copy, summarize, reconstruct, migrate or synchronize another project's learning history here.

When the user explicitly switches to an independent project, stop applying this repository's recordkeeping workflow and follow that project's own instructions and sources of truth. An integration link is navigation only.

For learning within this repository, use the most specific authoritative source:
1. approved profession module and its current curriculum;
2. profession-specific lesson records, exercises, assessments and artifacts stored with that module;
3. this repository's local Competency Register;
4. this repository's local Learning Log;
5. current chat, as provisional context until a durable local record is saved;
6. assistant recollection or inference, labelled unverified.

If two authoritative sources conflict, surface the conflict and do not silently overwrite either one.

## 3. What to load at session start

Load the compact orientation set first:
1. current `PROJECT-STATUS.md` and `manifest.json`;
2. `core/knowledge-and-evidence-governance.md`;
3. `core/README.md` and only Core documents relevant to the current lesson;
4. `learning-system/SKILL.md` and this protocol;
5. selected profession's current README, approved curriculum and profession-specific Skill;
6. relevant profession-specific records and the latest relevant entries in this repository's Learning Log and Competency Register.

The Dasha identity charter may be consulted for identity context at its designated source. It is not a source of learning records for this repository. Do not load a separate Cross-Project Learning System as authority for this repository's records.

Load detailed lessons, source packs, casebooks and additional Core documents only when needed. Never omit the authoritative curriculum or local records that establish the continuation point.

## 4. Recovery when local progress records are incomplete or inconsistent

1. Identify the latest authoritative approved curriculum and its version.
2. Search the selected profession module's own lesson, casebook and assessment records for the latest completed activity and evidence.
3. Compare those artifacts with this repository's local Learning Log and Competency Register. Do not compare them with unrelated project records.
4. Check the current chat for additional material, but label unsaved information as provisional.
5. Build a short recovery snapshot:
   - **Confirmed** — directly supported by an accessible authoritative local record or artifact.
   - **Inferred** — plausible from partial evidence but not independently confirmed.
   - **Unknown / conflicting** — missing, inaccessible or inconsistent information.
6. Resume from the latest confirmed point. Do not repeat confirmed completed work. Pause only a step that depends on unresolved information.
7. If no reliable completion point can be established, explain the narrow uncertainty; do not invent one or silently restart.

Never promote inferred or provisional activity into a completed lesson, assessment result or competency achievement without evidence.

## 5. Local Learning Log format

Append one concise entry for each meaningful milestone that occurs in this repository's learning program:
- **Event ID and date**
- **Profession/module and lesson or activity**
- **Participant:** user / Dasha / joint
- **Learning State**, if applicable
- **Evidence Level before → after:** E0–E5 or Not mapped
- **Learning outcome**
- **Evidence/artifact:** local path or exact source reference
- **Assessment and result**
- **Corrections / open questions**
- **Next step**
- **Saved at / readback verification**

Do not add entries about learning events from another project, including short summaries or reconstructed histories.

## 6. Local Competency Register format

Maintain one row per competency and participant for professions maintained in this repository:
- Competency ID and name;
- profession/module;
- participant;
- Learning State;
- Evidence Level (E0–E5 or Not mapped);
- local evidence references and assessment criteria;
- assessment method and date;
- confidence/limitations;
- next development step;
- last reviewed.

The register is a current snapshot, not a second narrative journal. Every demonstrated achievement must point to local evidence and criteria.

## 7. Evidence rules

Learning State and Evidence Level are independent dimensions. Apply the E0–E5 minimum evidence criteria in `core/knowledge-and-evidence-governance.md`. Distinguish reading, explanation, guided exercise, independent application, repeatability and external review. Keep Dasha's evidence separate from the user's. Ratings, attendance, confidence and lesson counts do not promote an E-level.

## 8. End-of-session update

At the end of a meaningful lesson or milestone within this repository:
1. summarize the learning outcome;
2. capture answers, practical artifacts and assessment;
3. record corrections and unresolved questions;
4. update only affected local competency entries;
5. append a local Learning Log event;
6. identify the next lesson or unfinished task;
7. save to the authorized local repository and read the saved content back.

### Required fallback when repository write access is unavailable

Provide a complete, copy-ready update labelled:

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
Competency changes:
Next step:
Intended local destination:
Reason not saved:
```

Clearly state that the record has not been written. If a field is unknown, mark it `unknown`; do not invent it. Do not prepare a record for another project's repository under this protocol.

## 9. Avoiding repeated questions

Before asking the user to restate a preference, background detail, prior decision or completed lesson, search relevant local records and current project files. Ask only if information is absent, conflicting, outdated or materially ambiguous.

## 10. Synchronization

No automatic synchronization is assumed between chats, GitHub, Library or plugins. Every saved update identifies its local destination and is verified by readback. This protocol does not authorize cross-project record synchronization, copying or migration.
