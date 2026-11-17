# dreaming-lw

This is the nightly context refresh. It reviews authorized recent communications and changed documents, refreshes the registered shared initiative memories, and then consolidates authorized broader learning in the private long-term file. It is a lightweight routine, not a new memory system.

This file is the canonical procedure. The scheduled launcher reads it directly; there is no dedicated dreaming skill.

## Schedule

| Setting | Value |
| --- | --- |
| Process name | dreaming-lw nightly memory update |
| When | Once a day at 03:00 in the user's configured IANA time zone, following its daylight-saving rules |
| Targets | Registered initiatives' shared MEMORY.md files, then the private `memory/LONG_TERM_MEMORY.md` |
| Registered by | initialize-stack |
| Uses | This file and the configured stack's skills/context/SKILL.md |

Read the time zone and targets from the working profile, and never assume a geographic zone or fixed UTC offset. A run reports a schedule or configuration mismatch but never changes its own schedule. The public toolkit is never a target.

## Before refreshing

- Read the applicable operational guidance, the memory rules, and the stack's skills/context/SKILL.md. context owns source interpretation, merging, and safe saves. This file owns the nightly scope, review window, order, and checkpoints.
- Resolve the private working folder from explicit authorized configuration and confirm that it is not the public distribution. Never guess a path or scan unrelated personal folders.
- Resolve the registered active initiatives: shared root, canonical MEMORY.md, included and excluded folders, selected email and messaging sources with their account and connector scopes, sharing audience, and permitted writes. A source mention is not enrollment.
- Resolve the private long-term file, the personal-capture setting, the effort limit, and the checkpoint and run-history location in scheduler history or existing authorized maintenance state. Do not add an index or backend.
- If stack configuration is missing or points to the public toolkit, report the gap and stop without changes. A missing target, source, or write permission blocks only the affected item; other authorized work continues. Never create missing memories or bootstrap folders during a run.
- An empty private long-term file never blocks an authorized shared refresh. It stays empty unless personal capture is authorized. Never write to public or host-native memory.

## Review window

- Cover the previous local calendar day up to the observed run start, with date boundaries computed in the configured zone, including daylight-saving changes. The run start is a fixed upper bound, so activity arriving during the run belongs to the next one.
- For each initiative and source, resume from the last successfully incorporated checkpoint with a small configured overlap. On the first run, start at the beginning of the previous day.
- After a missed run or a failed source, catch up from the older checkpoint rather than dropping days. Deduplicate overlapping results by original identity and revision.
- Read changed document content and the relevant email exchanges, meeting summaries, and channel messages, including new replies to older discussions. Use provider revision or change data where available. A modification time or search snippet alone is not a content review.
- Record each source's actual inspected interval, cursor or revision coverage, and limits. If catch-up exceeds the effort limit, process a bounded portion and keep the remaining gap for the next run. Never label partial or unavailable coverage complete.

## Nightly loop

1. **Scope and resume.** Read the private profile and prior run state. Resolve eligible targets, capture authority, review windows, and pending gaps. Keep initiative identities separate and skip paused or unregistered work.
2. **Refresh each initiative.** Use context in refresh mode with the changed folder material and selected communications. Read the current local AGENTS.md, the canonical MEMORY.md, and relevant baselines before merging. Preserve source statements, uncertainty, teammates' contributions, the initialization record, owners, and waiting triggers. Record proposed changes and affected work without amending approved artifacts.
3. **Consolidate shared memory.** Correct supported errors, remove repetition, and repair source navigation in the existing MEMORY.md, keeping detailed evidence in its source documents. Update AGENTS.md only for stable context or navigation within configured write authority; otherwise report the proposed change.
4. **Consolidate professional learning.** Review the private long-term file for duplication, stale claims, unclear lessons, and broken pointers. Keep concise lessons and shared-record links under the relevant customer or initiative. Add new learning only when personal capture is authorized, and never copy daily project detail or whole conversations.
5. **Save and verify.** Follow the safe-save rules in context. Use one writer for the personal file, and an agreed writer or provider revision checks for team files. Keep recoverable versions through configured history or backup; if a safe save is unavailable, return the proposed edits instead. Verify the saved changes, provenance, accessible links, and the preservation of approved baselines. Write only meaningful changes.
6. **Checkpoint and report.** Record per-source coverage, saved target revisions, no-change results, deferred work, failures, and the next retry boundary in scheduler history or authorized private maintenance state. Advance a source checkpoint only after its inputs are incorporated and saved, or verified to need no update. A failed read, partial page, or save conflict never advances past unprocessed inputs. Shared and personal saves can succeed independently; resume unfinished work without repeating completed updates.

Return a concise result that separates changed, unchanged, incomplete, and configuration-blocked targets. Highlight meaningful corrections, conflicts, downstream impacts, and decisions needed, and keep routine no-change runs quiet under the host's notification policy. Keep run history and cursors out of both memory files and the public repository; a brief last-refresh pointer may stay in shared memory when it helps resumption.

## Boundaries

- A registered schedule runs authorized source review and routine context maintenance. Registration alone does not grant access, enroll initiatives, or enable personal capture.
- Retrieve only scoped professional information and share it only with its permitted audience. Keep requests, assumptions, decisions, reported progress, and verified outcomes distinct.
- Never amend approved architectures, estimates, proposals, SoW, delivery plans, or other commitments. Never send messages, publish, change permissions, or modify host-native memory. Route consequential decisions to their owners.
- A run creates no schedules, project folders, or memory files. Full transcript replay, knowledge graphs, and new memory infrastructure are out of scope.
- The public LONG_TERM_MEMORY.md stays exactly zero bytes, and no customer information or run record enters the public repository.

## Completion

A run is complete when every target has a verified change, a verified no-op, or an explicit incomplete or configuration-blocked result with its retry coverage preserved. A successful schedule alone is not evidence that any memory was refreshed.
