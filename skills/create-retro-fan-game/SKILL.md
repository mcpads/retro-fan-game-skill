---
name: create-retro-fan-game
description: >-
  Build personal retro fan-game workflows from a verified execution-host game,
  optional user-supplied source games, and a proven or newly established
  structure map. Use when the user wants a
  private fan game, alternate scenario, dialogue or asset overlay, generated
  content pack, new resource insertion plan, local patch recipe, or an optional
  shareable builder that does not redistribute original game assets. Trigger
  for "fan game", "fanfic game", "personal patch", "AI-generated scenario",
  "structure map", "creative overlay", "new resource", "resource insertion",
  "ROM mod recipe", or requests to turn retro-game reverse engineering into a
  personal playable work while keeping philosophy, execution, and observation
  independently replaceable.
---

# Create Retro Fan Game

## Overview

Help a person create and consume a fan game from an original game they possess.
Map only the surfaces the intended work needs, preserve human authority over
high-impact creative choices, build locally, and prove runtime claims with an
observer suited to the claim. Treat a translation patch as one possible source
of structure evidence; do not require a parent skill, repository, builder, or
observer by name.

Compose bounded creative components whose source relationships may differ. Do
not force the whole work into one port, reskin, remix, or total-conversion mode;
the exact component judgment belongs to
`references/strategy/creative-overlay.md`.

Treat a private playable as a first-class outcome. Open the sharing branch only
when the person asks for it or the current project has already declared it in
scope.

## Operating Model

Use this as a decision system, not a fixed sequence. Reconstruct the available
project state, state the next decision, and seek the cheapest evidence that can
change it. Advance independent branches in parallel when useful, but never skip
a dependency gate merely because another branch is ready.

Begin by establishing:

- the creative target, intended personal route, and completion target,
- the bounded creative components, their dependencies, semantic source
  relationships, target host surfaces, and required domain capabilities,
- which high-impact decisions require the person's approval and which
  lower-impact decisions they have explicitly delegated,
- the exact execution-host input and any additional build-source or
  evidence-only original inputs available locally,
- the relevant surface facts, hypotheses, evidence, and gaps,
- the current claim and what success, failure, or ambiguity would change.

Read `references/strategy/fan-game-pipeline.md` for the non-linear decision
model and `references/strategy/composition.md` before selecting executor or
observer capabilities.

## Dependency Gates

- Identify the base before applying or evaluating build mutations.
- Prove the relevant surface's extraction and rebuild behavior before committing
  broad generated content to that surface. Premise and brief exploration may
  proceed earlier as explicitly provisional creative work.
- Prove one minimal creative unit through the real game-consumption path before
  expanding the corresponding build-bound overlay.
- For a component that claims an external source meaning, cross-surface
  coherence, behavior equivalence, world reachability, or another specialized
  property, require the applicable domain capability's readiness assessment
  before broad build-bound expansion.
- Prove the discovery, load, residence, consumption, and retirement path before
  inserting a resource the original game did not expose.
- Obtain sufficient game-visible evidence before claiming private playability.
- Treat shareable packaging as a conditional branch with its own clean-workspace
  and asset-boundary checks, never as a prerequisite for personal completion.

The exact pass conditions are owned by
`references/strategy/workflow-gates.md`.

## Strategy Routing

| Current judgment | Read |
| --- | --- |
| Decide which branch can move next | `references/strategy/fan-game-pipeline.md` |
| Separate creative policy, execution, and observation | `references/strategy/composition.md` |
| Decide whether a surface is ready for build-bound creative work | `references/strategy/structure-map.md` |
| Evaluate PoC, private-playable, or optional sharing gates | `references/strategy/workflow-gates.md` |
| Bound story, route, dialogue, UI, asset, or rule changes | `references/strategy/creative-overlay.md` |
| Decide how generated or newly authored assets may enter the work | `references/strategy/asset-generation.md` |
| Decide whether replacement is insufficient and insertion is justified | `references/strategy/resource-insertion.md` |
| Select evidence for a runtime claim and close observation gaps | `references/strategy/runtime-observation.md` |
| Classify what may remain local or enter a shareable package | `references/strategy/asset-distribution-policy.md` |
| Decide whether and how to open the optional packaging branch | `references/strategy/patch-package.md` |

## Convention Routing

| Artifact or record | Read |
| --- | --- |
| Structure-map fields and conditional insertion fields | `references/conventions/structure-map-fields.md` |
| Creative brief, approval, content state, and provenance records | `references/conventions/artifact-states.md` |
| Expected writes, deterministic transforms, and execution receipts | `references/conventions/execution-records.md` |
| Observer-produced raw evidence and collection limits | `references/conventions/observation-records.md` |
| Claim interpretation, evidence sufficiency, and gate promotion | `references/conventions/claim-assessments.md` |
| Conditional shareable package manifest and clean-workspace test | `references/conventions/package-manifest.md` |

## Core Invariants

- Never commit or package original game images, extracted copyrighted assets, or
  rebuilt full game images.
- Keep philosophy, execution, and observation independently replaceable. State
  claims and evidence contracts without mandating products by name.
- Treat execution success as proof that a declared transform completed, not as
  proof that the game consumed the result correctly.
- Keep the original baseline and extracted structure evidence immutable.
  Creative work is an overlay against stable identities.
- Keep the execution host distinct from optional build-source and evidence-only
  inputs. A source role does not grant host-structure or semantic authority.
- Reuse and extend an existing project-native structure, manifest, or record when
  it already owns the required meaning. Introduce a new artifact only when no
  equivalent owner exists.
- Let AI draft inside proven constraints, but never let it invent missing engine
  or story-state facts. Preserve unknowns as gaps or questions.
- Do not absorb domain analysis into the core. Consume stable prepared-artifact
  and assessment references from compatible optional capabilities, while
  leaving their meaning and criteria with their owners.
- Return premise, character, meaning, canon, tone, and acceptable-risk decisions
  to the person. Exercise delegated authority only inside its recorded scope.
- Prefer reuse or replacement before insertion, and require evidence across the
  actual runtime asset chain for any insertion.
- Treat story-state breaks, softlocks, missing required assets, and unobserved
  changed routes as blockers for the affected private route.
- When sharing is in scope, apply the classifications and package boundary owned
  by `references/strategy/asset-distribution-policy.md`; do not improvise a
  stricter rule that excludes legitimate new work or a weaker rule that exposes
  original material.
- Do not assume a nearby repository, translation patch, or particular
  implementation is available.

## Expected Outputs

Produce the smallest durable artifact that advances the current decision. That
may be a structure gap list, fact/hypothesis/evidence table, creative brief,
component scope or capability handoff, one-unit PoC, overlay state update,
execution receipt, raw observation, claim assessment, or a narrow
implementation change. Extend the project's existing equivalent artifact
before proposing a new filename or schema.

Create an inserted-resource registry only when insertion is in scope. Create a
package manifest and clean-workspace evidence only when sharing is in scope. If
the user asks for broad direction, first inventory the available workspace and
identify the unresolved gate whose evidence would most reduce uncertainty.
