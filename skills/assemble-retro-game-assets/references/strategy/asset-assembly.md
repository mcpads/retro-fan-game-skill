# Asset Assembly

Asset assembly owns the semantic layer between creative intent and proven host
surfaces. It applies when several assets represent one concept, one asset must
serve several surfaces, or source-aware continuity and coverage matter.

## Open Asset Profiles

Profiles may include:

- field characters, NPCs, and animation-state sets,
- battle actors, enemies, formations, and visual effects,
- maps, tilesets, backgrounds, props, and environmental states,
- portraits, expressions, cutscene frames, and staged character surfaces,
- items, equipment, status marks, cursors, and interface icons,
- music, ambience, voice, and event cues when audio is in scope.

These are discovery aids, not a universal enum. Add the profile required by the
host and intended work. A map graphic belongs here; collision, topology, warps,
and reachability do not. A battle sprite belongs here; hitboxes, AI, damage, and
timing behavior do not.

## Separate Semantic And Physical Relations

Semantic relations describe meaning: preserve, variant, retarget, merge, split,
substitute, remix, or newly author. Physical host binding describes how a
proven surface is reused, replaced, repurposed, extended, inserted, or hooked.
Do not derive one from the other.

One character may map to field sprites, portraits, battle graphics, cutscene
frames, and UI icons. Several source assets may merge into one host sheet, and
one source sheet may split across several host surfaces. Preserve these
many-to-many relations.

## Ownership Flow

Keep the flow separable:

`source or authored intent -> semantic asset unit -> host-surface mapping`

The host structure owner supplies physical budgets. The provenance owner
records newly authored or generated artifacts. Execution owns conversion and
writes. Observation owns raw display or playback evidence. The assessment
combines references without copying them.

Before broad production, require a readiness assessment for the declared asset
component. Before claiming completion, require coverage and coherence, plus
source conformance when adaptation is part of the claim. Runtime visibility is
necessary for a display claim but insufficient for semantic approval.

## Hard Stops

- Keep unknown animation, pose, expression, state, or surface relationships as
  explicit gaps.
- Reject a catalog that identifies only files without their semantic role.
- Reject a semantic map that embeds palette or byte-write decisions.
- Reject an apparently complete character or location when a required surface
  or state has no mapped representation.
- Reject asset work that silently changes narrative facts, map behavior,
  combat behavior, or interface actions outside its authority.
