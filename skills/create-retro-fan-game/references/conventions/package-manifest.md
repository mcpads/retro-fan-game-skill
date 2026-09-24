# Package Manifest

Create this manifest when sharing is in scope. It tells another owner of the
required originals how to reproduce the declared target.

## Required Identity

Record the package and overlay scope, the execution host and every required
build source with accepted sizes and hashes, the builder and structure
identities, the output identity policy, and known limits. Evidence-only sources
are listed without becoming build requirements.

## Included Artifact Inventory

For each included file, record its hash, purpose, class under
[Asset Distribution Policy](../strategy/asset-distribution-policy.md),
provenance or local-transform relationship, build step, and license assumption.
For previews, also record the source observation, supported claim, retained
original context, and the review of all exports together under
[Preview Evidence](../strategy/asset-distribution-policy.md#preview-evidence).
Point to the [inserted-resource record](structure-map-fields.md#conditional-inserted-resource-record)
when the package inserts resources.

## Clean-workspace Verification

Rebuild in a workspace holding only the package and the expected originals, and
record the receipt and output identity; it must reproduce the declared target.
Then remove the host and each required build source in turn; each build must
stop before using a missing or mismatched input. Validation fails on any
content that violates the distribution policy or lacks its provenance record.
