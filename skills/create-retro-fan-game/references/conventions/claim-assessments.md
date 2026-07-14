# Claim Assessments

A claim assessment is owned by the philosophy or application layer. It declares
what evidence would change a decision, then interprets independently produced
execution, observation, and approval records. It never becomes part of an
observer's output contract.

## Predeclared Claim

Before requesting evidence, record:

- assessment and claim IDs,
- the decision, artifact state, or gate the claim may change,
- relevant game, surface, route, build, and overlay scope,
- success, failure, and ambiguity observables,
- evidence types and sufficiency criteria,
- alternatives that the requested evidence must distinguish.

Unavailable identities remain explicitly pending rather than being fabricated
to satisfy the schema.

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
- artifact states or gates promoted, invalidated, or left open,
- next action for a failed or inconclusive result.

Only a pass that satisfies the predeclared criteria may promote a claim. New
evidence creates a new assessment or supersedes the interpretation record; it
does not mutate the referenced raw observation.
