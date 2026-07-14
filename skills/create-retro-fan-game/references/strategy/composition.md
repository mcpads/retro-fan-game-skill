# Capability Composition

Philosophy, execution, and observation answer different questions. Keep their
contracts separable even when one local implementation provides more than one
capability.

## Claim-first Judgment

1. State the claim that would change the next decision.
2. Decide whether it requires creative approval, execution evidence, runtime
   observation, or a composition of them.
3. Declare the success, failure, and ambiguity observables before acting.
4. Select the smallest capable executor and observer independently.
5. Preserve raw results separately from the interpretation and gate decision.

If the available capability cannot distinguish the outcomes, narrow the claim
or choose a stronger capability. Its product name never becomes part of the
pass condition.

## Cross-boundary Rules

- Do not infer creative approval from a successful transform or observation.
- Do not infer runtime consumption from a build receipt or intermediate write.
- Keep observer output limited to raw results, conditions, provenance, and
  collection limits.
- Interpret evidence and promote gates in a separate claim assessment.

Execution success proves only that the declared transformation completed. A
connection, command response, or changed intermediate buffer proves only the
claim it directly observes. Visibility, state, and playability claims require
evidence from the real game-consumption path.

Use `references/conventions/execution-records.md` for transform records,
`references/conventions/observation-records.md` for raw observer output, and
`references/conventions/claim-assessments.md` for interpretation and gate
promotion.

## Optional Domain-capability Handoffs

For each bounded component, activate only the domain capability needed to
decide its specialized meaning or readiness. Different components may use
different capabilities or no specialized capability at all.

The core handoff consumes stable prepared-artifact IDs, assessment outcome and
scope, limits, blocked dependencies, and invalidation references. It does not
copy the domain records or prescribe the product that produced them. A domain
capability may define narrative conformance, asset coherence, behavior
equivalence, reachability, or procedural solvability, but it does not inherit
execution, observation, packaging, or final creative authority.

Use `references/conventions/artifact-states.md` for the generic component scope
and handoff record. Leave a specialized claim open when no compatible
capability can assess it.

## Creative Authority

Record the person's approval boundary before high-impact content work. Choices
that materially affect premise, character, meaning, canon, tone, or acceptable
risk return to the person. Lower-impact choices may be delegated, but only
inside the recorded scope; delegation is not blanket authorship transfer.

## Replacement Check

Before promoting a reusable conclusion, ask:

- Could another compatible observer challenge the claim from the saved record?
- Could another executor reproduce the transform without changing what the
  runtime evidence means?
- Could the creative policy change without modifying either implementation?

If not, expose and separate the hidden dependency.
