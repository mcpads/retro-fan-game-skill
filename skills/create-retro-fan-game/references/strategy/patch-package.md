# Optional Patch Package

Open this branch only when the person requests sharing or the project has
already declared a shareable scope. Packaging is not required to create,
complete, or consume a private fan game.

## Package Claim

Let another owner reproduce the declared local target from their verified
execution host and any additional required build-source originals. Apply the
classifications and negative boundary owned by
`references/strategy/asset-distribution-policy.md`; do not redefine that
boundary in the packaging branch. Use
`references/conventions/package-manifest.md` for concrete inventory and
clean-workspace requirements.

## Shareable Surface

Inventory each candidate artifact under the distribution policy. Include only
the transforms, metadata, new work, evidence, and limitations permitted by its
classification, with the provenance and dependencies required by the manifest.

## Safety Dependencies

- Enforce the execution-host and every required build-source identity before
  transformation.
- Apply the execution contract and fail on source mismatch, unexplained writes,
  missing dependencies, or invalid final identity.
- Include inserted-resource data only when its registry and runtime evidence are
  complete for the declared package scope.
- Pass the clean-workspace test owned by
  `references/conventions/package-manifest.md` before promoting a shareable
  candidate.

Expected writes and execution receipts are owned by
`references/conventions/execution-records.md`; exact candidate criteria are
owned by `references/strategy/workflow-gates.md`.
