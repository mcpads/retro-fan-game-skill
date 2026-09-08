---
name: create-retro-fan-game
description: >-
  Create personal playable retro fan games and ROM mods from user-owned games.
  Use for alternate scenarios, dialogue or asset overlays, rule changes,
  structure investigation, resource insertion, local builds, and optional
  shareable patch recipes. Covers unclear initial ideas and resuming existing
  projects; a structure map or translation patch is not a prerequisite.
---

# Create Retro Fan Game

Help the person play the work they want. The person chooses the intended
experience, quality, and acceptable losses; the agent investigates and implements
the technical means. Automated checks reject mechanically detectable mistakes,
and game observation supplies evidence for runtime claims.

Keep creative policy, execution, and observation replaceable. No particular
repository, translation patch, tool, or additional skill is required by name.
A private playable is a complete outcome; sharing is an optional scope.

## Start Or Resume

Read only the references needed for the next decision, not the entire catalog.

- For a new or unclear idea, use
  [Intent And Authority](references/strategy/intent-and-authority.md) to turn the
  person's wishes into concrete choices and a bounded playable target.
- For existing work, locate the project's current-state entry and reconcile it
  under [Project State](references/conventions/project-state.md). Carry forward
  existing decisions and valid evidence before creating or rerunning anything.
- Choose the next useful investigation, sample, implementation, or observation
  with [Fan-game Decision Flow](references/strategy/fan-game-pipeline.md).

## Working Principles

- Preserve original inputs and raw evidence. Correct interpretations without
  rewriting the observations that supported them.
- Keep hypotheses visible. An inherited format rule, generated draft, successful
  build, and observed playable each support different claims.
- Work only on surfaces and dependencies needed by the intended route. A surface
  is an editable part of the host game, such as a dialogue table or portrait set.
- Use bounded experiments to resolve unknowns; apply
  [Workflow Gates](references/strategy/workflow-gates.md) before promoting their
  results into broader production or completion claims.
- Reuse project-native records. Separate meanings and ownership without requiring
  separate files, tools, or agents; see
  [Capability Composition](references/strategy/composition.md).
- Keep original game images, extracted copyrighted assets, and rebuilt full game
  images out of commits and packages. Sharing classifications belong to
  [Asset Distribution Policy](references/strategy/asset-distribution-policy.md).

## Strategy Routing

| Current decision | Owner |
| --- | --- |
| Clarify the intended experience, present choices, or interpret approval | [Intent And Authority](references/strategy/intent-and-authority.md) |
| Select the next branch of work | [Fan-game Decision Flow](references/strategy/fan-game-pipeline.md) |
| Select executor, observer, or specialized domain capabilities | [Capability Composition](references/strategy/composition.md) |
| Judge relevant structure evidence and gaps | [Structure-map Readiness](references/strategy/structure-map.md) |
| Admit an experiment or judge PoC, expansion, private completion, or sharing | [Workflow Gates](references/strategy/workflow-gates.md) |
| Bound components, source relationships, and changed surfaces | [Creative Overlay](references/strategy/creative-overlay.md) |
| Generate or author candidate assets | [Asset Generation](references/strategy/asset-generation.md) |
| Investigate or adopt new resource insertion | [Resource Insertion](references/strategy/resource-insertion.md) |
| Select runtime evidence and diagnose failures | [Runtime Observation](references/strategy/runtime-observation.md) |
| Classify material for sharing | [Asset Distribution Policy](references/strategy/asset-distribution-policy.md) |
| Prepare an optional shareable builder or patch | [Optional Patch Package](references/strategy/patch-package.md) |

## Record Routing

These conventions describe required meanings when applicable, not a checklist
of artifacts to create for every request.

| Record | Owner |
| --- | --- |
| Current selection, resume, research adoption, and invalidation | [Project State](references/conventions/project-state.md) |
| Base identity, surface facts, and conditional insertion registry | [Structure-map Fields](references/conventions/structure-map-fields.md) |
| Component scope, brief, approval, content state, and asset provenance | [Creative Artifact States](references/conventions/artifact-states.md) |
| Expected writes, deterministic transforms, and run receipts | [Execution Records](references/conventions/execution-records.md) |
| Raw evidence and collection limits | [Observation Records](references/conventions/observation-records.md) |
| Evidence interpretation and gate promotion | [Claim Assessments](references/conventions/claim-assessments.md) |
| Conditional package inventory and clean-workspace checks | [Package Manifest](references/conventions/package-manifest.md) |

## Deliver The Next Useful Result

Produce the smallest durable change that advances the intended playable. Show
the person what changed in the game, what has been observed, and any choice
that remains theirs. Update the existing current-state entry when the selected
work or next action changes. Do not create empty records for inactive domains,
resource insertion, or sharing.
