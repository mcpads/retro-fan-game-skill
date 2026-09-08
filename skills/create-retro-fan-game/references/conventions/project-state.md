# Project State

Keep one stable entry for current work in an existing status page, manifest,
issue, or record section. It identifies selected results and how to resume;
no particular filename or new tracking system is required.

## Current Entry

Keep only the information needed to resume:

- intended playable route and completion target, with decision references,
- selected structure, creative plan, content, and transform revisions,
- selected build receipt and output identity, if a build has been selected,
- applicable assessment references and unresolved blockers,
- work in progress, the next action, and the question it will resolve,
- last verified time and references to the records checked.

Reference records without copying their evidence or assigning new verdicts.
Keep unit IDs stable, but pin revisions or hashes for content-dependent execution
and assessments. A stable ID alone cannot identify changed content. Use existing
revision mechanisms, such as Git, without inventing release numbers.

Update the same entry when selection, dependencies, or the next action changes.
Keep history in run records or the journal, not dated copies of current state.
A temporary handoff must not be the sole source of current state.

## Resume From Evidence

Read the entry and its referenced records before old logs. Verify selected input
and output identities and the assessments' applicability to those contents and
the intended route. Inspect unfinished work before duplicating a run or
overwriting its outputs.

Reconstruct a missing or stale entry from explicit decisions, receipts, and
evidence. Recency, filenames, and historical success do not establish current
selection. Record uncertainty, perform the smallest check that resolves it, and
resume the next decision without repeating valid work to rebuild chat memory.

## Research, Experiments, And Adopted Work

Keep each kind of material distinguishable within the existing project layout:

| Role | Use |
| --- | --- |
| Research and hypotheses | Explain possible structures and source meanings; not authoritative build rules |
| Experimental code and outputs | Test a bounded question; not selected product inputs by default |
| Adopted facts, content, and transforms | Explicit inputs to the reproducible product build, with supporting evidence |
| Raw evidence and historical runs | Preserve what happened for exact inputs, even when an interpretation is later rejected |

Adoption means selecting a result for product use. Record its exact contents,
supporting assessment, scope, limits, and what it replaces. The agent decides
technical adoption unless it crosses the creative boundary in
[Intent And Authority](../strategy/intent-and-authority.md).
Reuse experimental code in place when suitable; adoption requires no copy.

Selecting a finding does not select its discovery procedure. Adopt a procedure
for recurring product use only when it supplies a required deterministic transform
or mechanical check, with declared inputs, outputs, and failure behavior under the
[Product Build Path](execution-records.md#product-build-path).
Preserve adopted analysis or generation results and provenance. Do not scan old
experiments for inputs, rerun exploratory analysis or creative generation on each
build, or depend on a transient cache.

## Invalidation

When evidence or intent changes, follow dependencies to affected facts, product builds,
and assessments. Mark conclusions that no longer apply as invalid before further
adoption or completion decisions; preserve unrelated proof.
Applying runtime evidence to a different build requires the scoped comparison in
[Claim Assessments](claim-assessments.md#evidence-from-another-build).

Retain raw observations and historical outcomes. Correct or supersede the fact or
assessment, record the reason and any replacement, then update the current entry
and affected statuses together. A historical pass covers its original scope.
Unresolved conflicting evidence keeps a claim open; do not hide it with an older
pass.

For example, a corrected compression rule invalidates builds that used the old
compressor and claims depending on its validity. Their captures remain useful
evidence of those runs. An unrelated approved scene need not be reapproved.

Use existing automated checks to reject missing references, identity mismatches,
and completion statuses based on invalidated assessments where possible. Valid
references alone do not establish creative quality or playability.
