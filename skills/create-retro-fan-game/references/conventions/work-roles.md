# Work Roles

Classify technical work by its inputs and the claim its result supports. Map these
roles to existing project commands and records; separate directories, executables,
or agents are not required. Qualify tooling builds and product builds when the
word "build" could refer to either.

## Responsibilities

| Role | Purpose and result | Limit of a successful result |
| --- | --- | --- |
| Tooling build | Compile or package an analyzer, patcher, verifier, or supporting code | The tooling was produced; no claim about current game inputs or output follows |
| Analysis | Resolve uncertainty about game structure, behavior, or an implementation method; retain scoped findings and evidence | Findings require explicit adoption before they govern product construction |
| Product build | Construct an exact game output from the selected originals, content, configuration, and adopted transforms | Construction alone proves neither static validity nor runtime behavior |
| Test | Exercise an implementation's stable behavior or a reproduced defect with controlled inputs | The result covers that case, not the current selected game image |
| Artifact verification | Check an exact source or output against its applicable format, input conditions, write plan, and structural constraints | Static validity does not establish game consumption |
| Runtime verification | Observe the game consuming an identified image on a declared route, state, and environment | Evidence covers that behavior and scope; it does not grant creative approval |

A command may perform several roles. Preserve their separate results: compilation
success cannot stand in for a product build, and a test runner can invoke analysis
or verify a current image without changing the meaning of that evidence. A
hypothesis-discriminating run is an investigation experiment, even when automated.
Runtime automation remains runtime verification.

## Tests And Current Artifact Checks

Tests protect stable interfaces, format rules, deterministic invariants, or
reproduced failures. Use controlled fixtures that distinguish correct behavior
from a relevant defect. An integration test may construct a fixture image and
exercise its verifier; it does not replace construction and verification of the
selected playable. A test that merely finds a checker or confirms it ran adds no
evidence about whether the checker accepts valid input and rejects invalid input.

Derive counts, addresses, sizes, and checksums from current product inputs. Do not
freeze such results as test expectations when valid content edits should change
them. Exact fixture values are useful when the fixture or reproduced failure fixes
them; exact values for a supported original or selected output belong to artifact
verification with that identity and scope.

The [Product Build Path](execution-records.md#product-build-path) must reject
invalid current inputs and structurally invalid outputs. Tests exercise those
checks with controlled cases; a passing test suite cannot waive them.
Source-dependent checks that could not run must remain explicitly not run.
Continue tool or fixture work that needs no original, without reporting the
product build or verification as complete.

## Evidence And Handoff

Use [Technical Investigation](../strategy/technical-investigation.md) for unknown
structure, [Execution Records](execution-records.md) for declared runs and outputs,
and [Runtime Observation](../strategy/runtime-observation.md) for game evidence.
[Claim Assessments](claim-assessments.md) interprets results within their scope.
Keep each role's input dependencies explicit rather than making every command
require a ROM or treating every successful command as a verified playable.
