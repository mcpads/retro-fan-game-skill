# Creative Artifact States

Creative approval, build validity, and runtime observation are separate axes.
Do not collapse them into one optimistic progress label.
Use the smallest unit or coherent group that shares the same scope and evidence;
split it when approval or validation differs. These records may be sections of
existing project data rather than separate files.

## Composition Scope Record

For the intended playable route, record:

- exact execution-host input identity,
- additional original input identities and their role as `build_source` or
  `evidence_only`,
- stable creative component IDs and open domain labels,
- each component's semantic source relationship and target host-surface IDs,
- dependencies between components,
- approval boundary and completion claims,
- required optional capability handoffs and current blockers.

Do not force one source relation or creative mode on the entire project. A
component may be original, adapted, preserved, divergent, synthesized,
restored, generated, or another explicitly defined relation.

## Capability Handoff Record

For a component that requires specialized domain judgment, record:

- stable handoff and component IDs,
- capability class and the claim it is expected to decide,
- prepared source, plan, mapping, or constraint artifact IDs and exact revisions,
- readiness or conformance assessment IDs,
- outcome projected from the referenced assessment: `pass`, `fail`, or
  `inconclusive`,
- assessed scope, limits, unresolved gaps, and blocked dependencies,
- invalidation references that require reassessment when they change.

The handoff points to domain-owned artifacts; it does not copy their schemas or
evidence, and its outcome is not a second verdict owner. A missing applicable
handoff keeps the specialized claim open but does not block unrelated
components.

## Creative Brief Record

For each bounded unit or group of units, record:

- stable unit and target surface IDs,
- intended route and creative purpose,
- references to premise decisions and relevant character, relationship, or world
  state, distinguishing approved intent from provisional choices,
- glossary, naming, voice, and continuity constraints,
- required flags, branches, portraits, cues, or other runtime elements,
- references to proven structure budgets,
- forbidden contradictions and out-of-scope changes,
- unresolved creative questions and unresolved structure gaps.

The brief may exist provisionally before the surface is build-ready. Label
unknowns; do not convert them into invented facts.

## Approval Record

Record material creative decisions under
[Intent And Authority](../strategy/intent-and-authority.md). Routine technical
methods belong in execution or research records, not an approval queue.
For each applicable decision, record:

- decision ID, class, affected units or revisions, and review scope,
- authority evidence: the explicit request, prior choice, or project decision
  reference, with enough context to preserve its meaning,
- approval owner: `human` or `delegated_agent`,
- the explicit delegation scope when the owner is `delegated_agent`,
- chosen result, unresolved effects, and rationale or alternatives when relevant,
- status: `pending`, `approved`, `rejected`, or `superseded`.

Distinguish direction approval from review of produced content. Reconstruct
missing records from existing authority evidence using the policy above; do not
fabricate decisions or introduce another approval step to populate these fields.

## State Axes

Track production units with these axes when applicable. A provisional sample
does not need build or observation records before anyone can review it.

| Axis | Values | Meaning |
| --- | --- | --- |
| Creative | `provisional`, `draft`, `approved`, `rejected` | Whether the content is authored and approved inside the recorded authority boundary |
| Build | `unbound`, `encoded`, `statically_valid`, `failed` | Whether it is represented by the target format and passes applicable deterministic checks |
| Observation | `unobserved`, `pass`, `fail`, `inconclusive` | Whether the declared runtime claim has sufficient evidence |
| Issue | `open`, `clear` | Whether a known issue still blocks the unit's declared route |

A production unit is complete when its creative state is approved for the review
scope, its build is statically valid, an applicable passing assessment supports
the runtime claim, and blocking issues are clear. States apply to referenced content
and build identities. The observation axis projects the assessment's outcome;
it is not a second verdict. Clear affected pass projections under
[Project State](project-state.md#invalidation) when their dependencies change.
Product-level completion remains owned by
[Workflow Gates](../strategy/workflow-gates.md).

## Authored Or Generated Asset Provenance

When an asset is newly authored or generated, record:

- source class and human source note or generation prompt reference,
- author, generator capability, or model identity when relevant,
- rights or usage assumption,
- source and converted artifact hashes,
- conversion transform and configuration references,
- target surface and conditional inserted-resource IDs,
- semantic asset-unit, mapping, or capability-handoff IDs when the asset belongs
  to a multi-surface component,
- the four state axes and their evidence references.

Do not place original game images or extracted original assets in a generation
provenance bundle.
