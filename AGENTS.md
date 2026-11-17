# Maintaining mava-stack

These instructions govern maintenance of this public toolkit. Operational user and project configuration belongs outside it. Keep this file below 200 readable lines.

## Read first

- README.md: purpose, structure, skills, workflows, and getting started.
- PRINCIPLES.md: canonical behavior.
- ORCHESTRATE.MD: activity lifecycle, PLAN.md, and the shared execution rules every skill applies.
- memory/README.md and memory/dreaming-lw.md: memory stores and the nightly context refresh.

Preserve informed human control. Explain material choices and intended actions, and complete understood routine work without repeated confirmation. Keep instructions, evidence, assumptions, and actual execution results distinct.

## Purpose to preserve

mava-stack is a public, employer-neutral, tool-agnostic toolkit for an AI Architect. It covers discovery and presales, requirements, agentic solution design, the estimation basis, proposal, document, and deck work, delivery architecture oversight and coordination, and continuous improvement. Delivery implementation and runtime execution stay with their assigned contributors. The toolkit must remain usable across ChatGPT Work, Codex, and Claude Code through configured tools and routes.

## Public boundaries

- Keep methods independent of any employer, vendor, or individual's configuration. Use "shared team folder" for shared project storage; provider and internal team names belong in operational profiles.
- Keep customer information, credentials, internal templates, operational memory, private reflections, and release-review records out of this repository. Removing names from customer material does not make it public, so write synthetic examples independently.
- The operational working edition is a folder without Git; only the public distribution uses Git. Compare editions through revisions, checksums, or authorized review snapshots.
- Select and generalize release candidates rather than mirroring the operational folder. Keep source-to-release mappings and private publication-preparation skills private.
- Before public visibility, check supporting files, hidden notes, metadata, paths, dependencies, links, and third-party terms and attribution.
- The user reviews and approves public PRs. Never merge, enable auto-merge, or push directly to the public default branch.

## One owner per method

| File or skill | Owns |
| --- | --- |
| README.md | Reader-facing overview, skill outcomes, and the start sequence. |
| PRINCIPLES.md | Behavioral principles, including the explanation states and evidence levels. |
| ORCHESTRATE.MD | Activity lifecycle, start/resume/status, PLAN.md, waits and handoffs, shared execution rules, and the scheduling model. |
| memory/README.md | Memory stores, shared-memory contribution rules, private long-term organization, and host-native memory. |
| memory/dreaming-lw.md | The nightly refresh procedure read directly by its scheduled launcher. |
| initialize-stack | Working profile, connectors, nightly job registration, and shared bootstrap (AGENTS.md plus the MEMORY.md initialization record). |
| context | Briefs, incremental refresh, handoffs, and shared-memory maintenance. |
| search | Authorized resource discovery, source roles, version lineage, and reuse limits. |
| decompose | Guided explanation and scoped work breakdowns. |
| prepare-session | Discovery, kickoff, and solution-design session preparation. |
| requirements | Traceable requirement extraction, consolidation, and revision. |
| architect | Recommended design, meaningful alternatives, validation needs, and the estimation basis. |
| storyline | Decision narratives and the deck and formal-document production method. |
| verify | What specific evidence supports a claim, number, artifact, or result. |
| reconcile | Plan, artifact, memory, and change alignment in both directions. |
| deslop | Clearer expression without weakening meaning or necessary detail. |
| workflow-presales, workflow-delivery, workflow-evolve, workflow-reassess-stack | Their stage procedures. ORCHESTRATE.MD holds what they share. |

Reference an owner instead of restating its method. A skill keeps a short "Uses" list naming its required dependencies and directs the agent to read the applicable instructions before acting. Load another capability's full procedure only when the task calls for it.

## Authoring rules

- Package each entry as skills/<name>/SKILL.md with a lowercase hyphenated name. The frontmatter name matches the folder, and the description says when to use the skill.
- Keep every SKILL.md and this file below 200 readable lines, counting a soft-wrapped line at about 100 characters. Use clear headings, short paragraphs, and lists; remove duplication instead of packing dense paragraphs.
- Define procedures through inputs, work, outputs, evidence, and completion. Preserve ownership, waits, handoffs, retries, and resumption.
- Keep the existing files and folders. Ask before adding a folder, file, or skill unless the user's requested structure already authorizes it. There is no orchestrate directory and no dreaming skill.
- Inspect content before editing, preserve meaning when reorganizing, and remove only task-created temporary material.
- Develop skills from reviewed professional-work operations and user corrections, and exclude personal-project histories. Distinguish listing metadata, actual message review, and historical assistant reports from verified execution. Keep source-to-change evidence private and publish the generalized method.
- Keep README reader-facing. Implementation and publication notes belong here.

## Memory and scheduling invariants

- memory/LONG_TERM_MEMORY.md is the single private work-wide long-term file. The public copy is exactly zero bytes.
- Shared bootstrap writes only AGENTS.md and a Who/When/Details record in MEMORY.md. No PROJECT.md, REQUIREMENTS.md, DECISIONS.md, PLAN.md, STATUS.md, SOURCES.md, or deliverables.
- Native host memory stays host-managed. Do not relocate, synchronize, bulk-ingest, or rewrite generated native files.
- `dreaming-lw nightly memory update` runs daily at 03:00 in the user's configured time zone. initialize-stack registers it, and memory/dreaming-lw.md is its procedure. Empty personal memory never blocks an authorized shared refresh.
- Locations, time zones, sources, tools, filters, templates, and authority are operational configuration. Authoring the toolkit authorizes no memory capture, population, schedule change, or operational configuration change.

## Validation before handing back changes

- All 15 entries have valid frontmatter (name matches folder, description present), and README lists the same 15.
- Local links and heading anchors resolve.
- Every SKILL.md and this file is below 200 readable lines.
- memory/LONG_TERM_MEMORY.md is exactly zero bytes.
- The schedule name and time, record names, ownership, and deck rule are stated consistently.
- Changing product facts come from current primary sources. Report limitations accurately.

## Status

- All 15 skill and workflow entries listed in README are authored.
- Independent synthetic chains cover requirements to architecture; verification, reconciliation, and content cleanup; and session preparation with an actual DOCX copy, adaptation, and render plus the missing-PPTX-reference fallback. These checks do not establish live connector access, PowerPoint production, or customer acceptance.
- Host installation, operational profile and shared-folder access, live initialization, and real workflow outcomes remain unvalidated.
- App schedules are managed through the supported automation tools. The existing nightly routine and monthly maintenance schedules keep their user approval and source-scope boundaries.
