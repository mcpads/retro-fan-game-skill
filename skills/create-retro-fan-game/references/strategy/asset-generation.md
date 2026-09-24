# Asset Generation

Generated and newly authored assets are candidates for a segment. Keep their
origin separate from extracted original material.

## Before Making

- Establish what the surface tells the player and what drives it. A face may be
  a health indicator rather than an expressive portrait; count the states the
  surface shows in play.
- For a replaced animation, record what each original frame shows: facing,
  hidden parts, gaze, hand action, and the move it depicts. Generators drift
  toward front-facing, readable poses, so check candidates against this record.
- Identify an original asset through the code or event that selects it. Look for
  existing original assets that fit the surface before generating.
- Record each reference's origin under
  [Reference Identity](creative-review.md#reference-identity).
- Provisional samples may come before the surface's constraints are proven;
  format experiments follow [Workflow Gates](workflow-gates.md#experimental-work).

## Making And Binding

- Author outside the immutable extraction tree.
- Cross-surface identity, source conformance, map or combat behavior, and
  narrative meaning are decided through their
  [domain handoffs](composition.md#optional-domain-capability-handoffs), such as
  asset coherence when several assets express one entity, place, item, state,
  or cue.
- Convert deterministically and validate every measured budget, including
  engine state the asset shares: palettes, video memory, cursor or font tiles,
  and duplicated tables that restore or redraw it.
- When no existing slot can hold the asset, evaluate
  [Resource Insertion](resource-insertion.md).
- Present candidates under [Creative Review](creative-review.md), and observe
  the adopted asset through the game's consumption path in its segment.

Record provenance and states in
[Creative Artifact States](../conventions/artifact-states.md), and sharing class
under [Asset Distribution Policy](asset-distribution-policy.md).

## External Generators

Send an external generator only the creative brief and independently described
constraints; original images and extracted assets stay local. Engine limits
come from measurement.
