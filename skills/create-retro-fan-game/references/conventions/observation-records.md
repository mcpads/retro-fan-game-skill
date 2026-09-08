# Observation Records

An observation record is observer-produced raw evidence. It reports what was
collected and under which conditions. Responsibility boundaries are owned by
[Capability Composition](../strategy/composition.md#responsibilities).

## Observation Request Reference

Record:

- observation ID and the referenced claim or assessment ID,
- required observable and capability description supplied by the requester,
- game or base identity and the runtime identity available for the request,
- original input, build receipt, structure-map, and overlay identities when the
  requested observable depends on those artifacts,
- the loaded output's identity and starting save or runtime state when relevant,
- declared preconditions, route or procedure, inputs, and relevant timing,
- known observer blind spots at selection time.

The observer product or tool name may be retained as provenance, but it is never
a substitute for the capability description.

## Raw Result

Preserve:

- capture, trace, state, memory, audio, log, or human-observation artifact,
- artifact identity, hash when practical, and collection provenance,
- actual route or procedure, inputs, timing, and deviations from the request,
- whether the result is deterministic, replayable, or human-only,
- collection failures, missing observables, and newly discovered limits.

Keep project verdicts in assessments, not raw observations. Preserve raw results
and the actual observed build identity when conclusions or selected builds change.
Retain any tool-supplied verdict as part of its original response; the project's
assessment must decide whether it supports the claim.
