# Structure-map Readiness

A structure map connects reverse engineering to the surfaces and dependencies
the intended overlay needs. It need not describe the whole game. Concrete
fields belong to [Structure-map Fields](../conventions/structure-map-fields.md).
Use [Technical Investigation](technical-investigation.md) to establish missing
facts, including when no structure map exists yet.

## Evidence Distinctions

| Evidence | What it supports |
| --- | --- |
| Hypothesis | A possible rule, not established for the local identity |
| Measured fact | A scoped rule supported by local parsing, disassembly, comparison, or observation |
| Rebuild proof | Extraction and reconstruction preserve relevant behavior or bytes |
| Runtime proof | A controlled change is consumed through the intended game path |
| Gap | Missing knowledge that could change a decision |

A mature patch, toolkit, editor, or disassembly may supply useful evidence.
Preserve its provenance and verify applicability to the local input and new use;
do not promote inherited assertions by reputation. Keep original inputs and raw
evidence immutable while correcting the interpreted structure record when needed.

## Surface Readiness

Derive each label from its referenced evidence:

| Level | Referenced evidence |
| --- | --- |
| Surveyed | Likely locations and dependencies identified, with explicit gaps |
| Rebuild-proven | Relevant-surface proof gate passes |
| PoC-proven | Creative-unit PoC gate passes for the proposed surface use |
| Overlay-ready | Required proof covers the declared surfaces and cross-surface dependencies |

[Workflow Gates](workflow-gates.md) defines when work may proceed.
Its experimental-work conditions apply even at the surveyed level;
a readiness label must not prevent the experiment needed to establish proof.
Private playability and sharing are product outcomes, not structure-map levels.

## Gap-driven Work

Explore premises and provisional drafts while structure is unknown. Distinguish
an authored creative choice from a claim about existing engine or story state;
missing facts remain unknown.

When a rule changes, identify affected fields and dependent claims under
[Project State](../conventions/project-state.md#invalidation). Recheck those
dependencies while preserving unrelated work.
