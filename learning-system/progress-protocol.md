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

If two authoritative sources conflict, surface the conflict and do not silently overwrite either one. A general governance document does not override a more specific approved project decision or professional source on factual matters; conversely, project-specific facts do not silently rewrite Dasha's general operating rules.

## 3. What to load at session start

Read in this order:
1. governing Library documents and relevant Core documents;
2. selected profession module and its current curriculum;
3. latest relevant profession-specific learning record;
4. shared Competency Register;
5. latest relevant entries in shared Learning Log;
6. unresolved tasks and prior chat context, if available.

Load only records relevant to the selected profession and its dependencies; do not dump the user's entire learning history into every chat.

## 4. Shared Learning Log format

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

## 5. Competency Register format

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

## 6. Evidence rules

Distinguish:
- reading or exposure;
- explanation in one's own words;
- a single guided exercise;
- independent application;
- repeated performance under varied conditions;
- external or independent assessment.

A higher level requires stronger evidence. Do not infer durable mastery from attendance, a multiple-choice result alone, or one successful example. Record the scope and conditions under which performance was demonstrated.

Keep Dasha's learning evidence separate from the user's. Joint work is not automatically proof that each participant can perform independently.

## 7. End-of-session update

At the end of a meaningful lesson or milestone:
1. summarize the learning outcome;
2. capture answers, practical artifacts and assessment;
3. record corrections and unresolved questions;
4. update only affected competency entries;
5. append a Learning Log event;
6. identify the next lesson or unfinished task;
7. save to the authorized source, then verify the saved content.

If the repository is unavailable or write permission is absent, produce the exact update in the chat and label it **NOT SAVED**. Do not claim that the central records have changed.

## 8. Avoiding repeated questions

Before asking the user to restate a preference, background detail, prior decision or completed lesson:
- search the relevant records;
- check the current chat and available project files;
- use the latest confirmed value;
- ask only if the information is absent, conflicting, outdated or materially ambiguous.

If a record is missing, ask for the smallest missing piece. Do not ask the user to reconstruct an entire history when a partial record or artifact can be recovered.

## 9. Cross-profession transfer

Transfer a competency only when its meaning and evidence genuinely apply to the destination profession. Record the source profession, original evidence, limits and any additional validation required. Similar names do not guarantee equivalent competencies.

## 10. Synchronization and versioning

No automatic synchronization is assumed between chats, GitHub, Library or plugins. A synchronization claim requires a completed write and read-back verification.

Every saved update should identify the target branch or source, date and relevant file. Preserve historical entries and use version control for changes. Do not overwrite profession-specific sources from the shared system.
