# Capability Composition

This document owns responsibility boundaries and capability selection. Creative
policy, execution, and observation must remain independently replaceable even
when one implementation performs all three.

## Responsibilities

| Responsibility | Owns | Record or policy |
| --- | --- | --- |
| Creative authority | Intended experience and material creative tradeoffs | [Intent And Authority](intent-and-authority.md) |
| Execution | Declared transforms and their mechanical checks | [Execution Records](../conventions/execution-records.md) |
| Observation | Raw results, conditions, and collection limits | [Observation Records](../conventions/observation-records.md) |
| Assessment | Interpretation of evidence and claim promotion | [Claim Assessments](../conventions/claim-assessments.md) |

Execution success proves that a declared transform completed. A connection,
command response, or intermediate write does not prove downstream consumption.
Runtime claims need evidence from the real game path, and neither execution nor
observation grants creative approval.

These are logical responsibilities, not mandatory files, services, or agents.
A project record may hold separately addressable sections for a transform,
observation, and assessment, provided the raw evidence remains unchanged when
the interpretation changes. Preserve exact input references across those sections.

## Select Capabilities From The Claim

Declare the decision and the success, failure, and ambiguity observables, then
select an executor and observer capable of distinguishing them. Use the smallest
sufficient combination of local tools, analysis, and human observation. Product
names are provenance, never pass conditions.

When an available tool cannot distinguish the outcomes, investigate another
method or keep the claim open. Do not substitute a weaker technical claim for
the person's requested experience.

## Optional Domain-capability Handoffs

Activate a specialized assessment only for a component that needs it. Narrative
source conformance, cross-surface asset coherence, world reachability, and combat
behavior have different evidence requirements; components need not share one
project-wide mode.

A capability may be supplied by the current agent's evidenced analysis, a
compatible skill, or another tool. No separately installed specialist is required
merely to satisfy a role name. If the available methods cannot assess the actual
property, leave it open and work on its evidence gap or independent components.

Consume references to domain-owned plans, mappings, assessment scope, outcomes,
limits, and dependencies using the
[Capability Handoff Record](../conventions/artifact-states.md#capability-handoff-record).
Do not copy the domain's schema or transfer execution, observation, packaging,
or final creative authority to it.

For a reusable boundary, another observer should be able to challenge the saved
claim and another executor should be able to reproduce the transform without
changing what the evidence means. Expose hidden dependencies when they prevent
that replacement.
