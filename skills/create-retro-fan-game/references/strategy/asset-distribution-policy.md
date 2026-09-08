# Asset Distribution Policy

When sharing is in scope, classify each artifact by its relationship to the
user's original game inputs. This policy defines what may be included and what
must be reconstructed locally from those originals.

## Asset Classes

| Class | Shareable rule |
| --- | --- |
| Original game image or extracted original asset | Never include |
| Derived original asset | Keep as a local transform or delta; do not include the reconstructed asset directly |
| Structure metadata and build recipe | Include when it does not embed recoverable original content |
| Newly authored asset | Include when provenance and rights assumptions are recorded |
| Generated asset | Include when provenance, approval state, and runtime validation are recorded |
| Runtime evidence or preview | Include only under [Preview Evidence](#preview-evidence) |

Use [Creative Artifact States](../conventions/artifact-states.md) for provenance
fields and [Package Manifest](../conventions/package-manifest.md) for inventory
and reconstruction checks.

## Package Boundary

A package may be useful on its own as writing, artwork, metadata, or tooling.
Without the expected original inputs, it must not build the playable target or
supply or reconstruct original assets from any omitted input. Limited original
context in [Preview Evidence](#preview-evidence) is the only exception for evidence
exports; it is not an exception for build inputs.

The local builder validates the execution host and every required build-source
identity, reconstructs derived data locally, and emits rebuilt game outputs
only to local ignored paths. Evidence-only sources do not become package build
requirements. Sharing a rebuilt archive or full image is not made acceptable
by the presence of one new asset.

## Preview Evidence

Include only the frames, regions, or audio duration needed to support a declared
claim. Original scenery, interface, or sound may remain when needed to understand
the changed behavior; remove unrelated material from the export.

Review the exact exports together. They must not serve as extracted asset sets,
script dumps, or a collection that reconstructs original assets beyond the
necessary context. Save states, memory dumps, and game archives are not previews.
Classify actual content, not its filename or a generated or authored label.

Preserve raw observations locally and record any cropping, redaction, or other
export transform separately. Keep previews out of the build dependency chain.
Record their purpose, retained original context, and review result in the
[Package Manifest](../conventions/package-manifest.md#included-artifact-inventory).

This is an engineering boundary for reducing redistribution risk, not legal
advice.
