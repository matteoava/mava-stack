# Orchestration

This file explains how workflows, skills, people, and feedback combine into activities that continue across sessions, machines, and owners. Each workflow's procedure lives in its skill under skills/workflow-*/. This file holds the shared operating model and the execution rules every skill applies.

## Method and instance

A workflow skill is a reusable method. An activity instance applies that method to one distinct assignment, such as one presales opportunity. The instance's state lives in the initiative's shared folder, not in the skill or in a chat. One customer can have several activities.

For example, workflow-presales describes the path from discovery to handover. One opportunity's PLAN.md records that discovery is waiting for a customer answer, who owns that answer, the scope agreed so far, and which architecture or estimate will need revisiting.

## Activity lifecycle

1. **Stack setup (once per user).** initialize-stack configures the working profile, communication connectors, and the nightly context refresh.
2. **Activity bootstrap (once per activity).** initialize-stack inspects the shared folder and the selected communications. It writes AGENTS.md in the root and each authorized subfolder with the initial activity context (objective, phase, chosen workflow, known owners, and boundaries). It writes MEMORY.md with only who, when, and setup details, and creates nothing else.
3. **First workflow run.** When execution records are needed, the workflow creates or reuses PLAN.md or an existing equivalent. Other skills create requirements, decisions, or status records only when their work calls for them.
4. **Resume.** Later sessions, skill calls, and teammate handoffs continue the same instance from its last evidenced checkpoint.
5. **Complete or hand over.** The workflow records the outcome, open items, and the receiving owner.

## Start, resume, or report status

Every workflow begins the same way:

- Read local AGENTS.md, the shared MEMORY.md it points to, PLAN.md if present, and the authoritative records they reference.
- For start or resume, use initialize-stack for missing shared bootstrap in the explicitly selected folder. A status request only reports missing setup; it creates no files. Never invent a destination or facts.
- **Start:** establish the outcome, current stage, available evidence, owners, and understood action boundaries. Enter at the stage the evidence supports; do not redo completed work just to follow the sequence.
- **Resume:** load the existing instance and check changed inputs, baselines, pending feedback, and completed-action evidence before continuing the affected stage.
- **Status:** report the evidence-backed position, gaps, dependencies, and next actions. Create no files and start no new work.

A new chat or agent never repeats bootstrap, resets progress, or creates a second instance. Create a new instance only for a genuinely distinct activity. When new evidence or decisions arrive, update only the arrangements they affect. For example, a customer clarification can reopen requirements, identify the affected architecture and estimate, and resume proposal work within the same activity.

## PLAN.md

Keep the instance in PLAN.md or the existing equivalent, reusing its names and schema:

- Instance ID, workflow method name, and method version.
- Current stage and state: active, waiting, blocked, or complete.
- Owners per work item, including agreed joint ownership.
- Baseline references with their versions.
- Completed action IDs with their outputs and evidence.
- Waits: what is missing, who owns it, and the trigger that resumes the work.

Keep the method in its skill and the execution state with the project. Do not copy the procedure into project records.

## Waits, retries, and handoffs

Waiting is a normal checkpoint. Record what is missing, who owns it, and what resumes the work: a user request, a configured event, or a schedule. A Markdown procedure is not a running service, so nothing monitors in the background unless a scheduler is configured for it.

After a partial failure, inspect the completion evidence and repair only the missing step. Never blindly repeat an external action.

A handoff carries the instance ID, current basis, completed actions, open questions, and the receiving owner's inputs and expected outputs, not just a link to a previous chat.

## Shared execution rules

Every skill applies these rules. Skills state only their own additions.

- **Read before acting.** Inspect current guidance, memory, and original sources. Ask only about gaps that remain and would materially change the result, and continue independent work meanwhile.
- **Explain.** Explain material choices and intended actions step by step (principle 7), and report whether the explanation was delivered, understanding is confirmed, or a clarification is pending.
- **Evidence.** Keep source identity, version, and inspection depth, and label evidence levels (principle 8). Report coverage gaps instead of claiming that something does not exist.
- **Safe saves.** Reread the current revision before writing. Preserve teammates' edits and attribution and merge compatible changes. If a conflict cannot be resolved, report it with the proposed update instead of overwriting. Use an agreed writer or provider revision checks, because file synchronization is not locking. Report exactly which saves succeeded.
- **Records.** Create only the records the work needs, reuse existing names and conventions, and keep detailed project content in the shared folder. Memory updates follow memory/README.md.
- **Decks and formal documents.** Produce them through storyline: search prior work, choose and copy the best editable base, adapt it with minimal layout change, and validate. If no usable base exists, return the content brief and ask for a reference before producing the file.
- **Missing capability.** If a named skill, connector, or production route is unavailable, perform the supported part directly and state what did not run. Never claim that an absent tool executed.
- **Authority.** Saving a file does not authorize sending messages, publishing, approving, amending baselines, changing permissions, or creating schedules. Delivery implementation and runtime execution stay with the assigned contributors.

## Workflow entries

| Skill entry | Responsibility |
| --- | --- |
| workflow-presales | Discovery, requirements, architecture, effort, proposal, draft SoW, and handover. |
| workflow-delivery | Architecture oversight, delivery planning, dependencies, evidence, and handover. |
| workflow-evolve | Impact of new capabilities and changes on current work. |
| workflow-reassess-stack | Periodic assessment of model and harness changes across the stack. |

Each host must expose the skill folders through its supported skill or plugin setup. A folder under skills/ is not registered automatically, so verify that a skill is available before relying on it. In the Codex CLI and IDE, /skills lists skills and $name mentions one; see the [Codex skill documentation](https://learn.chatgpt.com/docs/build-skills). Other hosts use their own skill discovery.

## Scheduling

The only stack-wide schedule is `dreaming-lw nightly memory update`, which runs daily at 03:00 in the user's configured IANA time zone. initialize-stack registers it, and its launcher reads memory/dreaming-lw.md directly. Bootstrapping an initiative never creates another job.

Recurring workflow cadences, such as a monthly stack reassessment, are host scheduler settings. Skills do not create or change schedules without explicit authorization, and a registered schedule is not evidence that a run happened.
