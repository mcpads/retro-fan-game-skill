# Claim Assessments

An assessment decides whether evidence supports a claim under
[Capability Composition](../strategy/composition.md). Record consequential
decisions in existing project data; routine tool calls need no separate assessment.

## Predeclared Claim

Before requesting evidence, record:

- assessment and claim IDs,
- the decision, artifact state, or gate the claim may change,
- relevant game, surface, route, build, and overlay scope with exact input
  revisions or hashes when the claim depends on content,
- observations that distinguish success, failure, and uncertainty,
- evidence types and sufficiency criteria,
- alternatives that the requested evidence must distinguish.

Mark unavailable identities as pending. Reuse saved evidence when it meets the
current criteria; collect more if it cannot distinguish the alternatives. If
criteria were defined after collection, record that timing accurately.

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

Only a current pass for the selected inputs can support completion or the next
gate. Reassess new evidence while retaining prior outcomes and raw observations.
Apply [Project State](project-state.md#invalidation) to outdated or conflicting
assessments.
