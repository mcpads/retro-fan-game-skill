# Resource Insertion

Resource insertion adds something the original game did not already expose as a
replaceable slot. It is higher risk than replacement because storage is only one
link in the runtime path.

## Preference Order

Use the lowest-risk option that can express the overlay:

1. Reuse or repurpose a proven slot.
2. Extend a table, archive, or bank already scanned by the game.
3. Point an existing entry at a proven free or appended region.
4. Add a new entry and update every owning count and index.
5. Add a loader hook only when data-level extension cannot reach the surface.

Do not insert merely because it is cleaner for authoring. Choose it only when
replacement would create greater content loss or runtime risk.

## Runtime Asset Chain

Before insertion, prove the relevant chain:

`storage -> discovery -> load or transform -> residence -> consumption -> retirement`

The proof must cover the owning table or lookup, identities and counts, format
and media rules, memory destination and lifetime, failure behavior, and adjacent
resources that could be shifted or shadowed. Any unknown link keeps insertion a
hypothesis.

Record concrete insertion fields in
`references/conventions/structure-map-fields.md`. Record planned mutations and
their checks in `references/conventions/execution-records.md`.

## Minimal Proof

The first insertion should be one small observable resource. Verify both the new
resource and a relevant adjacent old resource through the real consumption path.
This is the evidence that table shifts, caches, fallbacks, and retirement rules
did not silently damage the surrounding game.

## Distribution Branch

Newly authored or generated resources may be shareable with provenance. Derived
original resources remain local transforms or deltas. Never include a rebuilt
archive or game image merely because it contains one new resource; apply
`references/strategy/asset-distribution-policy.md` when sharing is in scope.
