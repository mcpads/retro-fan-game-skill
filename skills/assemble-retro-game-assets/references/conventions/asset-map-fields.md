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
  `references/strategy/asset-assembly.md#separate-semantic-and-physical-relations`,
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
- physical binding intent by reference to the host owner,
- structure-proof and relevant budget references,
- provenance, transform, inserted-resource, observation, and assessment IDs,
- adjacent representations that must remain coherent,
- unresolved host gaps and the claims they block.

Interpret physical binding intent under
`references/strategy/asset-assembly.md#separate-semantic-and-physical-relations`;
its mechanics and pass conditions remain with the host structure and execution
owners.

Do not include byte writes, conversion settings, copied evidence, or a final
coherence verdict.
