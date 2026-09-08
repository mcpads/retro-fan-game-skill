# Runtime Observation

Runtime observation answers claims about what the game actually consumed,
displayed, played, or did. Define the observable from the claim and then choose
any manual, interactive, automated, or combined observer capable of producing
sufficient evidence under [Capability Composition](composition.md).

## Evidence Selection

- Use static and execution evidence for claims about encoding, budgets,
  deterministic transforms, or expected writes.
- Use the real game-consumption path for visibility, state, timing, audio,
  route, save/load, and playability claims.
- Use human observation for aesthetic or semantic judgments that cannot be
  reduced to a deterministic predicate, while preserving the route and result.
- A successful connection or command is sufficient only when connectivity or
  command execution is the declared claim.

Use [Observation Records](../conventions/observation-records.md) for collection
and [Claim Assessments](../conventions/claim-assessments.md) for interpretation.
Check the loaded game against the selected build receipt before using a capture
as evidence for current completion. Saved evidence can be reused when its input
identities, route, and claim remain applicable.

## Coverage Judgment

Observe each changed surface on the intended route, any inserted resource
through its loader path, relevant save/load or story-state transitions, and an
adjacent unchanged path when shared tables, archives, caches, or engine logic
could regress. Select traces or memory measurements only when the claim needs
them; screenshots alone do not prove hidden state, and traces alone do not prove
human-visible output.

## Issue Loop

1. Reproduce from the declared local inputs and starting state.
2. Identify the affected surface and last passing dependency gate.
3. Separate structure, content, execution, runtime-state, and observation
   explanations.
4. Fix the smallest confirmed cause.
5. Add the failed claim to repeatable coverage when feasible.

Preserve failed hypotheses when they eliminate a layer. Do not promote a
workaround until its safety is supported well enough for the affected claim.

For a costly failure worth reusing, preserve the symptom, triggering input and
scope, misleading evidence, confirmed cause, corrective check, and proof limits
in the project's existing case or issue record. Keep the current fix selected
through [Project State](../conventions/project-state.md). Retain cases that change
a future decision; do not turn one game's measurements into universal rules.

## Completion Role

Observation is one input to completion, not its owner. Exact private-playable
and shareable-candidate criteria belong to
[Workflow Gates](workflow-gates.md).
