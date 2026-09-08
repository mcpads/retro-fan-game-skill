# Asset-ledger Fields

Reuse an existing asset catalog that records these meanings.
Keep semantic IDs stable across file renames, conversions, sheet repacking, and
host relocation.

## Asset Unit

Record:

- stable asset-unit ID,
- open profile and semantic role,
- represented entity, place, item, state, action, cue, or interface meaning,
- intended route and creative component,
- source relationship: preserved, adapted, remixed, substituted, or newly
  authored,
- source or authored provenance references,
- relevant source locators when adaptation is claimed,
- required variants, views, poses, expressions, states, or cues,
- continuity-group and related asset-unit IDs,
- narrative, world, system, or interface requirement references,
- approval references and unresolved semantic gaps.

Do not store original game images or extracted assets in the ledger. Refer to
their locally owned identities and provenance records.

## Variant Or Continuity Group

Record:

- stable group ID and shared semantic identity,
- member asset-unit IDs,
- required cross-surface or state relationships,
- allowed intentional differences,
- coverage expectations for the intended route,
- human approval references and unresolved conflicts.

The group may connect a character's field sprite, battle representation,
portrait, cutscene frames, and UI icon without assuming they share a physical
format.

Reference structure, execution, and observation records for format budgets,
conversion, loading, and runtime results instead of copying those fields.
