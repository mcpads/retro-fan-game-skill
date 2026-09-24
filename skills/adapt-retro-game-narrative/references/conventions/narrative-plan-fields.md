# Narrative-plan Fields

The narrative plan owns what the authored playable work says. It refers to
source records and stays independent of where the host stores or displays each
unit.

## Authored Narrative Unit

Record:

- stable narrative-unit ID,
- intended route and creative purpose,
- preceding narrative state,
- event, meaning, or assertion introduced by the unit,
- resulting narrative state,
- predecessor, successor, branch, and convergence relationships,
- applicable source entries and canon constraints by reference,
- new claims introduced by the authored work,
- forbidden contradictions and intentionally changed meanings,
- required presentation or asset meanings by requirement ID,
- human approval references and unresolved questions.

An authored unit may be wholly new, with zero source entries.

## Derivation Relation

Record:

- stable derivation ID,
- zero or more source-entry IDs,
- zero or more authored narrative-unit IDs,
- descriptive relation defined in
  [Unit-level Relations](../strategy/narrative-derivation.md#unit-level-relations),
- meaning and state transitions that must be preserved,
- intentional differences and their rationale,
- affected branches and convergence conditions,
- required human decision references,
- unresolved source or authored-plan gaps.

Allow zero source entries for new or continuation units and zero authored units
for explicit omission. Many-to-many relations are required for merge, split,
and synthesis. Host data, build status, runtime results, and verdicts stay in
their owning records.
