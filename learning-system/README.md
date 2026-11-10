# Professional Learning System

**Status:** first implementation; structural consistency review completed 2026-11-10, approval pending.  
**Working branch:** `feat/universal-learning-system`.

## Purpose

A reusable system for launching and conducting structured professional education in a separate chat without repeatedly collecting information already established in Core, the selected profession module, or the learning records.

## Architecture

1. **Core** — identity, principles, universal methodology, quality, governance and knowledge-management rules.
2. **Professional Learning System** — this folder; universal learning behavior, startup protocol, module template and progress protocol.
3. **Profession module** — profession-specific curriculum, competencies, standards, sources, cases, exercises and assessment criteria.
4. **Records** — shared Learning Log and Competency Register, plus profession-specific evidence and detailed learning artifacts.
5. **Independent project integrations** — references to existing projects, whose repositories remain their own sources of truth.

## Start a learning chat

Use [START-PROMPT.md](START-PROMPT.md). The chat must load the current Core, this system, the selected profession module and relevant records before teaching. Until this branch is approved and merged, explicitly load `feat/universal-learning-system`.

## Files

- [SKILL.md](SKILL.md) — universal instructions for all profession-learning chats.
- [START-PROMPT.md](START-PROMPT.md) — reusable startup prompt; specify a profession once.
- [profession-template.md](profession-template.md) — standard for creating new profession modules.
- [progress-protocol.md](progress-protocol.md) — continuity, evidence and recordkeeping rules.

## Shared records

- [Learning Log](../records/learning-log.md) — chronological learning events. It contains the initial program-design decision; detailed historical lesson records have not been imported.
- [Competency Register](../records/competency-register.md) — current competency states and evidence pointers. It is initialized but has no imported or assessed competency entries.

The shared records do not replace profession-specific histories or the authoritative records of standalone projects.

## Non-automatic synchronization

A GitHub repository, chat history, Library and plugins do not synchronize themselves. A new chat must actually retrieve the latest files and write updates through an available, authorized integration. If write access is unavailable, it must produce a concise record for later transfer and clearly say that it has not saved it.
