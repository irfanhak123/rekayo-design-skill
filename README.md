# Rekayo Design Skill

An agent skill for adaptive physical product engineering—covering concept exploration, evidence-based comparison, detailed mechanical/electrical engineering, assembly visualization, and controlled revisions (no CFD).

## Overview

**Rekayo Design Skill** guides coding and engineering agents to deliver physical product outcomes with the smallest useful workflow, scaling CAD/FEM, electronics, visualization, tools, and specialist delegation only when needed.

### Supported Modes
- **Explore**: Generate meaningfully different architectures or principles at low fidelity before committing.
- **Compare**: Evaluate candidates against identical requirements, interfaces, load cases, and evidence standards.
- **Detail**: Develop the selected concept with editable native artifacts, calculations, interfaces, and verification checks.
- **Change**: Preserve baselines, assess affected interfaces and requirements, revise, and re-verify.

### Key Disciplines
- **Mechanical & FEM**: Editable parametric CAD (e.g., FreeCAD), hand calculations, mesh convergence, and sensitivity checks.
- **Electronics**: Real schematics/PCBs (e.g., KiCad), component evidence, electrical margins, and ERC/DRC checks.
- **Assembly & Visualization**: Blender-based product views, exploded views, clearance/access checks, and manuals from released geometry.
- **Evidence & Release Discipline**: Traceable quantities (`SOURCE`, `CALCULATION`, `SIMULATION`, `MEASUREMENT`, `ASSUMPTION`), explicit `PASS / PARTIAL / FAIL / BLOCKED / NOT RUN` statuses, SHA-256 release manifests, and controlled change records.

## Repository Structure

```text
rekayo-design-skill/
├── SKILL.md                  # Core skill instructions and workflow
├── agents/
│   └── openai.yaml           # Agent interface metadata
└── references/
    ├── assembly.md           # Assembly and visualization procedures
    ├── electronics.md        # Electronics, schematic, and PCB guidelines
    ├── mechanical.md         # Mechanical CAD and structural FEM guidelines
    ├── release.md            # Evidence records, baselines, and change control
    └── toolchain.md          # Toolchain discovery, setup, and smoke tests
```

## Installation

Clone this repository into your project's or global agent skills directory:

**Project-level (`.agents/skills`)**
```bash
git clone https://github.com/irfanhak123/rekayo-design-skill.git .agents/skills/rekayo-design-skill
```

**Global skills directory**
- **Gemini / Antigravity**: `~/.gemini/config/skills/rekayo-design-skill`
- **Codex**: `~/.codex/skills/rekayo-design-skill`
- **Claude**: `~/.claude/skills/rekayo-design-skill`

```bash
git clone https://github.com/irfanhak123/rekayo-design-skill.git ~/.gemini/config/skills/rekayo-design-skill
```
