# Work Roles

Classify technical work by the claim its result supports. Map these roles to
existing commands; one command may perform several.

## Responsibilities

| Role | Result | Supports |
| --- | --- | --- |
| Tooling build | An analyzer, patcher, or verifier was produced | The tooling exists |
| Analysis | Scoped findings about structure, behavior, or method | Product use after explicit adoption |
| Product build | An exact game output from selected inputs | Existence of that output only |
| Test | Stable behavior or a reproduced defect under controlled inputs | That case |
| Artifact verification | An exact output checked against format, inputs, and write plan | Static validity |
| Runtime verification | The game consuming an identified image on a declared route | That behavior and scope; creative approval stays with the person |

Each role's claim comes from its own result; a test runner that checks the
current image is doing artifact or runtime verification.

## Tests And Current Artifact Checks

Tests protect stable interfaces, format rules, invariants, and reproduced
failures, using fixtures that separate correct behavior from the defect. Derive
counts, addresses, sizes, and checksums of the selected output from current
inputs in artifact verification; fixed values in tests come from fixtures. A
checker is tested by feeding it valid and invalid cases. When a check needs an
original that is unavailable, report it as not run and continue work that needs
no original.
