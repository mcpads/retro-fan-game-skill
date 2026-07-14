---
name: adapt-retro-game-narrative
description: >-
  Normalize and plan source-aware narrative composition for a retro playable
  work when an existing story or canon constrains more than a local line. Use
  for moving one game's story onto another game's execution host, retellings,
  divergences or alternate timelines, continuations and side stories,
  evidence-backed restoration, multi-source synthesis, or original scenarios
  bounded by declared canon. Establish scoped source authority, scene or canon
  ledgers, authored narrative units, host bindings, and mode-aware readiness or
  conformance assessments. Do not use for unconstrained original writing,
  translation-only work, isolated dialogue edits, cosmetic asset swaps, rule
  or UI mods, or build and emulator verification by themselves.
---

# Adapt Retro Game Narrative

## Overview

Turn relevant source evidence into a traceable narrative plan without making
the source, target host, or runtime observer interchangeable authorities. Use
the smallest source scope that constrains the intended playable route.

This skill owns narrative normalization and derivation contracts. It does not
own source extraction, asset semantics, binary mutation, runtime observation,
or the person's high-impact creative decisions.

## Operating Model

For each narrative unit, determine independently:

- which source or canon claims constrain it and within what scope,
- whether it preserves, transforms, branches from, continues, synthesizes, or
  merely draws constraints from those claims,
- what the authored work actually asserts before and after the unit,
- where the authored unit binds to the execution host, and
- which readiness or conformance claim must pass for the next decision.

Do not force one narrative mode on the whole project. A faithful route, a new
side scene, and a divergent ending may coexist when their unit-level relations
and approval boundaries are explicit.

## Dependency Boundaries

- Treat narrative authority, comparison evidence, inspiration, and execution
  host as scoped roles. A host does not gain narrative authority by providing
  the runtime.
- Normalize only source scenes and canon constraints needed by the declared
  route. Do not turn the skill into an encyclopedia project.
- Separate source evidence, authored narrative derivation, and host binding.
- Require human approval for premise, canon, meaning, intentional deviation,
  source-conflict policy, and acceptable fidelity tradeoffs.
- Keep narrative readiness and conformance separate from build success and
  runtime consumption. Runtime evidence may support playable realization but
  cannot approve meaning.
- Reuse existing project-native ledgers and plans when they already own the
  required meanings. Add records only for missing contracts.

## Reference Routing

| Current judgment | Read |
| --- | --- |
| Select narrative relation, source roles, and dependency gates | `references/strategy/narrative-derivation.md` |
| Normalize source editions, scenes, state transitions, and canon constraints | `references/conventions/source-ledger-fields.md` |
| Define authored narrative units and their derivation from zero or more sources | `references/conventions/narrative-plan-fields.md` |
| Bind authored units to stable host surfaces without absorbing implementation data | `references/conventions/host-binding-fields.md` |
| Predeclare mode-aware readiness and narrative conformance claims | `references/conventions/narrative-assessment-profiles.md` |

## Core Invariants

- Never invent a source event, order, state, or edition relationship to close a
  ledger gap.
- Never decide an absolute canon when the person or source-owning project has
  not granted that authority.
- Never use one direct source-scene-to-host-surface table as a substitute for
  the authored narrative plan.
- Never treat a deliberate divergence, continuation, or synthesis as failed
  fidelity merely because it differs from a source outside its declared
  preservation scope.
- Never copy source evidence, approvals, execution receipts, or observations
  into narrative records. Refer to their stable identities.
- Never let a narrative requirement choose the actual portrait, sprite, map
  asset, byte write, builder, or observer. Emit requirement and surface
  references for their owners.

## Expected Outputs

Produce only the artifact that advances the current narrative decision: a
source-role declaration, bounded source ledger, authored unit, derivation
relation, host binding, readiness assessment, conformance assessment, or an
explicit unresolved question. When composed with a fan-game orchestrator,
export stable artifact IDs, assessment outcome and scope, limits, and blocked
dependencies rather than transferring ownership of the underlying records.
