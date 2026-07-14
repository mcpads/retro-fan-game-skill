---
name: assemble-retro-game-assets
description: >-
  Plan coherent semantic asset sets for retro fan games across multiple game
  surfaces. Use for character or NPC sprite sets, battle graphics and effects,
  map tiles and environment art, cutscene frames and portraits, item or status
  icons, interface assets, audio cues, cross-title reskins, newly authored cast
  or world presentation, and any asset change that needs many-to-many mapping,
  cross-surface continuity, coverage, or source-conformance assessment. Do not
  use for one isolated format conversion, image generation alone, binary
  insertion alone, map collision or reachability design, combat behavior, or
  emulator verification by themselves.
---

# Assemble Retro Game Assets

## Overview

Define what an asset means, which authored set it belongs to, and which proven
host surfaces must express it. Keep semantic assembly separate from image or
audio generation, binary conversion, insertion, runtime observation, and
distribution.

Use this skill only when asset relationships or coverage span more than one
opaque replacement. A single icon or portrait can remain in the fan-game
orchestrator's ordinary asset path.

## Operating Model

For each asset component:

- identify the represented entity, place, item, state, cue, or interface role,
- declare whether the material is retained, adapted, remixed, substituted, or
  newly authored,
- group variants and cross-surface representations that must remain coherent,
- map semantic asset units to stable host surfaces independently of physical
  binding strategy,
- refer to structure, provenance, transform, observation, and approval owners,
  and
- predeclare the coverage, coherence, or source-conformance claim that matters.

Treat asset profiles as open, platform-specific labels. Do not make one fixed
taxonomy a prerequisite for every game.

## Dependency Boundaries

- Own semantic identity, intended role, source relationship, many-to-many
  mapping, cross-surface continuity, and assessment criteria.
- Leave palette, tile, frame, timing, compression, memory, and container limits
  to the host structure owner.
- Leave generation prompts and authored provenance to the asset-provenance
  owner; leave replacement or insertion mechanics to execution and resource
  owners.
- Leave collision, warp, quest reachability, combat hitboxes, AI, damage, and
  timing behavior to world, system, or host-structure capabilities.
- Keep runtime consumption evidence separate from visual, tonal, or semantic
  approval.
- Reuse an existing project asset catalog or mapping when it owns equivalent
  meanings.

## Reference Routing

| Current judgment | Read |
| --- | --- |
| Bound asset scope, profiles, semantic relations, and ownership | `references/strategy/asset-assembly.md` |
| Inventory semantic asset units and their variants or source roles | `references/conventions/asset-ledger-fields.md` |
| Map authored asset meanings to one or more host surfaces | `references/conventions/asset-map-fields.md` |
| Predeclare asset readiness, coverage, coherence, or conformance claims | `references/conventions/asset-assessment-profiles.md` |

## Core Invariants

- Never use a physical file, sheet index, or byte offset as the only semantic
  identity of a character, place, item, state, or cue.
- Never infer game-format compatibility from visual plausibility.
- Never treat the execution host's existing art as semantic authority for an
  adapted source.
- Never copy format budgets, writes, loader paths, runtime results, or package
  policy into the asset ledger or map. Refer to their owners.
- Never equate a displayed asset with an approved or coherent asset.
- Never let an asset requirement silently redefine narrative state, map
  topology, combat behavior, or interface action.

## Expected Outputs

Produce the smallest durable asset-semantics artifact that advances the current
decision: an asset unit, variant group, source relation, semantic mapping,
coverage gap, readiness assessment, coherence assessment, or explicit domain
dependency. Export stable IDs, outcomes, scope, and limits to the fan-game
orchestrator without taking ownership of build or observation records.
