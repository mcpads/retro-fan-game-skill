# Structure-map Readiness

A structure map connects reverse engineering to the surfaces and dependencies the
intended segments need. Fields belong to
[Structure-map Fields](../conventions/structure-map-fields.md); establish missing
facts with [Technical Investigation](technical-investigation.md).

## Evidence Distinctions

| Evidence | Supports |
| --- | --- |
| Hypothesis | A possible rule for the local identity |
| Measured fact | A scoped rule from local parsing, disassembly, comparison, or observation |
| Rebuild proof | Extraction and reconstruction preserve relevant behavior or bytes |
| Runtime proof | A controlled change is consumed through the intended game path |
| Gap | Missing knowledge that could change a decision |

A mature patch, toolkit, editor, or disassembly supplies candidate facts; record
its provenance and verify each fact against the local input before use.

## Surface Readiness

| Level | Evidence |
| --- | --- |
| Surveyed | Likely locations and dependencies, with explicit gaps |
| Rebuild-proven | Relevant-surface proof gate passes |
| PoC-proven | Creative-unit PoC gate passes for the proposed use |
| Overlay-ready | Proof covers the declared surfaces and their shared dependencies |

Experiments that establish proof may run at any level under
[Workflow Gates](workflow-gates.md#experimental-work). When a rule changes,
revisit its dependents under
[Invalidation](../conventions/project-state.md#invalidation).
