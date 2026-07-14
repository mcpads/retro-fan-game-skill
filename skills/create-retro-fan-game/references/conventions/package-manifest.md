# Package Manifest

Create this manifest only when sharing is explicitly in scope. It describes how
another owner of every required original input can reproduce the declared local
target; it is not required for a private playable.

## Required Identity

Record:

- package name, version, and declared overlay scope,
- execution-host identity and accepted input sizes and hashes,
- every additional required build-source identity, role, accepted size, and
  hash,
- evidence-only source identities without making them build requirements,
- structure-map, overlay, transform, and builder identities,
- local output identity policy,
- supported environment assumptions and known limitations.

## Included Artifact Inventory

For every included file or logical artifact, record:

- path or stable ID, hash, and purpose,
- asset class from
  `references/strategy/asset-distribution-policy.md`,
- provenance record for newly authored or generated assets,
- local transform or delta relationship for derived original assets,
- dependency and deterministic build step,
- license or usage assumption when applicable.

When insertion is in scope, point to the inserted-resource registry and its
runtime evidence. When it is not in scope, omit that section rather than adding
empty requirements.

## Evidence And Build Interface

Include or point to:

- deterministic builder entrypoint and configuration,
- expected-write and execution-receipt formats,
- required static checks,
- evidence records for the declared shareable scope,
- known issue count and documented non-critical limitations.

## Exclusion Checks

Fail package validation when any payload or inventory entry violates its class
rule in `references/strategy/asset-distribution-policy.md`, or when required
provenance and review data are missing.

## Clean-workspace Test

Test in a workspace containing only the package and all expected user-supplied
original build inputs. Record their roles and identities, package identity,
execution receipt, output identity, and checks run. The build must reproduce
the declared target.

Repeat without the execution host and then without each required build source.
Each build must fail closed before using a mismatched or missing input. The
package may still expose its newly authored or generated material, metadata,
and tooling, but it must not reconstruct meaningful original material from an
omitted input. Record whether the negative conditions owned by the policy's
Package Boundary hold; a violation fails this test.
