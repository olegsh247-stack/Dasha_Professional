# Knowledge & Evidence Governance

**Status:** Approved architecture baseline; corrective boundary revision proposed in PR.
**Purpose:** Define source authority, learning states, evidence levels and recordkeeping boundaries for this repository.

## 1. Scope and non-negotiable project boundary

This document governs the Core and the Professional Learning System maintained in `olegsh247-stack/Dasha_Professional`.

**All records in this repository are local to this repository.** The Learning Log and Competency Register may cover professions whose modules are maintained here, but they are not cross-project repositories and must never contain another project's learning events, lesson history, competency evidence or assessments.

Independent projects retain their own curricula, records, evidence, decisions and source-of-truth rules. Links may be maintained for navigation and boundary awareness only. A link does not authorize reading records into this repository, copying them, summarizing their history here, mapping their competencies here or migrating them here.

No cross-project learning-record migration or synchronization is supported by this repository's policy. If the owner later wants a different architecture, it requires a separately discussed and approved design; this document is not authorization for it.

## 2. Canonical-source governance

### 2.1 One authority per document

For every governing document used operationally, identify:
- repository or system and exact file path;
- designated branch, tag or immutable commit;
- document version and lifecycle status;
- content fingerprint where available;
- owner/approver and approval evidence;
- last verified date.

A filename, newest timestamp, Library location, branch name or plugin availability alone does not establish authority.

### 2.2 Authority roles

- **Canonical repository revision:** authoritative editable source when its exact ref, version and approval status are explicitly designated.
- **Library copy:** distribution mirror or working copy; it is not a second authority unless explicitly designated.
- **Plugin/portable Skill copy:** execution package derived from a canonical source; it must identify its source revision and may not silently override it.
- **Project-local records:** authoritative only for the project in which they were created and maintained.
- **Navigation pointer:** a link or short description identifying an independent project. It carries no learning history, evidence, approval or synchronization authority.

### 2.3 Conflict handling

If copies of the same governing document differ, do not merge them by choosing the newest or longest copy. Record each candidate's exact source, version, ref, fingerprint, status and unique content. Mark the canonical revision **Unresolved** until its owner selects or reconciles it. During the conflict:
- do not teach from conflicting instructions as though they were one approved version;
- do not overwrite either copy;
- use only independently authoritative, non-conflicting rules;
- pause only actions whose correctness depends on the unresolved rule;
- verify the selected copy by reading it back.

### 2.4 External identity reference

The Dasha identity/development charter is maintained by its owning project. This repository may retain a navigation pointer to that charter for identity context, but does not own, mirror or govern the charter's project-specific learning records. The pointer does not authorize importing another project's Learning Log, Competency Register, curriculum history or evidence.

## 3. Two independent dimensions: Learning State and Evidence Level

### 3.1 Learning State — lifecycle of activity

Use exactly one current state for a given participant, competency or learning objective:

| State | Meaning |
|---|---|
| **Not started** | No learning activity is recorded for this objective. This is not a judgment about prior knowledge. |
| **Studied** | Relevant material was reviewed. Practical performance is not established. |
| **In progress** | A structured learning activity is currently underway. |
| **Practiced** | The participant attempted exercises, simulations or real tasks. Quality and independence remain separately assessed. |
| **Demonstrated achievement** | A specified outcome was checked against explicit criteria and points to evidence. |
| **Open question** | A material gap, contradiction or uncertainty remains unresolved. |
| **Future direction** | The topic is intentionally outside the active learning plan. |

These states are not a mandatory linear ladder. A topic can return to In progress after a new standard, correction or failure. Open question may be tracked separately; do not erase the underlying activity state to hide uncertainty.

### 3.2 Evidence Level — strength of a competency claim

Use the E0–E5 scale only for a specific competency claim, participant and scope:

| Level | Meaning | Minimum evidence |
|---|---|---|
| **E0 — Not assessed** | No meaningful assessment yet. | None. |
| **E1 — Exposure** | Material reviewed; familiarity only. | Identified source/material and scope reviewed. |
| **E2 — Explained** | Can accurately explain core concepts and limitations. | Explanation checked against reliable sources or a knowledgeable reviewer. |
| **E3 — Applied with assistance** | Applied in a bounded real or simulated task with material guidance. | Concrete task, contribution, reviewer feedback and outcome; simulation explicitly labelled. |
| **E4 — Independently applied** | Completed a bounded task with limited prompting. | Reproducible artifact/result and validation. |
| **E5 — Repeatably verified** | Repeated successful application in different or non-trivial cases. | At least two distinct validations, including failure/boundary cases where relevant. |

E0–E5 describes evidence strength, not a human credential, licence, clinical competence or professional certification. E5 does not imply authorization to perform regulated work.

### 3.3 Relationship between dimensions

- Studied + E1 is common, but not mandatory.
- Practiced may remain E0 or E1 if the attempt was not meaningfully assessed.
- Demonstrated achievement requires identified assessment and evidence; it does not automatically mean E3 or higher.
- A competency may retain E3 while its learning state is In progress.
- E0 means not assessed; it does not mean incapable or no prior knowledge.
- Never calculate or promote E-levels automatically from lesson count, ratings, confidence, attendance or learning state.

Record both dimensions independently. If a source contains only one, preserve the original value and mark the missing dimension **Not mapped** until reviewed.

## 4. Evidence and attribution rules

Every competency claim must be scoped to:
- competency ID/name and domain;
- participant: Dasha, user or another explicitly identified person;
- task/context and date;
- learning state;
- evidence level (or Not assessed / Not mapped);
- evidence artifact and exact source reference;
- assessment method, assessor/reviewer and result;
- simulation/real-world status;
- limitations, confidence and excluded claims;
- next assessment or development step.

Keep the user's learning evidence separate from Dasha's model/tool performance. Distinguish user feedback from independent review. A numerical satisfaction rating is qualitative feedback, not by itself competency evidence.

Do not transfer an evidence level to a broader competency, another participant, another profession or another project without a separately approved assessment process and new supporting evidence. This repository does not provide a cross-project transfer process.

## 5. Project-local recordkeeping

### Learning Log — chronological local events

Record only meaningful learning events that occur within this repository's own learning programs. Each entry should include:
- event ID and event date;
- profession/module and learning objective;
- participant and attribution;
- activity/outcome and original assessment;
- Learning State, if applicable;
- Evidence Level before → after, or Not assessed / Not mapped;
- evidence artifact and exact local source reference;
- assessment method, reviewer and result;
- simulation/real-world status;
- limitations, corrections and next step;
- saved destination and readback verification.

### Competency Register — current local snapshot

Each row should include:
- stable Competency ID and name;
- profession/module maintained in this repository;
- participant;
- current Learning State and Evidence Level;
- evidence pointers and assessment criteria;
- assessor/method/date;
- scope, limitations and confidence;
- last reviewed and next assessment.

The Log is chronological. The Register is a current snapshot. Neither replaces source artifacts.

Do not add another project's event, lesson, assessment, competency status, evidence reference or reconstructed summary to either file. Do not use an external project's records to fill gaps in these local records. If the user asks to work in another project, follow that project's own workflow and keep its records there.

## 6. Synchronization and version control

No automatic synchronization is assumed among chats, GitHub, Library or plugins. Every mirror update must identify its source revision and be verified by content comparison or fingerprint. A sync operation must not overwrite unique destination-only material without reconciliation.

This synchronization rule applies to copies of documents within an explicitly authorized distribution workflow. It does not establish cross-project record synchronization or migration.

Changes to this governance standard require versioning, review and explicit approval. A proposed revision must not be represented as active policy until approved.
