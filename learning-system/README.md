# Professional Learning System

**Status:** Approved — first edition approved 2026-11-10.  
**Approved baseline:** v1.0.1.  
**Current source:** `main` (see [manifest.json](../manifest.json)).

## Purpose

A reusable system for launching and conducting structured professional education in a separate chat without repeatedly collecting information already established in Core, the selected profession module or learning records.

## Architecture

1. **Core** — identity, principles, universal methodology, quality, governance and knowledge-management rules.
2. **Professional Learning System** — universal learning behavior, startup protocol, module template and progress protocol.
3. **Profession module** — profession-specific curriculum, competencies, standards, sources, cases, exercises and assessment criteria.
4. **Records** — shared Learning Log and Competency Register, plus profession-specific evidence and detailed learning artifacts.
5. **Independent project integrations** — reference-only links in the active [integrations registry](../integrations/README.md). Independent projects remain their own sources of truth; no live technical connections or automatic synchronization are implied.

## Governing Library documents

- `dasha-personality-development-and-competencies.md` — canonical Dasha identity and long-term development charter.
- `LEARNING-SYSTEM.md` — cross-project learning, knowledge transfer and centralization rules.

Load the latest verified versions from Library when available. The 2026-11-05 revision was the latest identified on 2026-11-10 and supersedes the 2026-11-04 copy. These documents are not automatically synchronized with this repository.

## Start a learning chat

Use [START-PROMPT.md](START-PROMPT.md). The prompt points to the current approved `main` version. Do not use an old feature branch unless a current project instruction explicitly designates it.

The startup process has two levels:

- **Level 1 — required orientation:** project status and manifest, the two governing Library documents (if accessible), Core index, this system's Skill and progress protocol, the selected profession's entry documents, and the relevant shared/profession records.
- **Level 2 — on-demand context:** load individual Core documents, prior lessons, casebooks, source packs and related project artifacts only when the lesson or a conflict requires them.

If the profession module is absent from `main`, follow only the alternative-source pointers explicitly recorded in [PROJECT-STATUS.md](../PROJECT-STATUS.md). Do not infer approval from a branch name or inspect unrelated branches.

Do not confuse a shorter startup with permission to skip the profession's authoritative curriculum or current progress records.

## Files

- [SKILL.md](SKILL.md) — universal instructions for all profession-learning chats.
- [START-PROMPT.md](START-PROMPT.md) — compact reusable startup prompt; specify a profession once.
- [profession-template.md](profession-template.md) — standard for creating new profession modules.
- [progress-protocol.md](progress-protocol.md) — continuity, evidence and recordkeeping rules.

## Shared records

- [Learning Log](../records/learning-log.md) — chronological learning events. It contains the initial program-design decision; detailed historical lesson records have not been imported.
- [Competency Register](../records/competency-register.md) — current competency states and evidence pointers. It is initialized but has no imported or assessed competency entries yet.

The shared records do not replace profession-specific histories or authoritative records of standalone projects.

## Non-automatic synchronization

A GitHub repository, chat history, Library and plugins do not synchronize themselves. A new chat must actually retrieve the latest files and write updates through an available, authorized integration. If write access is unavailable, produce the complete update record in the conversation, label it **NOT SAVED**, and identify its intended destination.
