# Asset-map Fields

An asset map connects semantic asset units to stable host surfaces. It may
describe newly authored work, source adaptation, or a mixture. It does not own
the physical transform.

## Semantic Mapping

Record:

- stable asset-mapping ID,
- zero or more source asset references,
- one or more authored asset-unit IDs,
- semantic relation defined in
  [Separate Semantic And Physical Relations](../strategy/asset-assembly.md#separate-semantic-and-physical-relations),
- meaning and recognizable state that must be retained,
- intentional differences and their rationale,
- continuity-group references,
- required human decisions and unresolved source gaps.

Allow many-to-many mappings. Zero source references are valid for newly
authored units.

## Host-surface Binding

Record:

- stable binding ID,
- one or more asset-unit IDs,
- one or more target host-surface IDs,
- route, state, actor, item, map, cutscene, battle, or interface context,
- intended use or modification of the host surface, by reference to its structure
  record,
- structure-proof and relevant budget references,
- provenance, transform, inserted-resource, observation, and assessment IDs,
- adjacent representations that must remain coherent,
- unresolved host gaps and the claims they block.

The host structure and execution records define the binding's mechanics and
checks. See [Separate Semantic And Physical Relations](../strategy/asset-assembly.md#separate-semantic-and-physical-relations).

Do not include byte writes, conversion settings, copied evidence, or a final
coherence verdict.
