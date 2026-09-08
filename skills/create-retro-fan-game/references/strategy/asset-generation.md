# Asset Generation

Generated and newly authored assets are candidate creative inputs, not proof of
engine compatibility. Use them only inside a declared overlay and preserve
their origin separately from extracted original material.

## Decision Rules

- Classify the target surface and its proven runtime constraints before binding
  an asset to production. Provisional creative samples may precede that proof;
  bounded format experiments follow [Workflow Gates](workflow-gates.md#experimental-work).
- Generate or author outside the immutable extraction tree.
- When several assets must express one entity, place, item, state, or cue across
  multiple surfaces, require a semantic asset handoff rather than inferring
  coherence from matching files or prompts.
- Convert deterministically to the target format and validate every measured
  budget before insertion or replacement.
- If no existing slot can express the asset safely, evaluate
  [Resource Insertion](resource-insertion.md) rather than assuming storage alone
  makes insertion possible.
- Observe the asset through the actual game-consumption path before promoting a
  runtime claim.

Use [Creative Artifact States](../conventions/artifact-states.md) for provenance and state fields,
and [Asset Distribution Policy](asset-distribution-policy.md) for shareability
classification.

## External-service Boundary

Do not send original game images or extracted original assets to an external
generator. Provide only the minimum creative brief and independently described
constraints needed for the candidate asset. A generated result must not be used
to infer unmeasured engine limits.

## Hard Stops

- Reject assets that look plausible but fail binary, palette, tile, memory,
  timing, audio, compression, or route-state constraints.
- Do not silently treat generated resemblance as permission to redistribute an
  original or derived asset.
- Promote asset states only under
  [Creative Artifact States](../conventions/artifact-states.md#state-axes).
- Do not let this generation path decide cross-surface identity, source
  conformance, map behavior, combat behavior, or narrative meaning.
