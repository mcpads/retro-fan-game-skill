# Structure-map Readiness

A structure map is the contract between reverse engineering and build-bound
creative work. It need not describe the whole game; it must describe every
surface and dependency claimed by the intended overlay.

Concrete fields belong to
`references/conventions/structure-map-fields.md`.

## Evidence Distinctions

Keep these states explicit:

| State | Meaning |
| --- | --- |
| Hypothesis | Plausible but not proven for the local identity |
| Measured fact | Supported by local parsing, disassembly, comparison, or observation |
| Rebuild proof | Extraction and reconstruction preserve the relevant behavior or bytes |
| Runtime proof | A controlled mutation was consumed through the intended game path |
| Gap | Missing knowledge that could alter the build or claim |

A hidden hypothesis is more dangerous than a visible gap. Never promote an
inherited claim merely because it came from a mature translation patch, mod,
toolkit, editor, or disassembly; preserve its provenance and verify it when the
new overlay depends on it.

## Relevant-surface Readiness

| Level | Meaning | Allowed work |
| --- | --- | --- |
| Surveyed | Likely locations and dependencies are identified | planning and provisional creative exploration |
| Rebuild-proven | Relevant extraction, encoding, relocation, and reconstruction behavior is established | tooling and one controlled mutation |
| PoC-proven | One minimal changed unit is observed through the real game path | bounded expansion on that proven surface |
| Overlay-ready | Every surface and cross-surface dependency in the declared overlay has the required proof | declared overlay development |

Private playability and sharing are product completion states, not structure-map
readiness levels. Their definitions remain in
`references/strategy/workflow-gates.md`.

## Activation Rule

People may explore premises, briefs, and provisional drafts while structure is
unknown. Do not commit broad generated or authored content to a build surface
until the relevant structure and one-unit PoC are proven. Unknown engine or
story-state facts become questions or gaps, not invented constraints.

## Gap-driven Work

When existing artifacts are available, begin with a gap list. Prefer proving the
smallest missing fact that unlocks the intended overlay over remapping unrelated
game systems. If evidence changes, invalidate the affected fields, builds, and
runtime claims while retaining unrelated proof.
