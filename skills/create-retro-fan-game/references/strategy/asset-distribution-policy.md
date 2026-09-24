# Asset Distribution Policy

When sharing is in scope, classify each artifact by its relationship to the
original game inputs.

## Asset Classes

| Class | Shareable rule |
| --- | --- |
| Original game image or extracted original asset | Stays local |
| Derived original asset | Shared as a local transform or delta |
| Structure metadata and build recipe | Shared when it embeds no recoverable original content |
| Newly authored asset | Shared with provenance and rights assumptions recorded |
| Generated asset | Shared with provenance, approval, and runtime validation recorded |
| Runtime evidence or preview | Shared under [Preview Evidence](#preview-evidence) |

Record provenance in [Creative Artifact States](../conventions/artifact-states.md)
and inventory in [Package Manifest](../conventions/package-manifest.md).

## Package Boundary

A package may stand alone as writing, artwork, metadata, or tooling. The playable
target and every original asset come only from the recipient's own originals: the
local builder validates each required input identity, reconstructs derived data
locally, and writes rebuilt game outputs to ignored local paths. Rebuilt archives
and full images stay local however much new material they contain.

## Preview Evidence

Include the frames, regions, or audio duration a declared claim needs, with the
original scenery, interface, or sound required to understand the change. Review
all exports together so they cannot serve as an asset set, script dump, or
reconstruction. Save states, memory dumps, and game archives stay local. Classify
by actual content, keep raw observations local with any crop or redaction
recorded, and keep previews out of the build.

This is an engineering boundary for reducing redistribution risk, not legal
advice.
