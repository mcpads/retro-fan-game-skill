# Workflow Gates

These gates are dependency conditions, not a mandatory linear schedule. Evaluate
the gate relevant to the current claim and work on independent branches when
their dependencies are satisfied. Define evidence before selecting products;
leave a gate open when no available capability can prove it.

## Contents

- [Intent And Base Identity Gate](#intent-and-base-identity-gate)
- [Relevant-surface Proof Gate](#relevant-surface-proof-gate)
- [Creative-unit PoC Gate](#creative-unit-poc-gate)
- [Overlay Expansion Gate](#overlay-expansion-gate)
- [Private Playable Gate](#private-playable-gate)
- [Shareable Candidate Gate](#shareable-candidate-gate)

## Intent And Base Identity Gate

Pass when the intended personal route, changed surfaces, completion target,
human approval boundary, exact local input identity, and provenance of inherited
facts are known well enough to constrain the next action.

When more than one original game participates, identify one execution host and
classify every additional original as a required build source or evidence-only
source. Do not merge their structure or semantic authority.

Failure permits planning and provisional creative exploration, but not applying
or evaluating build mutations against an unidentified base.

## Relevant-surface Proof Gate

Pass for a surface when extraction or parsing preserves required data,
reconstruction is proven, mutable and protected parts are distinguished,
relevant budgets and relocation behavior are measured, and gaps that could
invalidate the proposed mutation are explicit.

Use `references/conventions/structure-map-fields.md` for the concrete record.
Failure keeps build-bound content for that surface provisional.

## Creative-unit PoC Gate

Pass when one minimal changed line, scene, asset, rule, cue, or route branch:

- builds from the verified original input under the execution contract,
- is consumed through the real game path,
- has sufficient raw observation for the declared runtime claim, and
- preserves the relevant adjacent content, control, state, timing, and save/load
  behavior.

Prototype code may be discarded. Promote only measured constraints, repeatable
transforms, and evidence records.

## Overlay Expansion Gate

Pass a unit into broader production only after its surface PoC succeeds and the
unit advances through the explicit artifact states in
`references/conventions/artifact-states.md`. A plausible draft is not a valid
build, and a valid build is not automatically a runtime-observed unit.

If the unit claims a specialized property such as source-narrative conformance,
cross-surface asset coherence, behavior equivalence, world reachability, or
procedural solvability, its applicable capability handoff must contain a
passing readiness assessment for that scope. This is conditional; units that
make no such claim do not inherit irrelevant gates.

## Private Playable Gate

A private playable is complete for its intended personal route only when:

- the exact execution-host input and every required build-source input are
  validated locally,
- the local output is reproducible from preserved execution inputs and receipts,
- required human decisions are approved within their recorded scope,
- every applicable specialized completion claim has a scoped passing
  assessment,
- every changed surface on that route has sufficient game-visible evidence, and
- known critical runtime, story-state, save/load, route, and required-asset
  issues are zero for that route.

Distribution checks are not part of this gate. The personal work may stop here
without being incomplete.

## Shareable Candidate Gate

Evaluate this gate only when sharing is in scope. A package is a candidate when:

- the private-playable gate passes across the declared shareable scope,
- original input requirements and hashes are enforced,
- modified routes and surfaces have sufficient evidence for that scope,
- known critical issues are zero and remaining limits are declared,
- every included artifact satisfies the classifications and negative boundary
  owned by `references/strategy/asset-distribution-policy.md`, and
- manifest, exclusion, and clean-workspace checks in
  `references/conventions/package-manifest.md` pass.

This gate composes those owners; it does not redefine their fields or policy.
