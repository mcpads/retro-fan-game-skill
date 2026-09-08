# Project State

This convention owns current selection, resumption, adoption, and invalidation.
Use an existing status page, manifest, issue, or equivalent as one stable entry
for ongoing work. A small task may use a section in its existing record; no
particular filename or new tracking system is required.

## Current Entry

Keep only the information needed to resume:

- intended playable route and completion target, with decision references,
- selected structure, creative plan, content, and transform revisions,
- selected build receipt and output identity, if a build has been selected,
- applicable assessment references and unresolved blockers,
- work in progress, the next action, and the question it will resolve,
- last verified time and references to the records checked.

The entry selects records; it does not copy their evidence or own their verdicts.
Use stable semantic IDs for units, and pin revisions or content hashes wherever
an execution or assessment depends on their contents. A stable ID alone must
not make evidence silently apply to changed content. Use existing revision
mechanisms; Git can identify tracked inputs without a separate release number.

Update the same entry when selection, dependencies, or the next action changes.
Keep historical events in execution records or the project's journal. Do not
accumulate dated current-state files or make a handoff the sole source of state.

## Resume From Evidence

Read the current entry and its referenced owners before searching old logs.
Check that the selected inputs and outputs still match their recorded identities
and that the assessments apply to those contents and the intended route. Inspect
unfinished work before launching a duplicate run or overwriting its outputs.

If the entry is missing or stale, reconstruct it from explicit decisions,
receipts, and evidence. Do not select an artifact because it is newest, has a
promising filename, or appears in a successful historical run. Preserve any
uncertainty that affects selection and perform the smallest check to resolve it.
Resume the next unresolved decision; do not repeat valid work merely to rebuild
the conversation's memory.

## Research, Experiments, And Adopted Work

Keep each kind of material distinguishable within the existing project layout:

| Role | Use |
| --- | --- |
| Research and hypotheses | Explain possible structures and source meanings; not authoritative build rules |
| Experimental code and outputs | Test a bounded question; not selected product inputs by default |
| Adopted facts, content, and transforms | Explicit inputs to the reproducible product build, with supporting evidence |
| Raw evidence and historical runs | Preserve what happened for exact inputs, even when an interpretation is later rejected |

Adoption records what was selected, its exact contents, supporting assessment,
scope, remaining limits, and what it replaces. It is a technical evidence
decision unless it crosses the creative boundary in
[Intent And Authority](../strategy/intent-and-authority.md).
Reusable parts of an experiment may be adopted in place; no directory copying
or duplicate implementation is required.

The product build consumes an explicit selection of adopted inputs and required
deterministic transforms. It must not discover product inputs by scanning old
experiments, rerun exploratory analysis or creative generation on each build,
or depend on a transient cache. Preserve adopted analysis or generation results
and their provenance so discovery need not be repeated to reproduce the game.

## Invalidation

When evidence or intent changes, identify the affected revisions, conclusions,
builds, and completion claims through their dependencies. Mark their applicability
invalid before allowing further promotion; preserve unrelated proof.

Retain raw observations and historical outcomes. Correct or supersede the owning
fact or assessment, record why and what replaces it when known, and update the
current entry and dependent state projections together. A historical pass remains
evidence about its original scope, not a current pass for changed dependencies.
Unresolved conflicting evidence keeps the affected claim open; do not select a
convenient older pass to hide it.

For example, a corrected compression rule invalidates builds that used the old
compressor and claims depending on its validity. Their captures remain useful
evidence of those runs. An unrelated approved scene need not be reapproved.

Use existing machine-readable checks where possible to reject dangling selected
references, content-identity mismatches, and completion projections based on
invalidated assessments. Keep creative sufficiency with its human or domain
owner; a valid reference graph alone does not prove a playable.
