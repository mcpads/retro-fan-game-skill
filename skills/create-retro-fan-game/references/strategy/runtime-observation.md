# Runtime Observation

Runtime observation shows what the game actually consumed, displayed, played, or
did in a segment. Define the observable from the claim, then choose a manual,
interactive, or automated observer that can produce it under
[Capability Composition](composition.md).

## Evidence Selection

- Static and execution evidence covers encoding, budgets, deterministic
  transforms, and expected writes.
- The real game path covers visibility, state, timing, audio, route, save/load,
  and playability.
- Aesthetic and semantic judgments belong to the person under
  [Creative Review](creative-review.md), shown on a preserved route.
- A successful connection or command covers connectivity or command execution.

Record collection in [Observation Records](../conventions/observation-records.md)
and interpretation in [Claim Assessments](../conventions/claim-assessments.md),
and check the loaded output against its build receipt.

## Coverage Judgment

Observe each changed surface in its segment, inserted resources through their
loader, relevant save/load and story-state transitions, and an adjacent unchanged
path where shared tables, archives, caches, or engine logic could regress. Units
on one proven consumer path, such as lines in one dialogue table, may share a
representative observation plus static checks of every unit; units with a
different path, state, or presentation get their own. Screenshots show visible
output and traces show hidden state; choose what the claim needs.

## Observation Limits

- Judge visuals from frames captured after the display settles, and record the
  frame timing.
- Record the channels the observer watched; findings cover those channels, and
  a check that exercised zero cases has not run.
- Record every intervention, such as memory writes, teleports, forced
  encounters, debug patches, or state restores, and what it leaves unproven.
  Keep debug patches in throwaway copies and the natural-path claim open.
- Before relying on repeated emulator state restores, show that a restore
  reproduces the baseline, and suspect the tool when behavior turns odd after
  restores. Record a starting state taken from another build as such, with what
  it leaves unestablished for the selected build. Prove persistence with the
  game's own save and a power cycle, and reproduce runs as input replays from a
  new game.

## Issue Loop

1. Reproduce from the declared inputs and starting state.
2. Compare the same view or state on the unmodified build, and find the last
   passing gate for the affected surface.
3. Separate structure, content, execution, runtime-state, and observation
   explanations.
4. Fix the smallest confirmed cause.
5. Add the failed claim to repeatable coverage when feasible.

Keep evidence that rules out a suspected cause. For a costly failure, record the
symptom, trigger, misleading evidence, cause, and corrective check in the
project's issue record, and keep the fix selected in the
[current entry](../conventions/project-state.md).
