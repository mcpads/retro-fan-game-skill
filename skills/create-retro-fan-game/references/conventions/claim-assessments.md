# Claim Assessments

An assessment decides whether evidence supports a claim that changes a
decision, state, or gate.

## Predeclared Claim

Before collecting evidence, record the claim, the decision it may change, its
segment, build, and input scope, and the observations that would distinguish
success, failure, and uncertainty. If criteria were set after collection, say so.

## Evidence From Another Build

An observation belongs to the build it observed. To apply it to another build,
record a scoped assessment showing that the output differences leave the claim's
runtime path, shared code, data, layout, and observation conditions unchanged.
An unchanged source file is insufficient on its own, since repacking or a shared
loader change can alter behavior. When the comparison is incomplete, observe the
selected build. A passing reuse covers that claim only; route coverage still
comes from play on the selected build.

## Interpretation And Promotion

After collection, record the outcome (`pass`, `fail`, `inconclusive`), how the
referenced evidence supports it, explanations ruled out or still open, limits,
applicability (`current`, `invalidated`, `superseded`), the states or gates it
changes, and the next action after a failure. Reference raw evidence by ID and
leave it unchanged. Completion and the next gate rest on current passes for the
selected inputs.
