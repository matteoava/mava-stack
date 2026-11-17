---
name: reconcile
description: Compare a current plan or build baseline with artifacts, shared memory, approved changes, and completion evidence in both directions. Use to find evidenced coverage, gaps, contradictions, unplanned work, and change impacts, with owners and next actions; reconciliation does not execute the build or approve changes.
---

# Reconcile

Give the user a traceable view of how the actual work aligns with the identified plan and approved basis. Keep planned, produced, reported, verified, and accepted work distinct instead of collapsing them into one status.

## Uses

Read the applicable instructions below before acting.

- [ORCHESTRATE.MD shared execution rules](../../ORCHESTRATE.MD#shared-execution-rules) and [principle 8](../../PRINCIPLES.md#8-make-claims-and-outcomes-traceable) for evidence levels.
- verify for deeper checks of specific claims, context for memory alignment, and [storyline](../storyline/SKILL.md) for a formal report or deck.

## 1. Resolve the comparison

- Read the local AGENTS.md, the canonical shared MEMORY.md, and existing activity records. Identify the initiative, activity and work-item IDs, the governing plan, the relevant requirement, architecture, and SoW baselines, approved changes, and the comparison date or source cutoff.
- Keep working plans, issued baselines, estimate scenarios, and draft changes distinct. Confirm material ambiguity about which version governs; the newest filename is not automatically authoritative.
- If no plan exists, report the missing comparison basis and review the supplied relationships provisionally, without inventing an approved plan.
- Agree the breadth (one workstream, delivery readiness, a changed requirement, or the whole activity). Reuse existing status schemas and ownership; a new chat does not reset the activity.

## 2. Inspect records and evidence

- Collect the plan's expected outcomes, scope, deliverables, dependencies, owners, acceptance criteria, and recorded status.
- Inspect the corresponding artifacts and source versions, approved change records, contributor updates, shared-memory claims, and the evaluation or runtime evidence supplied by responsible contributors.
- Treat filenames, indexes, AI summaries, and earlier completion reports as leads until their content is inspected. Label metadata-only and inaccessible items, and record partial coverage.
- Attach evidence identities and dates to the exact work item and artifact version. A test against an earlier configuration does not validate a later one, and an unsigned draft or customer request does not amend the baseline.

## 3. Reconcile in both directions

Use a compact matrix or the existing equivalent, with only the fields this decision needs:

| Field | Capture |
| --- | --- |
| Basis | Requirement or plan item, expected outcome, governing source and version, and relevant approved change. |
| Actual position | Artifact and version, recorded status, contributor report, and inspected evidence with usable locations. |
| Alignment | Supported coverage, partial coverage, no evidence found, contradiction, or applicability unresolved. |
| Impact and action | Affected dependencies and artifacts, consequence, responsible owner, next check or decision, and resuming trigger. |

Run four passes:

- **Plan to evidence:** does each relevant planned outcome have the right artifact, coverage, dependencies, and completion or acceptance evidence? Missing evidence is a gap, not a failure.
- **Evidence to plan:** what produced or reported work has no traceable requirement, plan item, or approved change? Recognize useful shared components, legitimate enabling work, and duplicates before judging something unplanned.
- **Memory to originals:** compare memory and summary claims with the plan, artifacts, corrections, and evidence. Flag stale or contradicted claims; memory never overrides approved records.
- **Changes across the chain:** trace approved or proposed changes through requirements, architecture, effort, proposal, SoW, delivery plan, tests, and handover, showing affected versions, pending alignment, and the owner of each update.

Preserve shared work and compound-operation boundaries: one component can cover several items without counting as several completed journeys. Check integration and end-to-end evidence, not only component evidence.

## 4. Assess conflicts and consequences

- Separate defects, evidence gaps, stale trackers, pending decisions, unmet dependencies, proposed changes, and acceptance gaps. A contributor reporting that work has begun can expose a stale "not started" tracker without proving completion; avoid duplicate assignments while the status is resolved.
- Investigation is not implementation, and implementation is not validation. Keep backlog, exclusions, and open feasibility checks visible. An existing artifact, a passed syntax check, or a deployed configuration alone does not prove runtime or business success.
- Explain conflicts by source authority, applicability, and version lineage. Keep genuine uncertainty, unknown owners, and joint ownership; never invent a root cause, completion percentage, effort, date, or approval to fill a table.
- Prioritize findings by their effect on the decision, scope, dependencies, acceptance, or customer commitments, and give the smallest useful next action and the evidence needed to close each material gap. Contributors keep build and runtime execution; the architect coordinates oversight.

## 5. Explain and maintain the result

- Start with the overall position, then explain material differences step by step with enough context to understand consequences and choices. Adapt through feedback, and report the understanding state.
- Return the comparison basis, prioritized findings, supported progress, coverage limits, affected work, and next owners and actions or waiting triggers. A short table or explanation in chat is usually enough; do not create a matrix file or send a status broadcast automatically.
- When persistence or correction is authorized, reuse existing shared records and save under the shared rules. Record the actual correction and its evidence, and keep baselines and historical approval intact. Use context for concise memory alignment within capture authority.
- Produce a formal report or deck through storyline. If no usable base exists, return the analysis and ask for a reference before producing the file.

## Completion and boundaries

The work is complete when the requested scope has a traceable alignment view, or an explicit incomplete result with its remaining gaps. Record item and source versions, completed comparisons, open decisions, owners, and next triggers so later reviews continue the same activity.

Reconciliation does not approve scope changes, amend signed or issued commitments, execute missing work, or claim acceptance for another owner. Messages, publication, access changes, schedules, and native-memory updates need their own authority. Keep operational findings and customer material out of the public toolkit.
