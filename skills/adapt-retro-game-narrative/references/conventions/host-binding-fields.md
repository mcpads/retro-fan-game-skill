# Narrative Host-binding Fields

A host binding places authored narrative units in the play segments and
execution-host surfaces that carry them. Meaning belongs to the plan, and
implementation to the execution records.

## Binding Record

Record:

- stable binding ID,
- one or more authored narrative-unit IDs,
- one or more target host-surface or event IDs,
- play segment and route placement,
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
The binding holds references to those records, so each owner can change
independently.
