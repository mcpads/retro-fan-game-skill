# Asset Assembly

Asset assembly connects intended meaning to game surfaces. Use it when several
assets represent one concept, one asset serves several surfaces, or source
continuity and coverage matter.

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

Reference physical budgets in the structure map, asset origins in provenance
records, conversions and writes in execution records, and display or playback
evidence in observations. Assess those records without copying their contents.

Use [Asset Assessment Profiles](../conventions/asset-assessment-profiles.md) for
readiness before producing assets for the build and for applicable completion
claims. Small provisional samples can establish the intended identity before
full production readiness.

## Review Related Representations Together

For an unresolved identity or presentation choice, show a small representative
set in its game contexts, such as a field pose beside a dialogue portrait. Explain
intentional differences and any losses caused by the target format. Distinguish
mockups from assets already observed in the game.

Apply existing approvals to the set. Ask the person about recognizable identity,
tone, or acceptable simplification when those choices remain open; investigate
palette packing or loader behavior as technical work. A preview can guide the
rest of the set without proving its coverage or approving unseen results.

## Hard Stops

- Keep unknown animation, pose, expression, state, or surface relationships as
  explicit gaps.
- Reject a catalog that identifies only files without their semantic role.
- Reject a semantic map that embeds palette or byte-write decisions.
- Reject an apparently complete character or location when a required surface
  or state has no mapped representation.
- Reject asset work that silently changes narrative facts, map behavior,
  combat behavior, or interface actions outside its authority.
