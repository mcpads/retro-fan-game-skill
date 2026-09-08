# Capability Composition

Choose tools and assign responsibilities so creative policy, execution, and
observation remain replaceable, even within one implementation.

## Responsibilities

| Responsibility | Decides or records | Reference |
| --- | --- | --- |
| Creative authority | Intended experience and material creative tradeoffs | [Intent And Authority](intent-and-authority.md) |
| Execution | Declared transforms and their mechanical checks | [Execution Records](../conventions/execution-records.md) |
| Observation | Raw results, conditions, and collection limits | [Observation Records](../conventions/observation-records.md) |
| Assessment | Whether the evidence satisfies a claim | [Claim Assessments](../conventions/claim-assessments.md) |

Execution success establishes that a transform completed. Runtime claims need
evidence that the game actually used its result; neither proves creative approval.

One record may contain separately referenced sections for a transform,
observation, and assessment. Preserve exact input references and keep raw evidence
unchanged when the interpretation changes.

## Select Capabilities From The Claim

Define the decision and the observations that distinguish success, failure, and
uncertainty. Choose tools, analysis, or human observation that can make those
distinctions. Record tool names for traceability, not as pass conditions.

When an available tool cannot distinguish the outcomes, investigate another
method or keep the claim open. Do not substitute a weaker technical claim for
the person's requested experience.

## Optional Domain-capability Handoffs

Activate a specialized assessment only for a component that needs it. Narrative
source conformance, cross-surface asset coherence, world reachability, and combat
behavior have different evidence requirements; components need not share one
project-wide mode.

The current agent may perform the specialized analysis using evidence, a
compatible skill, or another tool. A separate specialist is not required. If no
available method can assess the property, investigate the gap or continue
independent work while leaving the claim open.

Reference specialized plans, mappings, assessment scope, outcomes,
limits, and dependencies using the
[Capability Handoff Record](../conventions/artifact-states.md#capability-handoff-record).
Do not copy the domain's schema or transfer execution, observation, packaging,
or final creative authority to it.

For a reusable boundary, another observer should be able to challenge the saved
claim and another executor should be able to reproduce the transform without
changing what the evidence means. Expose hidden dependencies when they prevent
that replacement.
