# Creative Overlay

A creative overlay is the bounded fan-game layer applied to a verified base. It
may change dialogue, scenarios, routes, interface text, audiovisual assets,
rules, or a composition of those surfaces. Use
[Intent And Authority](intent-and-authority.md) to establish the playable target
when the request does not yet constrain a useful next action.

## Component Graph

Model the overlay as bounded components rather than one project-wide mode. A
component declares its creative domain, semantic source relationship, target
host surfaces, dependencies, approval boundary, and required assessments.
Relation labels may include preservation, adaptation, extension, divergence,
synthesis, replacement, restoration, or generation, but remain open to the
work's actual meaning.

The semantic relationship is independent of physical host binding. An adapted
story can reuse host events, newly authored character art can replace existing
slots, and a generated map can require insertion. Do not infer one axis from
another or require every component to share the same source.

## Scope Judgment

- Anchor every build-bound unit to a stable structure identity.
- State the intended personal route and the surfaces allowed to change.
- Preserve control, state, and runtime requirements beside the creative intent.
- Prefer changes with fewer affected dependencies when they preserve the intended
  experience; investigate broader changes when the target requires them.
- Activate a specialized domain capability only when the component claims a
  property that the core cannot assess, and consume its handoff without copying
  its records.

## Creative Brief Judgment

The brief should contain only context that constrains the current unit: approved
premise and route intent, relevant character or world state, naming rules,
required runtime elements, proven surface budgets, and forbidden
contradictions. Missing engine or story-state facts remain questions.

The concrete brief and state record is owned by
[Creative Artifact States](../conventions/artifact-states.md).

## Build Boundary

Apply [Workflow Gates](workflow-gates.md) for experiments, PoC, and broader
build-bound expansion. Apply [Intent And Authority](intent-and-authority.md) for
sample review and existing approval scope; a component graph creates no additional
approval requirement by itself.
