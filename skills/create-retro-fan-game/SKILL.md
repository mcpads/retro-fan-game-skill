---
name: create-retro-fan-game
description: >-
  Create personal playable retro fan games and ROM hacks from user-owned games.
  Use for alternate scenarios, story ports onto another game's engine, dialogue,
  art, or music overlays, rule and map changes, structure investigation,
  resource insertion, local builds, and optional shareable patch recipes. Covers
  unclear initial ideas and resuming existing projects. Translation-only patches
  are out of scope. 레트로 게임 팬게임·롬핵·개조·대체 시나리오의 신규 제작과 기존
  프로젝트 후속 작업에 사용한다.
---

# Create Retro Fan Game

Help the person play the work they want. They choose the experience, quality, and
acceptable losses; the agent investigates and implements the technical means.
A game playable on the intended personal route is a complete outcome; sharing is
optional.

## Foundational Principle

**Build the game one play segment at a time.** A play segment joins a place, the
player's purpose, interaction, dialogue and expression, success and failure, the
connection to the next segment, and resumption after saving. It is the unit of
production and proof: art, music, dialogue, and tables are made when a segment
consumes them and are finished when that segment plays. See
[Creative Overlay](references/strategy/creative-overlay.md#play-segments).

## Operating Principles

1. **Let the intended story and play decide the amount of work.** Investigate
   the engine as far as the next segment needs. Narrowing a technical question
   keeps the person's completion target. See
   [Decision Flow](references/strategy/decision-flow.md).
2. **Connect first, then present.** Connect the route early with visible
   placeholders when that exposes progression risk sooner. A placeholder stays
   open until it is replaced or the person accepts it. See
   [Placeholders](references/conventions/artifact-states.md#placeholders).
3. **Let the person judge meaning and taste.** The agent establishes technical
   facts, measures constraints, and prepares candidates. The person decides
   premise, canon, character, tone, appearance, sound, and acceptable loss. See
   [Intent And Authority](references/strategy/intent-and-authority.md) and
   [Creative Review](references/strategy/creative-review.md).
4. **Tie every claim to exact inputs.** Preserve originals and raw evidence, tie
   builds and observations to content identities, and keep hypotheses apart from
   established facts. See [Workflow Gates](references/strategy/workflow-gates.md).

## Start Or Resume

Read only the references the next decision needs.

- Existing work: recover the current entry with
  [Project State](references/conventions/project-state.md).
- New or unclear idea: establish the playable target with
  [Intent And Authority](references/strategy/intent-and-authority.md).
- Unknown host or engine path: start with
  [Technical Investigation](references/strategy/technical-investigation.md).
- Choose the next action with
  [Decision Flow](references/strategy/decision-flow.md).

Write the project's authority owners, input and storage boundaries, and
implementation gates into its own agent instructions or README, so later sessions
follow the project.

## Boundaries

- Change the surfaces and dependencies the intended segments need. A surface is
  an editable part of the host game, such as a dialogue table or portrait set.
- Keep original game images, extracted original assets, and rebuilt full game
  images local. A private store the person controls holds them only on the
  person's explicit instruction, recorded with its inventory. Shared material
  follows [Asset Distribution Policy](references/strategy/asset-distribution-policy.md).
- Test unknowns with small experiments before expanding production under
  [Workflow Gates](references/strategy/workflow-gates.md).

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
| Investigate or adopt new resource insertion or saved state | [Resource Insertion](references/strategy/resource-insertion.md) |
| Select runtime evidence and diagnose failures | [Runtime Observation](references/strategy/runtime-observation.md) |
| Classify material for sharing | [Asset Distribution Policy](references/strategy/asset-distribution-policy.md) |
| Prepare an optional shareable builder or patch | [Optional Patch Package](references/strategy/patch-package.md) |

Record fields live in `references/conventions/`; open one when a decision needs
that record. When an observation or repeated rejection feels familiar, search
the [case index](references/tips/README.md) by the direct observation.

## Deliver The Next Useful Result

Show what changed in the game, what has been observed, and any choice that remains
with the person. Update the current entry when selected work or the next action
changes.
