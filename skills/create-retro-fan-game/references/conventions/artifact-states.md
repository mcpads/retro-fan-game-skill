# Creative Artifact States

Creative approval, build validity, and runtime observation are separate axes.
Do not collapse them into one optimistic progress label.

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
- prepared source, plan, mapping, or constraint artifact IDs,
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
- approved premise and relevant character, relationship, or world state,
- glossary, naming, voice, and continuity constraints,
- required flags, branches, portraits, cues, or other runtime elements,
- references to proven structure budgets,
- forbidden contradictions and out-of-scope changes,
- unresolved creative questions and unresolved structure gaps.

The brief may exist provisionally before the surface is build-ready. Label
unknowns; do not convert them into invented facts.

## Approval Record

For each material decision, record:

- decision ID, class, affected units, and options considered,
- approval owner: `human` or `delegated_agent`,
- the explicit delegation scope when the owner is `delegated_agent`,
- chosen option, rationale, and unresolved effects,
- status: `pending`, `approved`, `rejected`, or `superseded`.

Premise, character, meaning, canon, tone, and acceptable-risk decisions use the
person as approval owner. Lower-impact decision classes may use a delegated
agent only inside an explicitly recorded scope. A missing approval record is not
implicit consent.

## State Axes

Track each unit with all of these axes:

| Axis | Values | Meaning |
| --- | --- | --- |
| Creative | `provisional`, `draft`, `approved`, `rejected` | Whether the content is authored and approved inside the recorded authority boundary |
| Build | `unbound`, `encoded`, `statically_valid`, `failed` | Whether it is represented by the target format and passes applicable deterministic checks |
| Observation | `unobserved`, `pass`, `fail`, `inconclusive` | Whether the declared runtime claim has sufficient evidence |
| Issue | `open`, `clear` | Whether a known issue still blocks the unit's declared route |

A unit may be called complete only when its required creative state is approved,
build state is statically valid, the latest applicable claim assessment promotes
an observation pass, and blocking issues are clear. The observation axis is a
projection of that assessment, not a verdict emitted by the observer.
Product-level private and sharing completion remains owned by
`references/strategy/workflow-gates.md`.

## Authored Or Generated Asset Provenance

When an asset is newly authored or generated, record:

- source class and human source note or generation prompt reference,
- author, generator capability, or model identity when relevant,
- rights or usage assumption,
- source and converted artifact hashes,
- deterministic conversion settings,
- target surface and conditional inserted-resource IDs,
- semantic asset-unit, mapping, or capability-handoff IDs when the asset belongs
  to a multi-surface component,
- the four state axes and their evidence references.

Do not place original game images or extracted original assets in a generation
provenance bundle.
