# Execution Records

Execution records make local mutation inspectable and replaceable. They prove
what a builder was asked to do and what it produced; they do not prove runtime
consumption.

## Expected Write

Before applying a binary or container mutation, record:

- one owning change or overlay unit,
- source identity and source coordinate or logical object,
- allowed range, object, or container boundary,
- expected source bytes or an equivalent source condition,
- final bytes or deterministic derivation,
- relevant alignment, relocation, checksum, compression, or media update,
- explicit composition rule when another owner may touch the same destination,
- verification that should fail if the write is skipped or misapplied.

Fail closed when a source condition mismatches, owners overlap without a rule, a
write enters a protected boundary, a dependency is missing, or a final
difference has no owner. Do not silently carry unknown entries, failed
conversions, or missing assets into the output.

## Transform Record

For each deterministic transform, preserve:

- transform identity and version,
- verified input identities, hashes, and roles: one execution host plus any
  required user-supplied build sources,
- configuration and any structure-map identity the transform consumes,
- declared outputs and expected identity policy,
- checks that run before, during, and after the transform,
- failure result and whether partial outputs are discarded.

## Execution Receipt

Each completed run records:

- run identity,
- exact input and transform identities,
- structure-map and overlay identities when the run consumes them,
- expected-write set when the run applies mutations,
- checks executed and their pass, fail, or skipped status,
- output paths or logical IDs and hashes,
- explained and unexplained final differences when outputs are compared against
  a baseline,
- warnings, failures, and known non-deterministic inputs.

A successful receipt requires no skipped required check and, when final-diff
ownership applies, zero unexplained final differences. Runtime evidence for a
built output references the receipt identity so the observed game cannot be
confused with another build.

Evidence-only sources do not become transform inputs. When a component derives
local material from another original game, identify that game as a build source
and fail closed if its expected identity is absent or mismatched.
