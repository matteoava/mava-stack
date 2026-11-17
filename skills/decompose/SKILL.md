---
name: decompose
description: Explain a complex problem, solution, or plan step by step, adapting structure and detail to the user's context and iterating through feedback until the material points are understood. Use for guided explanations and scoped work breakdowns; decomposition does not authorize execution or design changes.
---

# Decompose

Keep the user fully informed about the whole, how its parts fit, and what needs deciding or doing next. Choose useful detail rather than maximizing tasks or introducing a new framework.

## Uses

Read the applicable instructions below before acting.

- [Principle 7](../../PRINCIPLES.md#7-explain-until-the-user-understands): the explanation loop and its three states.
- [ORCHESTRATE.MD shared execution rules](../../ORCHESTRATE.MD#shared-execution-rules).
- [storyline](../storyline/SKILL.md) for a formal explanation document or deck.

## 1. Establish the question and basis

- Identify the objective, audience, decision, requested output, and what is currently hard to explain or delegate.
- Assess the user's role, domain familiarity, existing understanding, questions, and feedback from available context. Keep uncertain assumptions about what they know provisional.
- For initiative work, read the local AGENTS.md, shared MEMORY.md, and relevant requirements, architecture, or plans.
- Separate agreed scope and constraints from suggestions, assumptions, backlog, and unknowns. Ask only when the missing answer would change the breakdown, and keep explaining around explicit gaps.
- A standalone explanation needs no project initialization. Do not turn an explanation request into a full delivery plan.

## 2. Choose the useful lens

| Need | Break down |
| --- | --- |
| Understand a problem | Desired outcome, affected people and process, current difficulty, constraints, subproblems, uncertainties, and the decisions that unlock progress. Separate evidence from hypotheses about causes. |
| Understand a solution | End-user outcome and journey, meaningful capabilities, shared services, information and context, actions, outputs, controls, and how they interact. |
| Organize a plan | Outcomes or phases broken into work packages and tasks, with deliverables, dependencies, ownership, completion evidence, and waits. |

Combine lenses only when that helps. Start from the business outcome, explain why the chosen split suits this audience, and reuse meaningful existing names and levels rather than imposing a fixed hierarchy.

## 3. Preserve meaning while splitting

Split where a separate decision, deliverable, responsibility, interface, or verification makes the work easier to understand or coordinate. Make exclusions visible.

- A customer journey is different from a reusable capability, internal component, shared foundation, or cross-cutting service. A component may support only part of the outcome.
- Keep alternative approaches apart from components that must coexist, and name the decision and evidence needed to choose. Do not fold every option into committed scope.
- Preserve agreed compound or atomic operations. Internal parts do not become separate customer journeys or new scope.
- Represent shared work once and link its consumers, so repeated references do not count as separate deliverables or duplicate effort.
- Preserve existing contracts, state variables, interfaces, constraints, and behavior. Simplifying an explanation does not authorize refactoring the implementation.
- Show sequence, parallel work, branches, feedback loops, approval points, and waits where they matter. A linear diagram must not misrepresent an interactive system.
- Parallel contributors do not imply that runtime operations can run concurrently. Check dependencies and platform constraints first, and include integration and end-to-end validation; finished components alone do not prove a working journey.
- Mark a grouping or relationship as proposed when sources do not establish it. Do not invent a new architecture, runtime agent, or workflow node for each item.

## 4. Make coordination actionable when requested

For work to be delegated, use the existing planning format and keep the fields needed to act:

| Element | Clarify |
| --- | --- |
| Purpose and scope | Parent outcome, included work, exclusions, and relevant source or baseline IDs. |
| Inputs and dependencies | Required artifacts, access, customer inputs, upstream work, external decisions, and whether parallel work is possible. |
| Output and completion | The deliverable, review or acceptance evidence, and who can establish completion. Investigation is not build, and build is not validation. |
| Ownership | Confirmed owner, contributors, integration responsibility, and decision authority. Label proposed or unknown assignments. |
| Resumption | Current evidenced state, next action, waiting input and its owner, and the resuming trigger. |

- Preserve agreed joint ownership and expose unresolved coordination points without reassigning people. Architecture oversight does not mean owning implementation, runtime tests, or another team's commercial work.
- Keep unknown effort, dates, availability, and approval explicit. A proposed sequence is not a committed schedule; list the inputs estimation still needs.
- Reuse activity and work-item IDs, existing progress, and human edits. A new breakdown must not reset completed work or duplicate assignments. Flag status conflicts instead of asserting a new state.

## 5. Explain, check understanding, and iterate

Pick the best starting form for the context: a walkthrough for an unfamiliar process, a relationship diagram for interacting parts, a comparison for alternatives, or a work-package view for coordination. Change it when feedback suggests a better one.

1. **Check before presenting.** Verify source accuracy, scope coverage, sequence, relationships, and missing links. Keep uncertainty visible where evidence is missing.
2. **Orient.** Briefly explain the whole outcome and why it matters, introducing needed terms in familiar language.
3. **Walk through the parts.** For each meaningful step, cover its purpose, actor, input, what happens, output, and how it connects to the next. Expose relevant choices, rationale, assumptions, consequences, exceptions, and controls, and keep real branches and loops.
4. **Use feedback.** Invite focused clarification where understanding is uncertain. Use the user's questions, corrections, and choices to find the unclear point, and revisit it with a better example, representation, or depth rather than repeating the same explanation.
5. **Confirm.** Look for substantive feedback, an informed choice, or explicit confirmation for the stated scope. The user should be able to follow and challenge the material steps, decisions, consequences, and action boundaries. No quizzes, formal teach-backs, or approval after every step.
6. **Continue or wait.** Repeat for unresolved points. If a user response is needed, state the gap and the next question, record where the explanation stopped, and hold dependent work while continuing independent authorized work.

Report the state: **explanation delivered**, **understanding confirmed** for the stated scope, or **clarification pending**. Self-review, silence, or approval of the presentation does not show that the user is informed. Factual unknowns stay visible even when their explanation is understood.

For delegated work, also check that a contributor can identify the input, expected output, owner, completion evidence, and next handoff. A material change reopens the affected explanation.

## Output and boundaries

Return a proportionate explanation or work breakdown, source and baseline references, material assumptions and decisions, the understanding state, and the next useful action. An explanation can stay in chat; do not create a plan, matrix, or decision log just to complete the skill.

When saving or updating a plan is requested, reuse its existing record and conventions, preserve baselines, IDs, contributors, and completed-action evidence, and save under the shared rules. Update shared memory only within its capture mandate.

Decomposition does not execute tasks, send assignments or messages, start monitoring, or amend approved scope. Requirements, design choices, estimation, reconciliation, and deck production stay with their owning skills.
