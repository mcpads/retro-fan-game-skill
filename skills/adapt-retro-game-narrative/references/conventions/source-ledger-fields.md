# Source-ledger Fields

Reuse an existing source-narrative owner when it already records these
meanings. Stable source IDs must not depend on a physical offset or on the
target host.

## Source And Edition Registry

For each relevant source or edition, record:

- stable source-work and edition IDs,
- title, platform or medium, revision, and other identity discriminators,
- scoped role defined in
  `references/strategy/narrative-derivation.md#scoped-source-roles`,
- claims or units inside and outside that authority scope,
- relationship to other editions or sources,
- precedence or human conflict-decision reference when scopes overlap,
- evidence provenance and unresolved identity questions.

Calling a source the execution host does not grant narrative authority.

## Scene Or Canon-constraint Entry

Record:

- stable source-entry ID and source or edition ID,
- entry kind, such as scene, state transition, rule, or canon constraint,
- preceding narrative state,
- event, assertion, or constraint,
- resulting narrative state when applicable,
- ordering and causal evidence,
- certainty: `confirmed`, `strong_inference`, `weak_inference`, or `unknown`,
- one or more source locators,
- semantic invariants that a declared preservation relation must retain,
- conflicts, omissions, alternate readings, and unresolved questions.

## Source Locator

A locator records its kind, source identity, stable logical entry when
available, and a physical coordinate only when the medium provides one. A
locator may be a script entry, file and section, database row, timestamp,
address, or byte offset. Byte offsets are optional evidence coordinates, never
the stable source-entry identity.

Do not copy engine flags, host event IDs, build status, or runtime verdicts into
the source ledger. Those belong to host, execution, or observation owners.
