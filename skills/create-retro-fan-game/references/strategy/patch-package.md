# Optional Patch Package

Open this branch when the person asks to share the work or the project already
includes sharing.

## Package Claim

Another person reproduces the target from their verified host game and required
source games. Contents follow
[Asset Distribution Policy](asset-distribution-policy.md); inventory and
reconstruction checks follow [Package Manifest](../conventions/package-manifest.md).

## Safety Dependencies

- Check the execution host and every required build source before transforming.
- Stop on source mismatch, unexplained writes, missing dependencies, or a wrong
  final identity, using [Execution Records](../conventions/execution-records.md).
- Include inserted-resource data once its record and runtime evidence cover
  the package scope.
- Pass clean-workspace verification before declaring a candidate under
  [Workflow Gates](workflow-gates.md#shareable-candidate-gate).
