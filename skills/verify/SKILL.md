---
name: verify
description: Check a claim, calculation, artifact, or reported result against evidence suited to the decision. Use before relying on facts, numbers, documents, configurations, or completion claims; reports the exact verified scope and gaps without equating inspection with runtime or business success.
---

# Verify

Establish what the available evidence actually supports, what contradicts it, and what still needs checking. Scale the effort to the consequence of being wrong.

## Uses

Read the applicable instructions below before acting.

- [Principle 8](../../PRINCIPLES.md#8-make-claims-and-outcomes-traceable) for evidence levels, and the [ORCHESTRATE.MD shared execution rules](../../ORCHESTRATE.MD#shared-execution-rules).
- [storyline](../storyline/SKILL.md) for a formal report or deck, and the assigned contributors for runtime or acceptance evidence.

## 1. Define the question

- Identify the claim or artifact, its intended use and audience, the relevant version or environment, and the expected behavior or acceptance criterion.
- For initiative work, read the local AGENTS.md, shared MEMORY.md, and the authoritative records they reference. Memory and prior AI answers are leads to inspect, not proof.
- Resolve the exact baseline and scenario. A current product capability, an issued estimate, and a historical project result need different evidence. Ask only for information that would change the conclusion.

## 2. Choose evidence that can establish the claim

| Subject | Useful checks |
| --- | --- |
| Product or technical fact | Current primary documentation, release and version applicability, prerequisites, and observed configuration. Distinguish announced, documented, configured, and demonstrated behavior. |
| Calculation or estimate | Recompute material totals from inputs, units, rates, scenarios, dates, and formulas. Check detail rows against summaries, filters, duplicates, ranges, hidden sheets, and cached values. |
| Requirement or decision | Original source and location, intended meaning, stable ID, disposition, decision owner, and actual approval evidence. A request or draft is not approval. |
| Document or deck | Content against sources, numerical consistency, correct version and audience, the rendered layout, image and screenshot provenance, references, notes, and metadata. |
| Configuration or implementation | The actual artifact against the stated design or requirement, keeping syntax, configuration, import, deployment, runtime, and business outcome as separate levels. |
| Reported completion | Matching work-item and artifact versions, contributor evidence, reproducible results, and required acceptance. An update or a successful tool call alone does not prove the outcome. |

Use current authoritative sources for changing external facts, and record each source's identity, date, applicability, and inspection depth. Summaries, forwards, and copies of one original are not independent corroboration.

## 3. Perform bounded checks

- Inspect originals with format-aware tools. Distinguish metadata, extracted content, visual inspection, independent recalculation, executed tests, and results someone else merely reported.
- Recompute decision-critical numbers from their basis. For lower-risk repetition, a stated sample is acceptable; disclose its size and the uncovered scope. Never claim a workbook was recalculated when only stored values were read.
- Check consistency across the relevant source and output versions, including totals, claims, scope, assumptions, dates, captions, and references.
- For visual artifacts, render and inspect the changed or material pages for clipping, overflow, unreadable charts, broken images, and unintended layout changes. A valid file is not a visual check.
- For behavioral claims, state the input, expected outcome, actual evidence, and environment. Configuration inspection does not prove execution. Coordinate missing runtime or acceptance evidence with the assigned contributor rather than taking over delivery execution.
- Record inaccessible sources, unavailable tools, uninspected attachments, partial pagination, and incomplete checks. Absence of evidence alone does not prove failure or falsity.

Stop expanding once the decision-relevant scope is covered. Broaden only for a demonstrated inconsistency, material risk, or newly affected scope.

## 4. Resolve or report findings

- For each material finding, give the exact location, expected versus observed position, evidence level, consequence, and a useful correction or next check.
- Classify each claim as supported, contradicted, insufficiently evidenced, or not checked, with plain reasons rather than invented confidence scores.
- Separate a confirmed defect from a suspected cause. Explain disagreements by authority and applicability, not recency, and keep open ownership, rationale, and acceptance explicit.
- Correct only within write authority. Preserve originals and approved baselines, make targeted changes to the current human-edited version or a proposed amendment, and rerun the affected checks. Never overwrite contributor work, alter commitments, or drop qualifications to make a result pass.

## 5. Explain and hand off

- Lead with the scoped conclusion and the highest-impact findings, then evidence pointers, checks actually performed, corrections actually saved, uncovered scope, and the next owner and action or waiting condition. A qualified result beats a broad assurance the checks do not support.
- Explain material checks and reasoning step by step at the user's level, adjust through feedback, and report the understanding state. Keep any clarification needed before dependent consequential work visible.
- A chat response is enough for ordinary verification. Produce a formal report or deck through storyline, and if no usable base exists, return the findings and ask for a reference first.
- Keep detailed findings in the existing shared record when persistence is authorized, saved under the shared rules. Shared memory may receive a concise correction or pointer within its capture mandate.

## Completion and boundaries

The work is complete when the stated scope has an evidence-supported conclusion, or an explicit incomplete result with the missing evidence and next responsible action. Record completed checks and their artifact versions so later work can resume without repeating them.

Keep conclusions within the stated scope; broader system, business-outcome, or acceptance claims need their own support. Verification does not approve scope, send messages, publish material, or start monitoring.
