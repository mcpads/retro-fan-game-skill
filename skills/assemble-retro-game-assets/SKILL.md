---
name: assemble-retro-game-assets
description: >-
  Coordinate coherent retro-game asset sets across sprites, battle graphics,
  maps, portraits, cutscenes, interface elements, and audio. Use for multi-surface
  identity, variants, many-to-many mappings, coverage, or source conformance,
  including reskins and newly authored sets. Excludes isolated conversion or
  generation, binary insertion, map reachability, combat behavior, and emulator
  verification alone.
---

# Assemble Retro Game Assets

Define what an asset means and which game surfaces must express it. Keep semantic
assembly distinct from generation, conversion, physical insertion, and runtime
observation. A single icon or portrait with no wider relationship can remain in
an ordinary asset-editing workflow.

## Start Or Resume

Recover the intended experience, selected asset set, required representations,
and existing creative decisions. Use the project's current-state and approval
owners when composed with other capabilities. When used alone, keep a stable
entry to the selected catalog and mapping revisions, assessment, unresolved
choices, and next action in the existing asset record.

Carry explicit requests and prior approvals forward without asking again. Use a
small comparison of related representations to clarify unresolved identity or
aesthetic choices. The person judges their meaning and acceptable differences;
the agent investigates technical fit. Direction approval does not approve every
subsequently generated asset.

## Work At The Needed Scope

- Group represented entities, places, items, states, cues, and their required
  variants across the intended route. Profiles are open labels, not a fixed enum.
- Keep semantic relations independent of physical host bindings. One character
  may require field, portrait, and battle representations; one source sheet may
  split across several host surfaces.
- Reuse existing catalogs and maps. Semantic units, bindings, and assessments may
  be separately addressable sections of one artifact.
- Refer to host-owned format budgets, provenance-owned generation records, and
  execution-owned transforms instead of copying them into the semantic catalog.
- Keep collision, reachability, combat behavior, and interface actions with
  their domain owners. An asset change cannot silently redefine them.

## Reference Routing

| Current decision | Owner |
| --- | --- |
| Bound asset scope, semantic relations, and a reviewable sample | [Asset Assembly](references/strategy/asset-assembly.md) |
| Inventory semantic units, variants, and source roles | [Asset-ledger Fields](references/conventions/asset-ledger-fields.md) |
| Map meanings to one or more host surfaces | [Asset-map Fields](references/conventions/asset-map-fields.md) |
| Assess readiness, coverage, coherence, and source conformance | [Asset Assessment Profiles](references/conventions/asset-assessment-profiles.md) |

## Return The Useful Result

Produce the smallest sample, unit, mapping, coverage gap, or assessment that
advances the asset decision. Reference exact source and mapping revisions in
assessments. Keep semantic identity stable across file renames and conversions,
while invalidating affected assessments when the represented content changes.
Return those dependencies to the current-state owner; runtime visibility alone
cannot establish aesthetic approval or cross-surface coherence.
