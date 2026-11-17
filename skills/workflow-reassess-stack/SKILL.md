---
name: workflow-reassess-stack
description: Start, resume, or report on a bulk assessment of model and agentic-harness changes across an AI architect's stack, using current primary sources, representative acceptance cases, and evidence-backed recommendations.
---

# Reassess the stack workflow

Method version: 1.

Assess whether model or harness changes should alter the stack's methods, configuration, or delegation. It runs on the monthly cadence when one is configured in the host scheduler, or on explicit request between scheduled runs.

## Uses

Read the applicable instructions below before acting.

- [ORCHESTRATE.MD](../../ORCHESTRATE.MD): start, resume, or status; PLAN.md; waits and handoffs; and the shared execution rules.
- context, search, verify, reconcile, decompose, storyline, and deslop as appropriate. If one is unavailable, use the procedure directly and say what did not run.

## Start, resume, or status

Follow [Start, resume, or report status](../../ORCHESTRATE.MD#start-resume-or-report-status). Resolve the authorized operational working folder, the current skill and workflow inventory, the working profile, the prior assessment, and the designated private maintenance or shared records. Never store operational findings or private configuration in public toolkit files.

- **Start:** establish the review period, relevant releases, current configurations, audience, and decisions to support.
- **Resume:** reload source dates, tested configurations, completed cases, pending comparisons, and decisions. Reuse valid evidence and rerun only what changed.
- **Status:** report coverage, evidence, gaps, regressions, recommendations, and next actions without making unrequested changes or inventing results.

Keep the instance in PLAN.md or its existing equivalent, using the fields in [ORCHESTRATE.MD](../../ORCHESTRATE.MD#planmd) plus configuration baselines. Store detailed evidence with the assessment.

## Assessment loop

1. **Verify releases.** Use current primary vendor documentation and release notes for model and harness changes since the previous assessment. Record source dates, versions, availability, prerequisites, and uncertainty. Keep announced features separate from behavior verified in the configured environment.
2. **Inventory exposure.** Map each skill and workflow to its model, harness, tools, source access, artifact route, scheduling, memory, permissions, and handoff dependencies across ChatGPT Work, Codex, Claude Code, or other configured hosts. Report missing configuration rather than assuming parity.
3. **Assess effects.** Review context handling, reasoning, tool use, delegation, computer use, artifact quality, structured output, long-running work, resumption, evaluation, latency, and cost where evidence exists. Name the affected methods and the practical consequence for daily architecture work.
4. **Choose acceptance cases.** Use representative synthetic inputs with explicit expected outcomes. As relevant to the inventory, cover source routing, conflicting or missing context, requirements-architecture-estimate lineage, plan-artifact-memory reconciliation, session preparation, requirements consolidation, clear writing, and artifact handoffs.
5. **Compare honestly.** Run equivalent inputs against current and candidate configurations only when access, authorization, and tools allow. Keep configuration versions, inputs, outputs, observations, and scoring criteria. If one side is unavailable, report a documentary assessment or an untested proposal; never fabricate comparisons, costs, or runtime results.
6. **Prioritize changes.** Produce skill-by-skill and workflow-level findings, regressions, simplifications, migration dependencies, and recommendations, with the benefit, trade-off, evidence strength, expected effort, owner, and proposed validation for each material change.
7. **Apply or hand off.** Complete routine maintenance that is already authorized, with appropriate checks. Keep consequential changes reviewable and wait for the relevant authority. Coordinate with existing maintenance work and release candidates instead of producing duplicates.

## Action boundaries

- Never silently change default models, harnesses, permissions, source locations, production integrations, or artifact routes. Explain meaningful choices and intended actions, and report the understanding state. Current vendor documentation does not prove local compatibility.
- Do not create, modify, or duplicate schedules without explicit authorization. The monthly trigger is a host scheduler setting, not a runtime this skill provides. Preserve independently authorized maintenance routines.
- Keep detailed customer records in their shared folders and only relevant source references in the assessment. Leave public long-term memory empty and native-host memory controls unchanged.
- Never publish private findings. A public candidate must pass the release rules in AGENTS.md and user review.
- Produce requested decks and formal documents through [storyline](../storyline/SKILL.md); if no usable base exists, return the content brief and ask for a reference first.
- Save under the shared rules, and keep completed action IDs and evidence so resumed work repairs partial failures without repeating successful external actions.

## Handoff or completion

Return the review period, assessed inventory and configurations, primary sources, cases actually run, findings, prioritized recommendations, open decisions, owners, and next actions. Keep documentary checks, runtime observations, and untested expectations distinct.

Complete the scoped review or checkpoint an explicit waiting or incomplete state. A release announcement, a generated report, or a successful schedule registration does not show that the whole stack was tested or upgraded.
