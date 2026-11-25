# Toolchain setup and verification

## Discover and install only the needed routes

Inspect the project and existing tools before asking questions. For heavy work, inspect OS, CPU/RAM, free disk and GPU; check only relevant applications, runtimes, current MCP configuration and occupied bridge ports. Mechanical: FreeCAD, CalculiX and Gmsh. Electronics: KiCad. Visualization: Blender. Reporting: LaTeX only for a requested LaTeX deliverable. Use Python/Git where needed. No CFD prerequisites.

Reuse working versions. Prefer free, inspected, pinned dependencies in an isolated local environment. Respect host permissions and existing installation authorization; obtain required permission for additional administrator/system changes, replacement of working software, paid services, or security/network changes. Never bypass security prompts or broaden permissions to fix an installation. Do not run a downloaded installer or dependency script before inspecting its purpose and provenance. Keep secrets out of chat, logs and version control; never request an AI API key to run a local solver.

Use one suitable application connector per route and share it between real workers when supported. Verify current upstream compatibility and license; record repository/version/commit and local modifications. Prefer established tested MCP integrations over writing adapters. Direct CLI automation is a legitimate fallback, explicitly labelled. Do not install an orchestrator or create a custom MCP merely to claim MCP coverage. Bind bridges to loopback, avoid unauthenticated remote exposure, and leave optional paid/asset services off unless needed and authorized.

Configure the actual host: Codex uses its supported MCP settings; Claude and other clients use their own supported configuration. Use project scope when supported, otherwise the narrowest appropriate existing scope. Preserve unrelated settings and back up before modifying them. Verify tool access for every actual worker, not just the coordinator. If reload/restart is needed, save resume state; do not claim tools are active or launch another manager as a workaround.

## Real smoke tests

Run only routes required for current work or explicitly requested setup. Test in scratch files, never an unsaved user document. Capture versions, exact calls/commands, output paths and inspection evidence.

| Route | Minimum meaningful verification |
| --- | --- |
| CAD | Create, edit, save/reopen and export a known solid; inspect validity, dimensions and export. |
| Structural solver | Solve a textbook case with a known analytical answer, such as a cantilever tip load. Compare displacement and reaction balance with justified tolerances; inspect result files. Test before relying on FEM conclusions. |
| Electronics | Create a small schematic and board, save/reopen, run ERC/DRC and inspect reports. Resolve or document findings; tool availability alone is not a design pass. |
| Blender | Import known-size geometry, verify units/dimensions, save/reopen, render and inspect an image. |
| LaTeX | Compile and inspect one page when this format is needed. |
| MCP | Complete initialization, list available tools, then execute a meaningful relevant call and inspect its output. A config entry or handshake alone does not prove application operations. |

State separately: installed, configured, connected, verified. Use PASS/PARTIAL/FAIL/BLOCKED/NOT RUN against the specific tested scope. Never call the entire workflow operational if a required route is unverified. Route failures should not block unrelated concept or documentation work.

If user intervention remains necessary, give one consolidated list: application, exact action, and success check. Retry based on diagnostics; after three failures with no new information change approach or save the concrete blocker.
