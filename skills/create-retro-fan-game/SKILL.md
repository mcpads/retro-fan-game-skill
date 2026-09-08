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

Help the person play the work they want. They choose the experience, quality, and
acceptable losses; the agent investigates and implements the technical means.
Use automated checks for mechanical errors and game observation for runtime
behavior.

Keep creative policy, execution, and observation replaceable. No particular
repository, tool, or additional skill is required. A game playable on the intended
personal route is a complete outcome; sharing is optional.

## Start Or Resume

Read only the references needed for the next decision, not the entire catalog.

- For existing work, use [Project State](references/conventions/project-state.md)
  to recover current decisions, selected work, and valid evidence.
- For a new or unclear idea, use
  [Intent And Authority](references/strategy/intent-and-authority.md) to establish
  the playable target and unresolved choices.
- When the host or an affected engine path is unknown, start with
  [Technical Investigation](references/strategy/technical-investigation.md).
- Choose the next action with
  [Fan-game Decision Flow](references/strategy/fan-game-pipeline.md).

## Working Principles

- Preserve original inputs and raw evidence. Correct interpretations without
  rewriting observations, and distinguish hypotheses from established facts.
- Work only on surfaces and dependencies needed by the intended route. A surface
  is an editable part of the host game, such as a dialogue table or portrait set.
- Investigate unknowns with small experiments before expanding production; apply
  [Workflow Gates](references/strategy/workflow-gates.md).
- Reuse existing records. Different responsibilities need not require separate
  files, tools, or agents.
- Keep original game images, extracted copyrighted assets, and rebuilt full game
  images out of commits and packages. Sharing classifications belong to
  [Asset Distribution Policy](references/strategy/asset-distribution-policy.md).

## Strategy Routing

| Current decision | Read |
| --- | --- |
| Select executor, observer, or specialized domain capabilities | [Capability Composition](references/strategy/composition.md) |
| Distinguish analysis, tooling builds, product builds, tests, and verification | [Work Roles](references/conventions/work-roles.md) |
| Judge relevant structure evidence and gaps | [Structure-map Readiness](references/strategy/structure-map.md) |
| Admit an experiment or judge PoC, expansion, private completion, or sharing | [Workflow Gates](references/strategy/workflow-gates.md) |
| Bound components, source relationships, and changed surfaces | [Creative Overlay](references/strategy/creative-overlay.md) |
| Generate or author candidate assets | [Asset Generation](references/strategy/asset-generation.md) |
| Investigate or adopt new resource insertion | [Resource Insertion](references/strategy/resource-insertion.md) |
| Select runtime evidence and diagnose failures | [Runtime Observation](references/strategy/runtime-observation.md) |
| Classify material for sharing | [Asset Distribution Policy](references/strategy/asset-distribution-policy.md) |
| Prepare an optional shareable builder or patch | [Optional Patch Package](references/strategy/patch-package.md) |

## Record Routing

Read only the relevant record sections. Create no records for inactive domains,
resource insertion, or sharing.

| Record | Read |
| --- | --- |
| Base identity, surface facts, and conditional insertion registry | [Structure-map Fields](references/conventions/structure-map-fields.md) |
| Component scope, brief, approval, content state, and asset provenance | [Creative Artifact States](references/conventions/artifact-states.md) |
| Product build path, expected writes, transforms, and run receipts | [Execution Records](references/conventions/execution-records.md) |
| Raw evidence and collection limits | [Observation Records](references/conventions/observation-records.md) |
| Evidence interpretation and pass/fail decisions | [Claim Assessments](references/conventions/claim-assessments.md) |
| Conditional package inventory and clean-workspace checks | [Package Manifest](references/conventions/package-manifest.md) |

## Deliver The Next Useful Result

Show what changed in the game, what has been observed, and any choice that remains
with the person. Update the current-state entry when selected work or the next
action changes.
