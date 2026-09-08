# Optional Patch Package

Open this branch only when the person requests sharing or the project has
already declared it in scope. Packaging is not required for personal completion.

## Package Claim

Let another person reproduce the target from their verified host game and any
required source games. Apply [Asset Distribution Policy](asset-distribution-policy.md)
to package contents and [Package Manifest](../conventions/package-manifest.md)
to inventory and reconstruction checks.

## Shareable Surface

Inventory candidate files by asset class, provenance, and dependencies. Include
only what the policy permits, with the evidence and limits the manifest requires.

## Safety Dependencies

- Enforce the execution-host and every required build-source identity before
  transformation.
- Apply the execution contract and fail on source mismatch, unexplained writes,
  missing dependencies, or invalid final identity.
- Include inserted-resource data only when its registry and runtime evidence are
  complete for the declared package scope.
- Pass the manifest's clean-workspace verification before declaring a shareable candidate.

Use [Execution Records](../conventions/execution-records.md) for writes and receipts,
and [Workflow Gates](workflow-gates.md) for candidate criteria.
