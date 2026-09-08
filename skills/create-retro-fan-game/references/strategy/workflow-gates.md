# Workflow Gates

These gates define when to run experiments, expand production, or claim completion.
Evaluate only the relevant gate. A gate must allow the investigation needed to
establish its evidence. Here, production means preparing content and transforms
for the game build; provisional samples remain exploratory. Check that earlier
passes still apply under
[Project State](../conventions/project-state.md#invalidation).

## Contents

- [Intent And Base Identity Gate](#intent-and-base-identity-gate)
- [Experimental Work](#experimental-work)
- [Relevant-surface Proof Gate](#relevant-surface-proof-gate)
- [Creative-unit PoC Gate](#creative-unit-poc-gate)
- [Overlay Expansion Gate](#overlay-expansion-gate)
- [Private Playable Gate](#private-playable-gate)
- [Shareable Candidate Gate](#shareable-candidate-gate)

## Intent And Base Identity Gate

Pass when the intended route, allowed changes, completion target, authority
boundary, and exact local inputs are known well enough to constrain the next
mutation. Interpret existing authorization using
[Intent And Authority](intent-and-authority.md).

Identify one execution host and classify additional originals as required build
sources or evidence-only sources. Preserve inherited claims' provenance; a source
role does not grant host-structure or narrative authority.

Unresolved intent permits relevant investigation and provisional samples.
An unidentified base permits read-only analysis, but no binary mutation.

## Experimental Work

A small experiment may establish extraction, reconstruction, loader behavior,
or other unknown structure. Run it when:

- local input identity and the proposed change's scope are established,
- the hypothesis, unknowns under test, and distinguishing observable are recorded,
- expected writes and source conditions are bounded under
  [Execution Records](../conventions/execution-records.md),
- output and runtime state are isolated from originals, personal saves, and the
  selected playable, with a way to discard the result or restore the baseline,
- a stopping condition identifies when to inspect the result rather than expand.

Run applicable checks and retain failures as evidence. Inspect unknown write
boundaries before mutation, but do not require the test's conclusion in advance.
Use experimental results in production only after the applicable proof gates pass.
Record adoption under
[Project State](../conventions/project-state.md#research-experiments-and-adopted-work).

## Relevant-surface Proof Gate

Pass for the proposed scope when extraction or parsing preserves required data,
reconstruction is proven, mutable and protected parts are distinguished, relevant
budgets and relocation rules are measured, and no unresolved gap invalidates the
proposed production use. Record the evidence in
[Structure-map Fields](../conventions/structure-map-fields.md).

Failure keeps that production use provisional while allowing bounded experiments.
Proof of a rebuilt container alone does not prove its changed runtime behavior.

## Creative-unit PoC Gate

PoC means proof of concept: one changed unit demonstrates the intended behavior.
Pass when one minimal changed line, scene, asset, rule, cue, or route branch:

- has relevant surface proof and builds from the verified inputs with the
  applicable execution checks passing,
- is consumed through the real game path with sufficient raw evidence for the
  declared claim, and
- preserves relevant adjacent content, control, state, timing, and save/load
  behavior.

For insertion, the PoC must establish the affected resource chain and adjacent
resource behavior specified in [Resource Insertion](resource-insertion.md).
Preserve measured constraints, repeatable transforms, and evidence; experimental
code need not survive adoption.

## Overlay Expansion Gate

Allow broader production only for the proven surface and dependencies
of a passing PoC. Track units using the applicable axes in
[Creative Artifact States](../conventions/artifact-states.md). Drafting does not
require each unit's runtime pass in advance; completion does.

A component claiming source conformance, asset coherence, behavior equivalence,
reachability, or another specialized property also needs a scoped passing
readiness assessment from the applicable domain capability. Components making no
such claim inherit no extra domain gate. Reassess when expansion introduces a
different format, loader path, or unproven dependency.

## Private Playable Gate

Complete the work for its intended personal route only when:

- exact execution-host and required build-source inputs are validated locally,
- the selected output is reproducible from the adopted inputs and transforms,
- required creative decisions and content are approved within their review scope,
- applicable specialized completion claims have scoped passing assessments,
- every changed surface on that route has sufficient game-visible evidence tied
  to the selected build, and
- known critical runtime, story-state, save/load, route, and required-asset issues
  are zero for that route.

An invalidated or mismatched assessment cannot support completion. Unobserved
changed routes remain open. Distribution checks are not part of personal
completion; the person may stop here with a complete work.

## Shareable Candidate Gate

Evaluate only when sharing is in scope. Pass when the private-playable gate holds
across the declared shareable scope, remaining limits are declared, and both
[Asset Distribution Policy](asset-distribution-policy.md) and
[Package Manifest](../conventions/package-manifest.md) checks pass, including input
identity enforcement and clean-workspace reconstruction.
