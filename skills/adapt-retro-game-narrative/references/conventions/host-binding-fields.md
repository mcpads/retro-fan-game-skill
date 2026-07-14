# Narrative Host-binding Fields

A host binding connects the authored narrative plan to stable execution-host
surfaces. It does not decide source meaning and does not own the implementation
of those surfaces.

## Binding Record

Record:

- stable binding ID,
- one or more authored narrative-unit IDs,
- one or more target host-surface or event IDs,
- intended route placement,
- required entry state, flags, branches, and convergence conditions,
- required exit state and downstream narrative dependencies,
- structure-map and relevant surface-proof references,
- presentation, cast, asset, audio, or rule requirement IDs,
- approval, execution, observation, and assessment references,
- unresolved host gaps and the claims they block.

Many authored units may share one host event, and one authored unit may span
multiple host events. Record the relation rather than forcing one-to-one rows.

## Ownership Boundary

The narrative plan may require that a character appear injured or that a reveal
precede a confrontation. The asset owner chooses which portrait or sprite
expresses the state. The host structure owner records format and engine
constraints. Execution owns writes, and observation owns raw runtime evidence.

Do not copy byte coordinates, conversion settings, asset provenance, execution
status, or raw observations into the binding. Use stable references so each
owner can change independently.
