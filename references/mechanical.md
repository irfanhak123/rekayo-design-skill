# Mechanical design and structural analysis

Use FreeCAD when suitable, or the project's established CAD tool. Retain purchased parts as sourced envelopes/interfaces rather than redesigning their internals. Keep dimensions, material properties, and loads sourced or explicitly assumed.

Build editable parametric native files. Check solid validity, interference, tolerances/fit, packaging, seal/fastener strategy where relevant, assembly sequence, maintenance, and tool access. Save, reopen, and inspect an exchange export against the native model. Check part IDs, units, coordinate systems, and revision at handoffs. Windows/WSL share one authoritative editable source; any transfer has explicit revision and SHA-256 checks.

Before expensive FEM, establish requirement IDs, load cases and verification methods: mass, stiffness/deformation, strength, interfaces and access as applicable. Derive loads from documented use assumptions and actual lever arms. Start with hand calculations. Do not invent acceptance thresholds, material strengths, or safety factors.

When structural comparison is justified, evaluate distinct geometries using identical material, interfaces, restraints, contacts, loads, and reporting conventions. Start with three variants for a substantial optimization unless the brief specifies another scope; a minor edit need not trigger three designs. Compare mass, stress, displacement, reaction balance, manufacturing effort, and requirement margins. Treat stress singularities explicitly rather than choosing a convenient peak.

For decision-bearing FEM, justify elements, mesh quality, contact and restraints. Use at least three mesh levels for the chosen candidate and report convergence of relevant quantities with a declared tolerance; refine further if unresolved. Test load-introduction and support assumptions. Include neighbouring structure at least once where its flexibility/load transfer could change the conclusion. If this is outside the requested effort, leave that claim PARTIAL rather than implying validation. Static results do not validate drop, impact, fatigue, creep, or physical safety.

When another discipline's interface changes, identify its stale artifacts and rerun affected checks. Compare candidates from saved result files, not recollection or screenshots alone.
