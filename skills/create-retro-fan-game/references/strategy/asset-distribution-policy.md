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
| Runtime evidence or preview | Include only when necessary, scoped, and reviewed for original content |

Use [Creative Artifact States](../conventions/artifact-states.md) for provenance
fields and [Package Manifest](../conventions/package-manifest.md) for inventory
and reconstruction checks.

## Package Boundary

A package may be useful on its own as writing, artwork, metadata, or tooling.
Without the expected original inputs, it must not build the playable target or
reconstruct meaningful original assets from any omitted input.

The local builder validates the execution host and every required build-source
identity, reconstructs derived data locally, and emits rebuilt game outputs
only to local ignored paths. Evidence-only sources do not become package build
requirements. Sharing a rebuilt archive or full image is not made acceptable
by the presence of one new asset.

## Review Questions

- Can package data reveal meaningful original content without the original?
- Is a generated or authored asset actually a disguised copy of extracted
  material?
- Are previews necessary and limited to the claim they support?
- Can every derived asset be recreated locally from its declared expected
  original input?
- Can every inserted resource be explained without bundling original data?
- Does the optional clean-workspace reconstruction satisfy the declared package
  scope?

This is an engineering boundary for reducing redistribution risk, not legal
advice.
