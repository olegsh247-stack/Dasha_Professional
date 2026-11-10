# Knowledge & Evidence Governance

**Status:** Proposed — not approved until this change is reviewed and merged.
**Version:** 1.0.0
**Purpose:** Define one operational contract for canonical sources, learning states, evidence levels and safe migration of historical learning records across Dasha projects.

## 1. Scope and governing principle

This document governs cross-project knowledge and evidence handling. It does not replace a project's own source-of-truth rules, professional curriculum, legal obligations or safety controls.

Every record must answer four separate questions:

1. **Authority:** which source and exact revision is authoritative?
2. **Learning state:** where is the learning activity in its lifecycle?
3. **Evidence level:** how strongly is a specific competency claim supported?
4. **Provenance:** where did the record and its evidence originate, and how were they transformed?

Never infer one answer from another. A current record is not automatically authoritative; a completed lesson is not automatically a demonstrated competency; a high evidence level does not imply a licence or professional qualification.

## 2. Canonical-source governance

### 2.1 One authority per document

Each cross-project governing document must have one canonical source identity:

- repository or system;
- exact file path;
- designated branch, tag or immutable commit;
- document version and lifecycle status;
- content fingerprint (Git blob SHA where available);
- owner/approver and approval evidence;
- last verified date.

A filename, newest timestamp, Library location, branch name or plugin availability alone does not establish authority.

### 2.2 Authority roles

- **Canonical repository revision:** authoritative editable source when its exact ref, version and approval status are explicitly designated.
- **Library copy:** distribution mirror or working copy; it is not a second authority. It may be used as canonical only when the source register explicitly designates that Library item and version.
- **Plugin/portable Skill copy:** execution package derived from the canonical source. It must identify its source revision and may not silently override it.
- **Project-specific records:** authoritative for that project's facts, decisions, detailed evidence and artefacts.
- **Shared Learning Log:** cross-project chronology and provenance index; not a substitute for original evidence.
- **Shared Competency Register:** current cross-project snapshot; not a narrative history or source of detailed evidence.

### 2.3 Conflict handling

If copies differ, do not merge them by choosing the newest or longest copy. Record each candidate's exact source, version, ref, fingerprint, status and unique content. Mark the canonical revision **Unresolved** until the owner/approver selects or reconciles it. During the conflict:

- do not silently teach from conflicting governance instructions as though they were one approved version;
- do not overwrite either copy;
- use only non-conflicting rules that are independently authoritative;
- pause only actions whose correctness depends on the unresolved rule;
- create a reconciliation record and verify the selected copy by readback.

### 2.4 Current source bindings and unresolved items

The companion [Source Authority Register](source-authority-register.md) records the exact audited bindings. The 2026-11-10 audit established:

- **Dasha charter:** GitHub repository `olegsh247-stack/Dasha`, path `docs/dasha-personality-development-and-competencies.md`, branch `main`, version 2, blob SHA `d231f2e203ce512876c2f00cfa5f5526e58b0c08`. The Dasha Cross-Project Learning System and Archive Index identify this file as the canonical charter. The Library copy is version 1 and differs; it is a stale mirror, not an equal authority. The same version 2 blob was also present on the archive branch. That branch is 332 commits ahead of main, but the charter itself is already on main.
- **Cross-Project Learning System:** the latest identified Library item is `LEARNING-SYSTEM.md`, dated 2026-11-05 and listed as current operating rules. Its own text says GitHub is the source of truth and Library is a planned mirror, but a matching GitHub source path/ref and fingerprint were not confirmed. Its exact authority binding remains unresolved.
- **Central Learning Log:** GitHub branch v5.0 and Library v5.0 differ; the GitHub copy includes later entries (including MI-32) not present in the Library copy read during audit.
- **Central Competency Register:** GitHub branch v3.0 and Library v3.0 matched exactly in the comparison performed. The detailed v3.0 snapshot is on an archive branch 332 commits ahead of main; its approved release binding remains unresolved.

The repository identity and charter source are therefore resolved; mirror synchronization and the authority binding for the cross-project system and historical central records remain open. Do not promote the unresolved records to an approved migration baseline. See the Source Authority Register for hashes, statuses and required owner actions.

## 3. Two independent dimensions: Learning State and Evidence Level

### 3.1 Learning State — lifecycle of activity

Use exactly one current state for a given participant, competency or learning objective:

| State | Meaning |
|---|---|
| **Not started** | No learning activity is recorded for this objective. This is not a judgment about prior knowledge. |
| **Studied** | Relevant material was reviewed. Practical performance is not established. |
| **In progress** | A structured learning activity is currently underway. |
| **Practiced** | The participant has attempted exercises, simulations or real tasks. The quality and independence of performance remain separately assessed. |
| **Demonstrated achievement** | A specified outcome was checked against explicit criteria. This state must point to evidence and its limits. |
| **Open question** | A material gap, contradiction or uncertainty remains unresolved. |
| **Future direction** | The topic is intentionally outside the active learning plan. |

These states are not a mandatory linear ladder. A topic can return to In progress after a new standard, correction or failure. Open question may coexist as a separate issue record; do not erase the underlying activity state to hide uncertainty.

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

E0–E5 describes evidence strength, not a learning-state label, human credential, licence, clinical competence or professional certification. E5 does not imply authorization to perform regulated work.

### 3.3 How the dimensions relate

- Studied + E1 is common, but not mandatory.
- Practiced may remain E0 or E1 if the attempt was not meaningfully assessed.
- Demonstrated achievement requires an identified assessment and evidence; it does not automatically mean E3 or higher.
- A competency may retain E3 while its learning state is In progress.
- E0 means not assessed; it does not mean incapable or no prior knowledge.
- Never calculate or promote E-levels automatically from lesson count, ratings, confidence, attendance or learning state.

Record both dimensions independently. If a legacy source contains only one, preserve the original value and mark the missing dimension **Not mapped** until reviewed.

## 4. Evidence and attribution rules

Every competency claim must be scoped to:

- competency ID/name and domain;
- participant: Dasha, user, or another explicitly identified person;
- task/context and date;
- learning state;
- evidence level (or Not assessed / Not mapped);
- evidence artifact and exact source reference;
- assessment method, assessor/reviewer and result;
- simulation/real-world status;
- limitations, confidence and excluded claims;
- next assessment or development step.

Keep the user's learning evidence separate from Dasha's model/tool performance. Distinguish user feedback from independent review. A numerical satisfaction rating is qualitative feedback, not by itself competency evidence.

Do not transfer an evidence level to a broader competency, another participant or another profession without an explicit mapping and additional validation.

## 5. Historical migration protocol

Historical migration is an evidence-preservation operation, not a content-cleanup exercise.

### Phase 0 — Freeze and scope

1. Name the source projects, repositories, branches, Library locations and date range in scope.
2. Record the migration batch ID, operator, start date and immutable source snapshot (commit/ref, file version, blob SHA or equivalent).
3. Make no source edits or deletions during inventory.
4. Exclude sensitive or unnecessary personal data; retain only the minimum evidence needed.

### Phase 1 — Inventory

For every source artifact or record, capture:

- migration batch ID;
- original record/event ID, if any;
- original event date and source-record date separately;
- participant and project/module;
- source system, repository, exact path, ref/version and fingerprint;
- artifact type: user original, assistant output, dialogue, exercise, assessment, reconstruction, summary, correction or index;
- current status in the source project;
- links to related originals, superseded versions and duplicates;
- integrity/readability check.

Do not treat an index entry or summary as the original artifact.

### Phase 2 — Classify and reconcile

Classify each item as **Canonical original**, **Supporting evidence**, **Index/summary**, **Superseded**, **Duplicate**, **Reconstruction**, **Unverified** or **Conflict**.

- Preserve unique source material and its provenance.
- Keep superseded or reconstructed records as historical provenance; do not count them as independent evidence if they derive from the same event.
- Deduplicate only after comparing content and lineage; record which copy is retained and why.
- If GitHub and Library differ, preserve both snapshots and record the exact delta. Do not silently select one.
- If event date, participant, authorship or assessment cannot be verified, mark it Unknown.

### Phase 3 — Map without promotion

1. Map legacy topics/competencies to target competency IDs with a written rationale.
2. Preserve the original wording and status in the migration record.
3. Assign a proposed Learning State and Evidence Level separately.
4. Set evidence level to **Not mapped** or **E0 — Not assessed** when the source does not support a defensible assessment.
5. Do not raise a level because the record is old, extensive, highly rated or repeated in summaries.
6. Preserve simulation labels, reviewer identity and limits.
7. Require review for every proposed E3–E5 mapping; E4/E5 additionally require validation of independence/repeatability criteria.

### Phase 4 — Import and verify

1. Import only records explicitly approved for the target register.
2. Use stable IDs and preserve original IDs.
3. Append migration metadata; do not rewrite the source artifact.
4. Verify record counts, unique IDs, source fingerprints, links, classifications and competency mappings.
5. Compare a sample and all high-level competency claims against original evidence.
6. Record rejected, deferred and unresolved items; do not silently omit them.
7. Read back the saved target records and confirm the source snapshots remain unchanged.

### Phase 5 — Closeout and rollback

A migration batch is complete only when the inventory reconciles to imported + deferred + rejected + unresolved counts, with reasons for every non-imported item. Preserve the batch manifest and source snapshots. If verification fails, stop the batch and revert only the target import using the recorded batch ID; never delete or alter source originals.

No historical migration is authorized merely by this policy. Scope, sources, mappings and import batch require explicit approval before writes.

## 6. Required record schemas

### Learning Log — chronological event

Each event should include:

- Event ID; event date; record/import date;
- profession/project/module and learning objective;
- participant and attribution;
- activity/outcome and original assessment;
- Learning State (if applicable);
- Evidence Level before → after (or Not assessed / Not mapped);
- evidence/artifact type and exact source reference;
- repository/path/ref/version/fingerprint where available;
- reviewer/assessor and method;
- simulation/real-world status;
- limitations, corrections and next step;
- migration batch/original event ID if imported;
- saved destination and readback verification.

### Competency Register — current snapshot

Each row should include:

- stable Competency ID and name;
- profession/module and participant;
- current Learning State;
- current Evidence Level;
- evidence pointers and assessment criteria;
- assessor/method/date;
- scope, limitations and confidence;
- last reviewed and next assessment;
- provenance/migration reference where applicable.

The Log is chronological. The Register is a current snapshot. Neither replaces source artifacts.

## 7. Synchronization and version control

No automatic synchronization is assumed among chats, GitHub, Library or plugins. Every mirror update must identify its source revision and be verified by content comparison or fingerprint. A sync operation must not overwrite unique destination-only material without reconciliation.

Changes to this governance standard require versioning, review and an explicit approval record. Until approved, this file is a proposal and must not be represented as an active policy.
