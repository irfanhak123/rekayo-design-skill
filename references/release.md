# Evidence, reporting, release and change

## Records proportional to work

Keep small tasks in one existing state record. A larger project may split requirements, interfaces, source register, task board, toolchain, paths, metrics and handoffs as they become useful. Project guidance stays short and links to authoritative records. Reuse the existing workspace layout rather than imposing a second structure.

Engineering quantity record: `id | value | unit | evidence kind | source/result path | input revision | uncertainty/limit`. Evidence kinds: SOURCE, CALCULATION, SIMULATION, MEASUREMENT, ASSUMPTION. A named reproducible calculation/result file can support several table entries. Never relabel a failed check as success.

Handoff contract: `status; goal/requirement IDs; input revisions and absolute paths; output paths; checks actually performed; findings and units; assumptions; errors; open decisions; next actions`. Review reports are inputs, not approvals: the coordinator inspects representative native files and raw results. Preserve one writer per native file, explicit ownership, and locks when concurrent edits require them.

Record available model IDs, effort settings, tool versions, elapsed time, retries, and actual token usage only when exposed by the host. Mark unavailable data unavailable. Avoid a reporting system that costs more than the task.

## Reporting and baselines

Use the format requested. Markdown suffices for ordinary work; LaTeX source plus PDF and a presentation belong to requested formal reporting. Compile a one-page test before a substantial LaTeX report, then inspect the actual final output. For a full engineering demonstrator, cover requirements, architecture, purchased parts, interfaces, structural alternatives and mesh/sensitivity checks when performed, electronics checks, assembly, decisions, limitations and a physical validation plan. Link numerical claims to sources or reproducible results. Explicitly mark omitted/unrun routes.

At a requested release, collect native editable files, exports, report/manual where applicable, per-requirement verification status, reproduction instructions and a short demo runbook. Hash the released files with a SHA-256 manifest; verify it. Freeze the released folder. Unfinished requirements remain PARTIAL, FAIL, BLOCKED or NOT RUN. A file export, release folder or report is not submission, approval, certification, or production readiness.

## Changes

Run only after a clear user change request; documentation examples are not authorization. Stay with the current coordinator and reuse appropriate tools/specialists. Preserve the baseline or dated pre-change snapshot, open a numbered change record when project scale warrants it, assess affected requirements/parts/interfaces, revise and compare old/new behavior, rerun affected checks, update documents, and publish a new revision when requested. Never overwrite an immutable release or silently reset later work.

For a restart, save the smallest useful resume record: current mode, decisions, input/output revisions, pending checks, blocker and exact next action. Explain a required user action once, with how to verify completion; continue unaffected work.
