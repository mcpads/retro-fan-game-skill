# Workflow Gates

These gates decide when to experiment, expand production, or claim completion.
Evaluate the gate the next decision needs; each gate admits the investigation
that produces its evidence. Earlier passes hold while their inputs are current
under [Invalidation](../conventions/project-state.md#invalidation).

## Intent And Base Identity Gate

Passes when the intended route and its first segment, allowed changes,
completion target, authority boundary, and exact local inputs are known well
enough to constrain the next mutation. Identify one execution host and assign
roles to other originals under
[Input Scope](../conventions/execution-records.md#input-scope).

Before it passes, investigation and provisional samples proceed; an
unidentified base allows read-only analysis.

## Experimental Work

A small experiment may establish extraction, reconstruction, loader behavior, or
other unknown structure. Run it when:

- local input identity and the change's scope are established,
- the hypothesis and the observable that decides it are recorded,
- expected writes are bounded under
  [Execution Records](../conventions/execution-records.md),
- output and runtime state are isolated from originals, personal saves, and the
  selected playable, with a way back to the baseline,
- a stopping condition says when to inspect rather than expand.

Keep failures as evidence. Experimental results enter production after the proof
gates below pass, recorded under
[Project State](../conventions/project-state.md#research-experiments-and-adopted-work).

## Relevant-surface Proof Gate

Passes for a proposed use when extraction preserves the required data,
reconstruction is proven, mutable and protected parts are distinguished, budgets
and relocation rules are measured, and no open gap undermines that use. A rebuilt
container proves reconstruction; its changed runtime behavior needs the PoC.

## Creative-unit PoC Gate

A proof of concept shows one changed line, scene, asset, rule, cue, or branch
working inside its play segment. It passes when that unit:

- has surface proof and builds from the verified inputs with checks passing,
- is consumed through the real game path with evidence for the claim, and
- preserves adjacent content, control, state, timing, and save/load behavior.

For insertion, the PoC also covers the resource chain and adjacent behavior in
[Resource Insertion](resource-insertion.md). Keep measured constraints,
repeatable transforms, and evidence; experimental code may be discarded.

## Segment Playable Gate

A segment is playable when it is played through on the selected build from its
entry to its exit, including the transitions into and out of it and resumption
after saving, with its changed units observed and its placeholders listed. The
next segment builds on it.

## Overlay Expansion Gate

Production extends to further segments that use the surfaces and dependencies
of a passing PoC and a playable segment. Units
may be drafted ahead of their runtime pass; completion needs it. A component
claiming source conformance, asset coherence, reachability, or another
specialized property also needs a passing assessment from that domain for the
expansion. Reassess when expansion brings a different format, loader, or
dependency.

## Private Playable Gate

The work is complete for its intended personal route when:

- the execution host and required build sources are validated locally,
- the selected output contains every adopted change and is reproducible through
  the [Product Build Path](../conventions/execution-records.md#product-build-path),
- required creative content is approved at its review scope,
- specialized completion claims have current passing assessments,
- every changed surface on the route has game-visible evidence that applies to
  the selected build under
  [Claim Assessments](../conventions/claim-assessments.md#evidence-from-another-build),
- the route has been played continuously on the selected build from start to
  end, through segment transitions, required branches, and save/load resumption,
- every placeholder on the route is replaced or accepted by the person as final,
- critical runtime, story-state, save/load, route, and required-asset issues on
  the route are zero.

The continuous playthrough is the proof that segments join; separate segment
observations cover their segments.

## Shareable Candidate Gate

When sharing is in scope, passes when the private playable gate holds across the
shared scope, remaining limits are declared, and the checks in
[Asset Distribution Policy](asset-distribution-policy.md) and
[Package Manifest](../conventions/package-manifest.md) pass, including
clean-workspace reconstruction.
