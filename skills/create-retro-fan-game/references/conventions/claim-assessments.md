# Claim Assessments

A claim assessment interprets evidence for a decision under the responsibility
boundaries in [Capability Composition](../strategy/composition.md). A short
section in an existing record can suffice; create assessments for consequential
claims and promotion decisions, not for every routine tool call.

## Predeclared Claim

Before requesting evidence, record:

- assessment and claim IDs,
- the decision, artifact state, or gate the claim may change,
- relevant game, surface, route, build, and overlay scope with exact input
  revisions or hashes when the claim depends on content,
- success, failure, and ambiguity observables,
- evidence types and sufficiency criteria,
- alternatives that the requested evidence must distinguish.

Unavailable identities remain explicitly pending rather than being fabricated
to satisfy the schema.
Existing evidence may be reused after checking its relevance to these criteria.
Do not describe criteria devised after collection as having guided that earlier
collection; obtain additional evidence if the saved result cannot distinguish
the current alternatives.

## Evidence References

Reference independently identified inputs as applicable:

- human approval records,
- structure facts and their provenance,
- execution receipts and static checks,
- raw observation IDs,
- unresolved gaps or conflicting evidence.

Do not copy or rewrite raw evidence into the assessment.

## Interpretation And Promotion

After evidence collection, record:

- outcome: `pass`, `fail`, or `inconclusive`,
- interpretation connecting the referenced evidence to the claim,
- competing explanations ruled out or still open,
- evidence, observer, route, and scope limitations,
- dependency references and applicability: `current`, `invalidated`, or
  `superseded`, with reason and replacement reference when applicable,
- artifact states or gates promoted, invalidated, or left open,
- next action for a failed or inconclusive result.

Only a current pass that satisfies the declared criteria for the selected inputs
may promote a claim. New evidence creates a new assessment; retain the earlier
outcome and mark its applicability under
[Project State](project-state.md#invalidation). Do not rewrite raw observations
or select an older pass while relevant conflicting evidence remains unresolved.
