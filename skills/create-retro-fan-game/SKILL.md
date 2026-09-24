---
name: create-retro-fan-game
description: >-
  Create personal playable retro fan games and ROM hacks from user-owned games.
  Use for alternate scenarios, story ports onto another game's engine, dialogue,
  art, or music overlays, rule and map changes, structure investigation,
  resource insertion, local builds, and optional shareable patch recipes. Covers
  unclear initial ideas and resuming existing projects; a structure map or
  translation patch is not a prerequisite. Translation-only patches are out of
  scope. 레트로 게임 팬게임·롬핵·개조·대체 시나리오의 신규 제작과 기존 프로젝트
  후속 작업에 사용한다.
---

# Create Retro Fan Game

Help the person play the work they want. They choose the experience, quality, and
acceptable losses; the agent investigates and implements the technical means.
A game playable on the intended personal route is a complete outcome; sharing is
optional. No particular repository, tool, or additional skill is required.

## Foundational Principle

**Build the game one play segment at a time.** A play segment joins a place, the
player's purpose, interaction, dialogue and expression, success and failure, the
connection to the next segment, and resumption after saving. It is the unit of
production and proof. Do not mass-produce art, music, or dialogue before a
segment consumes it, and do not credit a surface, table, or asset as finished
apart from the segments that use it. See
[Creative Overlay](references/strategy/creative-overlay.md#play-segments).

## Operating Principles

1. **Let the intended story and play decide the amount of work.** The number of
   original lines, events, poses, or resources is not a measure of completeness.
   Investigate the engine as far as the next segment needs; extracting every
   feature or interpreting every original resource must not delay the playable
   work. Narrowing a technical question never shrinks the person's completion
   target. See [Decision Flow](references/strategy/decision-flow.md).
2. **Keep connection and presentation separate.** Connect the route early with
   explicit placeholders when that exposes progression risk sooner. A working
   trigger, passable tile, or temporary sprite does not complete the device,
   character, or scene it stands for. Keep each placeholder visible until it is
   replaced or the person accepts it. See
   [Placeholders](references/conventions/artifact-states.md#placeholders).
3. **Let the person judge meaning and taste.** The agent establishes technical
   facts, measures constraints, and prepares candidates. The person decides
   premise, canon, character, tone, appearance, sound, and acceptable loss.
   Self-review filters defects but never approves appearance or sound, and
   revision count is not progress. See
   [Intent And Authority](references/strategy/intent-and-authority.md) and
   [Creative Review](references/strategy/creative-review.md).
4. **Tie every claim to exact inputs.** Preserve originals and raw evidence, pin
   builds and assessments to content identities, and distinguish hypotheses from
   established facts. Segment evidence from different builds does not add up to
   one playthrough. See [Workflow Gates](references/strategy/workflow-gates.md).

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
  [Decision Flow](references/strategy/decision-flow.md).

Write the project's authority owners, input and storage boundaries, and
implementation gates into its own agent instructions or README, so later sessions
follow the project rather than this skill's wording.

## Boundaries

- Change only the surfaces and dependencies the intended segments need. A
  surface is an editable part of the host game, such as a dialogue table or
  portrait set.
- Keep original game images, extracted original assets, and rebuilt full game
  images out of anything shared or published. A private store the person
  controls may hold such material only on their explicit instruction; record
  that exception and its inventory. Sharing classifications belong to
  [Asset Distribution Policy](references/strategy/asset-distribution-policy.md).
- Investigate unknowns with small experiments before expanding production; apply
  [Workflow Gates](references/strategy/workflow-gates.md).
- Reuse existing records. Different responsibilities need not require separate
  files, tools, or agents.

## Strategy Routing

| Current decision | Read |
| --- | --- |
| Select executor, observer, or specialized domain capabilities | [Capability Composition](references/strategy/composition.md) |
| Distinguish analysis, tooling builds, product builds, tests, and verification | [Work Roles](references/conventions/work-roles.md) |
| Judge relevant structure evidence and gaps | [Structure-map Readiness](references/strategy/structure-map.md) |
| Admit an experiment or judge PoC, expansion, private completion, or sharing | [Workflow Gates](references/strategy/workflow-gates.md) |
| Define play segments, components, source relationships, and changed surfaces | [Creative Overlay](references/strategy/creative-overlay.md) |
| Generate or author candidate assets | [Asset Generation](references/strategy/asset-generation.md) |
| Present art, sound, or text for the person's judgment | [Creative Review](references/strategy/creative-review.md) |
| Investigate or adopt new resource insertion | [Resource Insertion](references/strategy/resource-insertion.md) |
| Select runtime evidence and diagnose failures | [Runtime Observation](references/strategy/runtime-observation.md) |
| Classify material for sharing | [Asset Distribution Policy](references/strategy/asset-distribution-policy.md) |
| Prepare an optional shareable builder or patch | [Optional Patch Package](references/strategy/patch-package.md) |

When an observation, repeated rejection, or accumulating exception suggests a
familiar trap, search the [case index](references/tips/README.md) by the direct
observation. Cases suggest hypotheses, not repairs.

## Record Routing

Read only the relevant record sections. Create no records for inactive domains,
resource insertion, or sharing.

| Record | Read |
| --- | --- |
| Base identity, surface facts, and conditional insertion registry | [Structure-map Fields](references/conventions/structure-map-fields.md) |
| Component scope, brief, approval, placeholders, and asset provenance | [Creative Artifact States](references/conventions/artifact-states.md) |
| Product build path, expected writes, transforms, and run receipts | [Execution Records](references/conventions/execution-records.md) |
| Raw evidence and collection limits | [Observation Records](references/conventions/observation-records.md) |
| Evidence interpretation and pass/fail decisions | [Claim Assessments](references/conventions/claim-assessments.md) |
| Conditional package inventory and clean-workspace checks | [Package Manifest](references/conventions/package-manifest.md) |

## Deliver The Next Useful Result

Show what changed in the game, what has been observed, and any choice that remains
with the person. Update the current-state entry when selected work or the next
action changes.
