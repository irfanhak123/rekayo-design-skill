---
name: rekayo-design-skill
description: Develop physical products through concept exploration, evidence-based selection, detailed engineering, and controlled revisions. Scale CAD/FEM, electronics, assembly visualization, tools, and specialists to the task. Use for engineering design work; no CFD.
---

# Rekayo Design Skill

Deliver the requested engineering outcome with the smallest useful workflow. Start with one coordinating agent; add tools, documentation, fidelity, and specialists only when they resolve a concrete need. This skill contains process, never a stored product brief.

## Scope and mode

Read the current brief, existing files, local instructions, and latest handoff. Preserve user edits and established decisions. Infer the immediate deliverable, constraints, purchased parts, open variables, and evidence needed; ask only for consequential information inspection cannot supply. Use the user's language. Do not turn a design question into a full product-development assignment.

Use the requested mode, or choose and state one briefly:

| Mode | Work | Stop or switch when |
| --- | --- | --- |
| **Explore** | Generate meaningfully different principles or architectures at low fidelity. Start with three if breadth is unspecified; expand only into uncovered promising regions. Avoid cosmetic variants. | Alternatives cover the important trade-offs or the agreed effort limit is reached. |
| **Compare** | Apply the same requirements, interfaces, load cases, and evidence standard. Eliminate infeasible options, expose uncertainty and trade-offs, recommend a shortlist. | Evidence supports a choice, or identify the smallest test that could change it. |
| **Detail** | Develop the selected concept through editable artifacts, calculations, interfaces, and relevant verification. Keep unselected choices open. | The requested acceptance checks pass or remaining limits are explicit. |
| **Change** | Preserve the baseline, assess affected requirements/interfaces, revise, compare, and reverify. | A new revision and its verification record are ready. |

Do not silently select a winner during exploration or reopen a settled architecture during detail work. A recommendation is not user approval. Continue through selection when the user delegated that decision. Reopen only the affected issue when new evidence undermines feasibility; name the reason. For mixed tasks, explore uncertain subsystems while detailing settled ones. Timebox breadth and depth separately; numerical mesh convergence is a different concept from choosing a design.

## Lean execution

1. Work toward the smallest next result that reduces uncertainty or completes the request. Use rough calculations before expensive models. Do not build future upgrades without a request.
2. Reuse working software, sources, files, and validated results. Read only the relevant reference below. Batch independent queries; request bounded outputs. Save raw logs to files and summarize findings rather than repeatedly loading them.
3. Keep one compact project state record for decisions, requirement IDs/checks, assumptions, interfaces, evidence paths, and next action. Reuse an existing record. Split out task boards, source registers, metrics, locks, or handoffs only when size, concurrency, or release needs justify them. Create directories as needed.
4. Delegate only a bounded independent task whose expertise or parallel benefit exceeds its coordination cost, within host permissions. Start with one specialist; expand only after a demonstrated need. Specialists do not recursively delegate by default. Without delegation, do the work sequentially and say so; do not simulate agent activity. Give each real worker only its goal, input revisions/paths, writable outputs, acceptance checks, resource budget, and handoff contract. Verify its actual tool access and inspect its results.
5. Use one writer per native application document. Coordinate ownership; use locks for concurrent work. Agree cross-discipline interfaces before parallel edits. Schedule heavy solves/renders against available resources. After three failed repairs without new evidence, preserve diagnostics and change approach or report the blocker.

## Tools and evidence

Install only prerequisites for the requested capabilities, within existing authorization. Setup requests may prepare all requested routes without creating a product. Read [toolchain.md](references/toolchain.md) for discovery, installation, MCP configuration, and real smoke tests. Use the host's supported configuration; do not assume Claude-specific paths or agent features. CLI automation is valid but is not an MCP connection. Installed, configured, connected, and verified are separate states.

Trace engineering quantities to **SOURCE**, **CALCULATION**, **SIMULATION**, **MEASUREMENT**, or **ASSUMPTION**, with units, revision, and evidence. Shared table/column labels suffice. Never invent tool results, datasheets, tests, approvals, or production readiness. Use **PASS / PARTIAL / FAIL / BLOCKED / NOT RUN** against explicit checks. Inspect output content; a successful exit or running process alone proves little. Simulations, rule checks, and visualization do not establish physical validation.

Read only the needed technical procedure:

- [Mechanical design and FEM](references/mechanical.md): editable CAD, fair geometry comparisons, mesh convergence, sensitivity, and integration.
- [Electronics](references/electronics.md): real schematic/PCB, electrical calculations, component evidence, mechanical interfaces, ERC/DRC.
- [Assembly and visualization](references/assembly.md): released geometry, dimensional fidelity, access, exploded views, manuals, and optional animation.
- [Evidence, release, and change](references/release.md): handoffs, reporting, checksums, reproducibility, metrics, immutable baselines, controlled revisions.

Run route-specific verification when that route is used; do not require every application before a simple task. Keep sensitive data out of reusable skills and logs. No CFD setup or work. Purchasing, manufacturing submission, flashing/powering hardware, paid services, and external publication require task authorization.

Finish with the result and editable artifacts, checks actually performed, material limits/blockers, and the next useful action. Record unavailable usage metrics as unavailable; never estimate token savings as measured usage. Store lessons as generic workflow improvements; retain product state in the project.
