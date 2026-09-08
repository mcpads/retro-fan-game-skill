# Execution Records

Execution records preserve declared inputs, writes, checks, and outputs. Their
evidence boundary is owned by
[Capability Composition](../strategy/composition.md#responsibilities).
Classify each operation under [Work Roles](work-roles.md).
Use [Project State](project-state.md) for selecting adopted product inputs;
experimental runs remain distinguishable from the selected playable.

## Expected Write

Before applying a binary or container mutation, record:

- one owning change or overlay unit,
- source identity and source coordinate or logical object,
- allowed range, object, or container boundary,
- expected source bytes or an equivalent source condition,
- final bytes or deterministic derivation,
- relevant alignment, relocation, checksum, compression, or media update,
- explicit composition rule when another owner may touch the same destination,
- verification that should fail if the write is skipped or misapplied.

Fail closed when a source condition mismatches, owners overlap without a rule, a
write enters a protected boundary, a dependency is missing, or a final
difference has no owner. Do not silently carry unknown entries, failed
conversions, or missing assets into the output.

## Input Scope

Record what each task actually consumes. Investigation may parse or extract an
`evidence_only` original; a conversion may consume only authored assets. Neither
requires the execution host as an input unless the task uses it.

Original-source roles describe product dependencies. An additional original is a
`build_source` when adopted game material must be reconstructed from it. Verify
its identity and keep that reconstruction in the product build; a cached extract
does not remove the dependency. Reading an original to establish facts or guide
newly authored work does not by itself make it a build source.

## Product Build Path

Keep one documented primary path from selected inputs to the cumulative ROM,
disc image, or other game output. Combine all adopted content, assets, code, and
container changes for the declared scope; separate component proofs do not
establish that integrated result. Isolated experiments may use provisional paths
under [Workflow Gates](../strategy/workflow-gates.md#experimental-work).

Document the invocation and dependency order using the transform records below.
Reuse an equivalent existing path; it may contain several tools or languages.
Select inputs and procedures under
[Project State](project-state.md#research-experiments-and-adopted-work).
Every stage that changes the final output, including postprocessing, participates
in [Expected Write](#expected-write). No untracked manual fixup or alternate writer
may modify the selected output after verification.

Derive current layout and values from declared inputs. Enforce mechanically
decidable constraints against independently established rules, and verify the
resulting artifact, including reparsing rebuilt structures where relevant.
Reject invalid current inputs or output even when the tooling build and tests
pass. Retained failed or partial outputs are diagnostic artifacts, not selectable
successful builds; they must not replace the selected playable.

Record the cumulative output's identity and checks in its execution receipt.
Attribute runtime evidence to that output under
[Runtime Observation](../strategy/runtime-observation.md). Optional distribution
patches must reproduce the same target when applied to their declared originals.

## Transform Record

For each deterministic transform, preserve:

- transform identity and exact source revision or content hash, including local
  changes that affect execution,
- verified identities and hashes of consumed inputs, their task purpose, and
  original-source roles when applicable,
- configuration and any structure-map identity the transform consumes,
- toolchain and external-component identities and options that affect output,
- declared outputs and expected identity policy,
- checks that run before, during, and after the transform,
- failure result and whether partial outputs are discarded.

## Execution Receipt

Each completed run records:

- run identity,
- run purpose and experiment question or adopted-input selection reference,
- exact input and transform identities,
- structure-map and overlay identities when the run consumes them,
- expected-write set when the run applies mutations,
- checks executed and their pass, fail, or skipped status,
- output paths or logical IDs and hashes,
- explained and unexplained final differences when outputs are compared against
  a baseline,
- warnings, failures, and known non-deterministic inputs.

A successful receipt requires no skipped required check and, when final-diff
ownership applies, zero unexplained final differences. Runtime evidence for a
built output references the receipt identity so the observed game cannot be
confused with another build.

An experimental run may fail its hypothesis while still producing useful
evidence. Record actual check failures; do not relabel them as passes to retain
the result. Choose tests and current-artifact checks under
[Work Roles](work-roles.md#tests-and-current-artifact-checks).
