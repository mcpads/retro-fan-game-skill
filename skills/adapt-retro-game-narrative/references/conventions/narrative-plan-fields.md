# Narrative-plan Fields

The narrative plan owns what the authored playable work says. It refers to
source records but does not redefine them, and it remains independent of where
the execution host stores or displays the unit.

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

An authored unit may be wholly new. Do not fabricate a source entry merely to
give it provenance.

## Derivation Relation

Record:

- stable derivation ID,
- zero or more source-entry IDs,
- zero or more authored narrative-unit IDs,
- descriptive relation defined in
  `references/strategy/narrative-derivation.md#unit-level-relations`,
- meaning and state transitions that must be preserved,
- intentional differences and their rationale,
- affected branches and convergence conditions,
- required human decision references,
- unresolved source or authored-plan gaps.

Allow zero source entries for new or continuation units and zero authored units
for explicit omission. Many-to-many relations are required for merge, split,
and synthesis.

Do not include host bytes, target asset hashes, build status, runtime results,
or a final conformance verdict. Point to their owning records.
