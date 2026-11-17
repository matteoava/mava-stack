---
name: workflow-delivery
description: Start, resume, or report on AI solution delivery architecture oversight, translating agreed scope into phased coordination, reviewing evidence, reconciling changes, and preparing handover. Implementation and runtime test execution remain with assigned delivery contributors.
---

# Delivery workflow

Method version: 1.

Coordinate delivery from the agreed architecture and scope through evidence-based handover. This workflow owns architecture oversight and coordination. Assigned delivery contributors own implementation and runtime test execution.

## Uses

Read the applicable instructions below before acting.

- [ORCHESTRATE.MD](../../ORCHESTRATE.MD): start, resume, or status; PLAN.md; waits and handoffs; and the shared execution rules.
- initialize-stack if the shared folder is not bootstrapped.
- The capabilities named in each phase. If one is unavailable, do the supported part directly and say what did not run.

## Start, resume, or status

Follow [Start, resume, or report status](../../ORCHESTRATE.MD#start-resume-or-report-status) for the project's explicitly selected shared team folder. Inspect the agreed architecture, statement of work, requirements, decisions, plan, status, and source versions, and adapt existing filenames and schemas.

On start, also establish delivery ownership, acceptance authority, and dependencies; never manufacture agreement or approval. On status, assess the evidence without executing delivery tasks or inferring progress from narrative alone.

Keep the instance in PLAN.md or its equivalent, using the fields in [ORCHESTRATE.MD](../../ORCHESTRATE.MD#planmd), with work-package owners and completed actions with their evidence.

## Phases

Begin with the actual current phase and the supplied evidence. Coordinate the next useful increment rather than recreating an existing plan or running every phase in one session.

1. **Establish the delivery baseline** (context, reconcile). Reconcile signed or approved scope, architecture, requirements, deliverables, assumptions, and acceptance criteria. Identify conflicts and missing approvals, and keep agreed scope separate from ideas still under discussion.
2. **Build the coordination plan** (decompose). Break phases into work packages and tasks with owners, dependencies, expected outputs, entry and exit criteria, and review points. Make access, customer inputs, environments, and external decisions visible, and keep implementation ownership explicit.
3. **Prepare alignment sessions** (prepare-session, requirements). Draft kickoff or solution-design material when needed. Consolidate new customer inputs into traceable requirements without silently changing the approved baseline.
4. **Oversee the architecture** (architect, verify). Review proposed designs and contributor-supplied artifacts against requirements and architecture decisions. Assess feasibility, interfaces, context and memory, permissions, failure behavior, evaluation criteria, and operational dependencies. Request specific corrections with evidence and clear owners.
5. **Review progress and acceptance evidence** (reconcile, verify). Compare the plan with artifacts, reported status, approved changes, and supplied test or evaluation results. Expose missing evidence, uncovered requirements, defects, blockers, and assumptions. Define checks and coordinate tests or retests with the contributors who run them.
6. **Manage change and recovery** (requirements, architect, reconcile). Assess new requirements, findings, and delays across scope, architecture, effort, dependencies, and acceptance. Propose explicit changes and recovery actions, preserve issued or approved baselines, and route consequential decisions to their owner.
7. **Prepare handover** (storyline, context). Assemble the evidenced final architecture, requirement coverage, decisions, limitations, operating guidance, product basics, ownership, and outstanding actions. Record acceptance evidence or the conditions still preventing handover.

## Evidence and action boundaries

- Produce requested decks and formal documents through [storyline](../storyline/SKILL.md): search prior work, choose and copy the best editable base, adapt it with minimal layout change, source informative visuals, and verify. If no usable base exists, return the content brief and ask for a reference before producing the file.
- Keep traceability in both directions between requirements, architecture, plan, artifacts, approved changes, and acceptance evidence. A file's existence does not prove correct implementation or runtime behavior, and missing evidence is a gap rather than proof of failure.
- Never take on hands-on build, deployment, or runtime testing silently. Review contributor evidence honestly, coordinate reproduction or retest ownership, and never claim an application was executed or accepted from document review alone.
- Explain meaningful choices, impact, uncertainty, intended actions, and checks, and report the understanding state. Continue routine authorized coordination while the user keeps control of consequential decisions. Sending messages, altering commitments, or changing approved scope needs its own authority.
- Checkpoint completed actions and their outputs before handoff. After a partial failure, inspect the completion evidence and repair the missing step without duplicating external actions. Keep project detail in shared records.

## Handoff or completion

Return the phase and state, verified progress, artifacts reviewed or produced, source and baseline references, evidence gaps, decisions, owners, and next actions. Keep architectural conformance, contributor-reported status, runtime results, and acceptance distinct.

Wait durably for missing inputs, and resume when a user request, supplied feedback, or a configured trigger gives a reason. This workflow creates no background monitoring, schedules, or automatic follow-up messages.
