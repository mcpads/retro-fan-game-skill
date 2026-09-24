# Creative Artifact States

Record creative units through the play segments that consume them. Keep these
records in existing project data; group units that share scope and evidence.

## Composition Scope Record

For the intended route, record the
[execution host](structure-map-fields.md#base-identity)'s identity, other
originals and their [role](execution-records.md#input-scope), stable component
IDs, each component's source relationship and target surfaces, dependencies, and the
approval boundary. Current status belongs to the
[current entry](project-state.md), so this record holds decisions only.

## Capability Handoff Record

When a component needs specialized judgment, record the claim it decides, the
exact plan or mapping revisions handed over, the referenced assessment and its
outcome (`pass`, `fail`, `inconclusive`), its scope and gaps, and what would
require reassessment. The handoff reads the outcome; it assigns no verdict.

## Creative Brief Record

Give the author what the current unit needs: its segment and purpose, approved
premise and character state, voice and naming constraints, required runtime
elements such as flags, portraits, or cues, proven budgets, contradictions to
avoid, and open creative or structure questions, labeled as open.

## Approval Record

For each material creative decision, record the affected units, the authority
(the person's request, prior choice, or explicit delegation and its scope), the
chosen result, and status: `pending`, `approved`, `rejected`, or `superseded`.
For produced content, record the accepted file's content hash with the person's
words. Record the agent's interpretation of those words as a proposal until the
person confirms it. Recover earlier approvals from existing instructions and
decisions rather than asking again.

## State Axes

Track production units on four separate axes; a provisional sample can be
reviewed before it has build or observation states:

| Axis | Values |
| --- | --- |
| Creative | `provisional`, `draft`, `approved`, `rejected` |
| Build | `unbound`, `encoded`, `statically_valid`, `failed` |
| Observation | `unobserved`, `pass`, `fail`, `inconclusive` |
| Issue | `open`, `clear` |

A unit is complete when approved, statically valid, observed passing in its
segment on the selected build, and clear of blocking issues. Tie states to exact
content and build identities, and reset them under
[Invalidation](project-state.md#invalidation).

## Placeholders

A placeholder stands in for intended content so connection and progression can
be built and observed early. Record what it replaces and the intended final
content. Its creative state stays provisional until it is replaced or the person
accepts it as final. Report open placeholders with the route status.

## Authored Or Generated Asset Provenance

For a new asset, record its source class, author or generator, prompt or source
note, the origin of each reference under
[Reference Identity](../strategy/creative-review.md#reference-identity), rights
assumption, source and converted hashes, conversion settings, target surface,
and its four state axes. Generation bundles contain authored material only.
