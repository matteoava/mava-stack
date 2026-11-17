# mava-stack

Skills and workflows for AI architects working across discovery, presales, delivery oversight, and continuous improvement.

Turn customer context into clear requirements, defensible architectures, traceable estimates, and decision-ready material. Keep work resumable across people, agents, tools, and time, with evidence and informed human control. Delivery implementation and runtime execution stay with their assigned contributors.

The toolkit is employer-neutral and tool-agnostic. It works in ChatGPT Work, Codex, and Claude Code through whatever tools and connectors you configure.

## Directory structure

~~~text
mava-stack/
├── README.md
├── PRINCIPLES.md
├── AGENTS.md
├── ORCHESTRATE.MD
├── memory/
│   ├── README.md
│   ├── dreaming-lw.md
│   └── LONG_TERM_MEMORY.md
└── skills/
    ├── initialize-stack/SKILL.md
    ├── workflow-presales/SKILL.md
    ├── workflow-delivery/SKILL.md
    ├── workflow-evolve/SKILL.md
    ├── workflow-reassess-stack/SKILL.md
    ├── context/SKILL.md
    ├── search/SKILL.md
    ├── decompose/SKILL.md
    ├── prepare-session/SKILL.md
    ├── requirements/SKILL.md
    ├── architect/SKILL.md
    ├── storyline/SKILL.md
    ├── verify/SKILL.md
    ├── reconcile/SKILL.md
    └── deslop/SKILL.md
~~~

- **PRINCIPLES.md** defines the shared behavior.
- **ORCHESTRATE.MD** explains how activities start, wait, resume, and hand over, and lists the rules every skill shares.
- **memory/** holds the memory guide, the nightly refresh instructions, and the empty long-term memory file.
- **AGENTS.md** governs maintenance of this toolkit.
- **skills/** holds one folder per capability or workflow. Each skill owns its procedure.

## How it works

**You stay informed and in control.** Agents explain meaningful choices and actions step by step, iterate on your feedback, and tell you whether understanding is confirmed or a clarification is still pending. Routine work you already understand proceeds without repeated approval.

**Work is a resumable activity.** Each customer activity, such as a presales opportunity, is set up once. Its state (stage, owners, baselines, completed actions, waits, and next trigger) lives in the shared team folder, so any teammate, session, or machine can pick it up without resetting progress.

**Memory stays simple.**

- One shared MEMORY.md per initiative, in its shared folder. Initialization records only who, when, and what was set up. Later authorized work adds concise, source-linked knowledge.
- One private `memory/LONG_TERM_MEMORY.md` for durable professional learning, organized internally by customer or initiative. The distributed file is empty.
- Scoped AGENTS.md files in the shared root and each authorized subfolder carry initiative context and point to the right MEMORY.md.
- Host-native memory stays under each host's control.

**Context refreshes nightly.** The process `dreaming-lw nightly memory update` runs at 03:00 in your time zone. It reviews authorized recent communications and changed documents, refreshes registered shared memories, and then consolidates broader learning where personal capture is authorized. It resumes from per-source checkpoints, so missed runs and unavailable sources do not silently lose updates.

## Skills

| Skill | When to use it | What it produces |
| --- | --- | --- |
| initialize-stack | Set up your working environment, or bootstrap a shared customer activity, opportunity, or project. | Working profile, connectors, and the nightly schedule; AGENTS.md populated from existing files and relevant email or channel discussions; MEMORY.md recording who, when, and setup details. |
| context | Start or resume work, absorb new evidence, or hand off an activity. | A source-backed brief with the current basis, changes, conflicts, affected work, and the next owner or trigger, plus authorized shared-memory updates. |
| search | Find prior decks, architectures, estimates, templates, or similar customer work. | Ranked original resources with inspected evidence, source roles, versions, adaptation needs, and sharing limits. |
| decompose | A problem, solution, or plan is hard to understand, explain, or delegate. | A step-by-step explanation adapted to you and refined until understood, and a scoped work breakdown when needed. |
| prepare-session | Prepare a discovery, kickoff, or solution-design discussion. | A flow matched to the phase, precise questions and decision roles, capture guidance, and requested materials. |
| requirements | Extract or consolidate customer inputs, or update a specification. | Source-linked requirements with stable IDs, scope and approval states, acceptance criteria, open questions, and version lineage. |
| architect | Translate requirements into an agentic design and estimation basis. | One recommended approach with alternatives and trade-offs, the solution views, validation needs, and traceable effort assumptions. |
| storyline | Produce or revise customer or executive decks and formal documents. | A decision narrative and an editable artifact adapted from the best existing base, with informative visuals and verified content and layout. |
| verify | Check a claim, calculation, artifact, or reported result before relying on it. | Supported, contradicted, or insufficient-evidence findings with independent checks and explicit limits. |
| reconcile | Compare the plan with artifacts, memory, and approved changes. | A two-way alignment view with gaps, unplanned work, stale memory, affected versions, and next owners. |
| deslop | Improve AI-generated or overworked material before it reaches a reader. | Clearer writing that keeps the facts, qualifications, scope, and useful detail. |

## Workflows

A workflow is a recurring process with stages, owners, feedback, and waiting states. Each workflow is a skill, so you can select it directly.

| Entry | Use | Result |
| --- | --- | --- |
| `workflow-presales` | Develop an opportunity from discovery to delivery handover. | Aligned requirements, architecture, versioned estimates, proposal, draft SoW, and handover evidence. |
| `workflow-delivery` | Coordinate delivery from agreed scope and architecture. | Phased plans, architecture decisions, evidence reviews, change alignment, and handover. |
| `workflow-evolve` | Assess what a new capability or product change means for existing work. | A source-backed impact analysis with affected work, options, and recommended actions. |
| `workflow-reassess-stack` | Review model and harness changes across the stack. | A capability assessment, representative comparisons where possible, regressions, and proposed improvements. |

## Decks and documents

For a new deck or formal document, the agent first searches authorized prior work across customers and projects. It inspects the candidates, chooses the best editable base, and explains why. It then copies that base and adapts the content with minimal layout change. Later revisions start from your current human-edited version, and originals are never overwritten.

Slides stay informative and graphical. Existing layouts and assets come first; missing screenshots, icons, or images are sourced online with attention to authenticity, version, and usage terms. Inherited customer text, numbers, notes, hidden content, and metadata are cleaned, and the content and rendered layout are verified.

If no usable reference exists, the agent prepares the content brief and asks you for a reference before producing the file. storyline owns this method.

## Get started

1. **Make the skills available.** Connect the skill folders through your host's supported skill or plugin setup. A folder under `skills/` is not installed automatically. In Codex, `/skills` lists skills and `$name` mentions one; other hosts provide their own skill selection.
2. **Set up your environment.** Ask `initialize-stack` to set up the stack. Choose your email and team-messaging connectors, eligible initiative folders, and what the nightly refresh may read and update. The agent verifies access, schedules `dreaming-lw nightly memory update` at 03:00 in your time zone, and reports any gaps.
3. **Bootstrap a customer activity once.** Give it the shared folder and the source scope. The agent reads the existing files and related communications, fills AGENTS.md in the root and subfolders, and records only who, when, and setup details in MEMORY.md.
4. **Run the workflow.** For example, ask `workflow-presales` to begin discovery. It reads the local guidance and memory, explains the next work, and creates requirements, plans, or other records only when that work needs them.
5. **Continue from shared state.** Ask the same workflow to resume or report status after new evidence or feedback. Rerunning initialization fills gaps without resetting progress.

Shared-folder initialization adds only this within your existing folders:

~~~text
initiative/
├── AGENTS.md
├── MEMORY.md
└── existing-subfolder/
    └── AGENTS.md
~~~

Example request:

> initialize-stack: Set up my working environment using my chosen email and team-chat connectors. Inspect this opportunity's shared folder and search related emails and channel discussions within the agreed scope. Use them to populate AGENTS.md, record only who, when, and setup details in MEMORY.md, ask for missing essentials, and tell me the next workflow step.
