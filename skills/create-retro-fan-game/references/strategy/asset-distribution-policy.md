# Asset Distribution Policy

Sharing is optional. When it is in scope, classify every artifact by its
relationship to the user's original game inputs and preserve a hard boundary
between shareable project data and material reconstructed locally from those
originals.
This document owns the skill's asset classifications and negative package
boundary; other references apply them rather than restating them.

## Asset Classes

| Class | Shareable rule |
| --- | --- |
| Original game image or extracted original asset | Never include |
| Derived original asset | Keep as a local transform or delta; do not include the reconstructed asset directly |
| Structure metadata and build recipe | Include when it does not embed recoverable original content |
| Newly authored asset | Include when provenance and rights assumptions are recorded |
| Generated asset | Include when provenance, approval state, and runtime validation are recorded |
| Runtime evidence or preview | Include only when necessary, scoped, and reviewed for original content |

Concrete provenance fields belong to
`references/conventions/artifact-states.md`; package fields belong to
`references/conventions/package-manifest.md`.

## Package Boundary

A shareable package may remain independently useful as writing, artwork,
metadata, or tooling. The required boundary is narrower and testable: without
the expected user-supplied original inputs, it must not build a playable target
or reconstruct meaningful original assets from any omitted input.

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
