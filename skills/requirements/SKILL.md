---
name: requirements
description: Extract, consolidate, or update source-linked solution requirements from customer inputs, sessions, comments, and existing records. Preserves scope and approval state, stable IDs, acceptance criteria, open questions, and version lineage without treating incoming feedback as an approved change.
---

# Requirements

Turn customer inputs into requirements the user can explain, review, and hand to design or delivery. Preserve what was actually requested, what remains uncertain, and who can decide it.

## Uses

Read the applicable instructions below before acting.

- [ORCHESTRATE.MD shared execution rules](../../ORCHESTRATE.MD#shared-execution-rules) and [principle 7](../../PRINCIPLES.md#7-explain-until-the-user-understands).
- prepare-session when a discovery or design session is needed, architect for the downstream design, and [storyline](../storyline/SKILL.md) for a formal requirements document or deck.

## 1. Resolve the task and current basis

- Decide whether the task is extraction, consolidation, or revision, and identify the initiative, audience, decision, and requested output.
- Read the local AGENTS.md, shared MEMORY.md, current requirements, scope or SoW, and relevant decisions before creating anything. Reuse existing filenames, IDs, structure, and activity state.
- Inspect supplied documents, deck content, annotations, spreadsheets, notes, and authorized communications. Record each source's identity, author, date, version, and precise location, and report inaccessible attachments, partial searches, and missing versions.
- Distinguish primary customer statements, participant notes, AI meeting summaries, existing synthesis, approved baselines, and reference examples. Read enough context to catch corrections, and do not count forwarded or repeated material as independent confirmation.

## 2. Extract faithfully before interpreting

- For an extraction-only request, return the statements or comments with their source locations, worded faithfully and kept separate from interpretation. Do not replace them with a proposed change list.
- For consolidation, restate each distinct need clearly while keeping its meaning and provenance. Split genuinely different needs, and link duplicates rather than losing their sources.
- Preserve corrections and conflicting accounts, and weigh them by authority, applicability, and evidence. A newer message alone does not amend agreed scope.
- Leave missing rationale, thresholds, owners, dates, and identifiers unknown under the existing convention. Ask a focused question where the answer changes scope or behavior.
- Another initiative's document is a structure reference only. Its facts, metrics, commitments, and acceptance terms never become requirements here.

## 3. Consolidate a usable requirement set

Use the existing schema and add only the fields this work needs. Give new requirements stable IDs, keep existing IDs through revisions, and keep a mapping when splitting or merging.

| Element | Capture where relevant |
| --- | --- |
| Need and purpose | Actor, business outcome, trigger, expected behavior, and boundaries. |
| Provenance | Original statement, source, version, location, contributor, and effective date. |
| Scope and authority | Proposed or agreed scope, backlog, exclusions, priority, decision owner, and actual approval evidence, kept separate from delivery status. |
| Acceptance | Observable expected result, conditions, examples, and the evidence or owner needed to accept it. |
| Dependencies and gaps | Required inputs, access, data, external decisions, assumptions, conflicts, and questions with owner and next trigger. |

- Check the complete user journey as well as reusable components. Capture exception paths, roles and permissions, human action authority, data and context, integrations, operating constraints, evaluation, and nonfunctional needs to the depth this stage supports. Do not invent an exhaustive specification from a use-case title.
- Keep customer needs separate from proposed design choices and observed platform constraints. A platform limit can create an assumption, option, or validation question, not a customer requirement.
- Write testable acceptance criteria without inventing numbers or policy, using normal, error, boundary, and permission examples where material. Proposed criteria stay proposed until their authority is established; a polished document does not prove agreement.

## 4. Resolve questions and manage change

- Prioritize gaps by their effect on scope, architecture, effort, risk, and acceptance, and group related questions into a useful discussion order. Record actual answers against the affected requirement with their source.
- For a revision, compare with the identified baseline and mark items as new, clarified, corrected, removed, deferred, or unchanged, with the reason for each material change. Preserve approval state.
- Never silently overwrite signed or issued requirements, remove an exclusion, or promote an investigation into implementation scope.
- Trace affected requirements to the existing architecture, estimates, proposals, SoW, plans, and evaluation references, and name the alignment still needed and its owner. Recording a requirement does not update those artifacts. Route consequential scope or contract decisions to their owner.

## 5. Explain and produce the output

- Explain the requirements and material choices step by step, showing what is known, proposed, conflicting, and undecided. Report the understanding state separately from acceptance of the requirements, and keep open clarifications visible.
- Produce a new formal document or deck through storyline: search prior work across customers and projects, choose and copy the best editable base, adapt it with minimal layout change, clean inherited facts, notes, and metadata, and validate the content and render. If no usable base exists, return the content brief and ask for a reference before producing the file.
- For an existing artifact, start from the current human-edited version and keep its layout and contributions. Do not swap in an older or different template.
- A structured chat answer or an authorized update to an existing working record keeps its current conventions; create no boilerplate files.
- Save under the shared rules. Validate IDs, traceability, contradictions, and acceptance wording, plus the rendered layout for formatted artifacts.

## Completion and handoff

Return the requirement set or the actual updated artifact, source and baseline versions, material changes, inspection limits, open questions, and the next owner, action, or waiting trigger. State whether the result is an extraction, a draft, a proposed revision, or an evidenced approved baseline.

Hand architecture-ready inputs to architect with unresolved design dependencies explicit. Keep detailed requirements in their authoritative record, and update shared memory only within capture authority with a concise pointer or meaningful change. Do not send questions, make commitments, execute delivery work, or start monitoring.
