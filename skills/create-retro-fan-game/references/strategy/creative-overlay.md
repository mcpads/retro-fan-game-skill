# Creative Overlay

A creative overlay is the set of changes applied to a verified game: dialogue,
scenarios, routes, interface text, audiovisual assets, or rules. Establish an
unclear target with [Intent And Authority](intent-and-authority.md).

## Play Segments

A play segment is the playable unit that components serve. For each segment,
define the place, the player's purpose, the interactions and information that
open the way, dialogue and expression before and after, success and failure
conditions, the connection to adjacent segments, and behavior after save,
reload, revisit, and retry. Bind components and host surfaces through the
segments that consume them; an asset or table enters production when a segment
needs it.

Keep source scenes, new play segments, and host bindings as separate records.
A source's order or unresolved gaps do not become execution order by default.
Prove the first segment end to end before expanding; later segments reuse its
proven foundation instead of reopening it.

## Component Graph

Define components by their creative purpose, relationship to source material,
target surfaces, dependencies, approval scope, and required assessments. Each
may preserve, adapt, extend, diverge from, combine, replace, or restore source
material, or contain new work. Choose labels that describe the actual relationship.

The semantic relationship is independent of physical host binding. An adapted
story can reuse host events, newly authored character art can replace existing
slots, and a generated map can require insertion. Do not infer one axis from
another or require every component to share the same source.

## Scope Judgment

- Link each unit intended for the build to a stable structure identity.
- State the intended personal route, its segments, and the surfaces allowed to
  change.
- Preserve control, state, and runtime requirements beside the creative intent.
- Prefer changes with fewer affected dependencies when they preserve the intended
  experience; investigate broader changes when the target requires them.
- Reuse host content where the person accepts it, and mark stand-ins under
  [Placeholders](../conventions/artifact-states.md#placeholders).
- Use specialized assessments only where needed, following
  [Capability Composition](composition.md#optional-domain-capability-handoffs).

## Creative Brief Judgment

Include only context needed to author and validate the current unit. Use
[Creative Brief Record](../conventions/artifact-states.md#creative-brief-record)
for fields, keeping unknown engine or story-state facts explicit.

## Build Boundary

Apply [Workflow Gates](workflow-gates.md) for experiments, PoC, and broader
production. Defining components does not create additional approval requirements.
