# Creative Overlay

A creative overlay is the set of changes applied to a verified game: dialogue,
scenarios, routes, interface text, audiovisual assets, or rules. Establish an
unclear target with [Intent And Authority](intent-and-authority.md).

## Play Segments

A play segment is the playable unit that components serve. For each segment,
define the place, the player's purpose, the interactions and information that
open the way, dialogue and expression before and after, success and failure
conditions, the connection to adjacent segments, and behavior after save,
reload, revisit, and retry. Components and host surfaces enter production when a
segment consumes them.

Keep source scenes, new play segments, and host bindings as separate records;
choose segment order from the intended play. Prove the first segment end to end,
then build later segments on its proven foundation.

## Component Graph

Define components by their creative purpose, relationship to source material,
target surfaces, dependencies, approval scope, and required assessments. A
component may preserve, adapt, extend, diverge from, combine, replace, or
restore source material, or be new work; label the actual relationship.

The source relationship and the physical host binding are separate axes. An
adapted story can reuse host events, new character art can replace existing
slots, and a new map can require insertion.

## Scope Judgment

- State the intended route, its segments, and the surfaces allowed to change.
- Link each unit intended for the build to a stable structure identity.
- Keep control, state, and runtime requirements beside the creative intent.
- Prefer changes with fewer affected dependencies when they deliver the intended
  experience; investigate broader changes when the target requires them.
- Reuse host content where the person accepts it, marked as
  [Placeholders](../conventions/artifact-states.md#placeholders) until then.
- Add specialized assessments only where a component claims them, following
  [Capability Composition](composition.md#optional-domain-capability-handoffs).

Write briefs with the [Creative Brief Record](../conventions/artifact-states.md#creative-brief-record)
and move units through [Workflow Gates](workflow-gates.md).
