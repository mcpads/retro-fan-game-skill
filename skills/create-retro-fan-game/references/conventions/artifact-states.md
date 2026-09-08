# Creative Artifact States

Track creative approval, build validity, and runtime observation separately.
Group units only when they share scope and evidence; split a group when approval
or validation differs. Use sections of existing project data where practical.

## Composition Scope Record

For the intended playable route, record:

- exact execution-host input identity,
- additional original input identities and their role as `build_source` or
  `evidence_only`,
- stable creative component IDs and open domain labels,
- each component's semantic source relationship and target host-surface IDs,
- dependencies between components,
- approval boundary and completion claims,
- specialized assessment references when required, and current blockers.

Define each component's relationship to its sources under
[Creative Overlay](../strategy/creative-overlay.md#component-graph).

## Capability Handoff Record

For a component that requires specialized domain judgment, record:

- stable handoff and component IDs,
- capability class and the claim it is expected to decide,
- prepared source, plan, mapping, or constraint artifact IDs and exact revisions,
- readiness or conformance assessment IDs,
- outcome read from the referenced assessment: `pass`, `fail`, or
  `inconclusive`,
- assessed scope, limits, unresolved gaps, and blocked dependencies,
- dependencies whose changes require reassessment.

The handoff references the specialized records and reads their assessment outcome;
it must not assign a separate verdict. A missing assessment leaves only the
dependent claims open.

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

Apply [Intent And Authority](../strategy/intent-and-authority.md) to material
creative decisions. Record routine technical methods in execution or research
records. For each material creative decision, record:

- decision ID, class, affected units or revisions, and review scope,
- authority evidence: the explicit request, prior choice, or project decision
  reference, with enough context to preserve its meaning,
- approval owner: `human` or `delegated_agent`,
- the explicit delegation scope when the owner is `delegated_agent`,
- chosen result, unresolved effects, and rationale or alternatives when relevant,
- status: `pending`, `approved`, `rejected`, or `superseded`.

Identify whether approval covers a direction or produced content. Recover missing
records from existing instructions and decisions; do not request approval again
just to fill these fields.

## State Axes

Track production units with these axes when applicable. A provisional sample
does not need build or observation records before anyone can review it.

| Axis | Values | Meaning |
| --- | --- | --- |
| Creative | `provisional`, `draft`, `approved`, `rejected` | Whether the content is authored and approved inside the recorded authority boundary |
| Build | `unbound`, `encoded`, `statically_valid`, `failed` | Whether it is represented by the target format and passes applicable deterministic checks |
| Observation | `unobserved`, `pass`, `fail`, `inconclusive` | Whether the declared runtime claim has sufficient evidence |
| Issue | `open`, `clear` | Whether a known issue still blocks the unit's declared route |

A production unit is complete when approved for its review scope, statically
valid, supported by an applicable runtime pass, and free of blocking issues.
Tie states to exact content and build identities. Read the observation status
from its assessment and reset outdated statuses under
[Project State](project-state.md#invalidation). Product completion follows
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
