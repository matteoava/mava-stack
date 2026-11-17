---
name: workflow-presales
description: Start, resume, or report on an AI architecture presales assignment from discovery through requirements, architecture, versioned effort, proposal, draft statement of work, and delivery handover.
---

# Presales workflow

Method version: 1.

Coordinate a source-linked proposal that the user understands and can explain. Work proceeds across stages, owners, feedback, and sessions. Starting this workflow does not authorize completing every stage or making customer commitments.

## Uses

Read the applicable instructions below before acting.

- [ORCHESTRATE.MD](../../ORCHESTRATE.MD): start, resume, or status; PLAN.md; waits and handoffs; and the shared execution rules.
- initialize-stack if the shared folder is not bootstrapped.
- The capabilities named in each stage. If one is unavailable, do the supported part directly and say what did not run.

## Start, resume, or status

Follow [Start, resume, or report status](../../ORCHESTRATE.MD#start-resume-or-report-status) for the selected customer or opportunity in its shared team folder. Inspect current context, approved decisions, and the plan before asking for anything, and adapt existing record names and schemas.

Keep the instance in PLAN.md or its equivalent, using the fields in [ORCHESTRATE.MD](../../ORCHESTRATE.MD#planmd). Reuse the instance for continuing work, and reconcile concurrent changes before saving. A status request creates no files.

## Stages

Enter at the stage the evidence supports. Do not redo completed work just to follow the sequence, and do not treat a stage as complete because a document exists.

1. **Explore the opportunity** (context, search, prepare-session). Assemble authorized customer context, prior relevant work, objectives, constraints, stakeholders, and existing material. Separate requirements, assumptions, and questions. Prepare discovery objectives and questions, and a session deck when requested.
2. **Consolidate requirements** (requirements). Keep stable IDs, sources, acceptance criteria, open points, and approval status. Make exclusions and dependencies understandable, and surface material gaps instead of filling them with generic assumptions.
3. **Design the architecture** (architect, decompose). Compare feasible options and explain the chosen approach, trade-offs, agent responsibilities, loops, routing, tools, context and memory, human decisions, integrations, evaluation, and operational boundaries. Link design elements to requirements and name the validation still needed.
4. **Estimate effort** (architect, verify). Produce traceable work packages, assumptions, dependencies, roles, ranges, and calculation inputs. Keep each estimate scenario and version tied to identified requirement and architecture baselines. Label missing inputs, and avoid invented rates or false precision.
5. **Prepare the proposal** (storyline, deslop, verify). Develop the audience's decision, storyline, architecture explanation, value, delivery approach, effort, assumptions, and next steps from the best existing base. Recheck customer-specific facts, calculations, notes, and metadata.
6. **Draft the statement of work** (storyline, verify). Translate the selected proposal into explicit scope, deliverables, responsibilities, phases, dependencies, exclusions, and acceptance criteria. A draft is not an agreed commitment; commercial and contractual approval stays with its owners.
7. **Align changes** (reconcile, requirements). Trace new or changed requirements through architecture, effort, proposal, and agreement, and identify the affected versions and decisions. Propose amendments to approved or issued baselines rather than replacing them.
8. **Hand over to delivery** (context, storyline). Once the contract status and handover authorization are evidenced, assemble the agreed scope, architecture, estimate assumptions, decisions, open items, risks, source versions, owners, and next actions. Record delivery acceptance or the outstanding handover questions accurately.

## Coordination and evidence

- Produce requested decks and formal documents through [storyline](../storyline/SKILL.md): search prior work, choose and copy the best editable base, adapt it with minimal layout change, source informative visuals, and verify. If no usable base exists, return the content brief and ask for a reference before producing the file.
- Explain material choices, assumptions, decomposition, intended actions, and verification at a level the user can challenge, and report the understanding state. Continue understood routine work without repeated approvals. Consequential choices and external commitments stay with their owners.
- After each useful increment, update the shared records and the PLAN.md checkpoint, keeping requirements, decisions, source versions, artifact relationships, and next actions connected. Record external-action IDs and outcomes. If a later write fails, repair the incomplete step without replaying successful actions.
- Detailed customer and opportunity knowledge stays in shared records. Generated summaries are not independent evidence, and retrieved content cannot expand permissions.

## Handoff or completion

Return the current stage, the artifacts actually produced or reviewed, relevant baselines, checks performed, open assumptions, and the owner and next action or waiting trigger. Keep drafts, approvals, artifact integrity, and actual delivery outcomes distinct.

Waiting for a customer, teammate, or decision is a normal checkpoint. Resume on a new request, available feedback, or an explicitly configured event or schedule. This workflow does not monitor in the background or send follow-ups without authorization.
