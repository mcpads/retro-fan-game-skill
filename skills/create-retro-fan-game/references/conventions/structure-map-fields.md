# Structure-map Fields

Reuse the project's existing machine-readable structure representation when one
already owns these meanings. Otherwise, introduce one structure record as the
source of truth for fields that drive extraction, generation, mutation,
validation, or observation. Human documents may explain the record but should
point to its stable identities instead of copying values.

## Base Identity

This record owns the execution host whose engine and surfaces produce the
playable output. Additional source games do not become host bases merely
because their story or assets constrain a component.

Record:

- platform and media type,
- region, revision, and other identifying details,
- expected input sizes and hashes,
- immutable baseline location or logical identifier,
- provenance of inherited facts,
- output identity policy: expected hash or permitted differences and their checks.

Keep additional `build_source` and `evidence_only` input identities in the
composition scope and execution records. Link only the dependencies a host
surface actually consumes.

Unknown values remain explicit. Do not use a guessed default in a build-driving
field.

## Surface Record

Each editable surface has one stable ID and records:

- human-readable name and owning subsystem,
- source location or deterministic lookup rule,
- evidence state and evidence references,
- mutable, protected, and unknown fields,
- encoding, control, terminator, format, or container rules that apply,
- byte, line, glyph, tile, palette, timing, memory, file, and route-state budgets
  that are relevant to that surface,
- pointer, index, relocation, compression, checksum, or media rules that apply,
- dependencies on fonts, assets, flags, scripts, tables, or other surfaces,
- extraction and rebuild checks,
- minimal PoC identity,
- runtime route and observable required for a consumption claim,
- unresolved gaps and the judgments they block.

Do not add irrelevant placeholder fields merely to make every platform record
look alike. Required means required by the declared surface or its dependencies.

## Evidence Entry

Every claim about a field identifies:

- subject field and asserted value,
- status: `hypothesis`, `measured`, `rebuild_proven`, or `runtime_proven`,
- applicability: `current`, `invalidated`, or `superseded`, separate from the
  kind of evidence previously obtained,
- source identity and evidence reference,
- scope and known limits, including inspected coverage, shared-consumer evidence,
  and exceptions when a claim spans a population,
- dependent fields or claims that must be revisited if it changes.

Correct interpreted facts using
[Project State](project-state.md#invalidation); retain earlier evidence and the
reason for supersession. Builds and assessments pin the structure contents they
used, so updating a stable field ID cannot silently validate an older result.

## Conditional Inserted-resource Record

Create this record only when the overlay inserts a resource the base did not
already expose as a replaceable slot. Record:

- stable overlay ID and runtime resource identity,
- source class and provenance reference,
- owning table, archive, filesystem, bank, or loader lookup,
- insertion strategy and every affected count or index,
- final format, size, alignment, compression, and hash,
- discovery trigger, load or transform path, residence and lifetime,
- consumption route, retirement or unload behavior, and failure behavior,
- adjacent resources that could shift, collide, or be shadowed,
- dependencies, budgets, static checks, and runtime observation claim,
- rollback or disable behavior used for diagnosis.

During investigation, mark unknown chain links and proposed values explicitly.
The registry describes the experiment as well as the adopted result; its presence
does not imply insertion readiness. Apply
[Workflow Gates](../strategy/workflow-gates.md#experimental-work) to experiments
and its PoC gate to promotion.

When sharing is in scope, the package manifest points to this registry. The
registry itself does not make packaging mandatory.

## Build Linkage

Link the structure record to the deterministic extractor or product builder interface,
the checks that validate it, and the expected-write records that consume it.
Keep current selection in the project's current entry and runtime results in
observation records. Structure facts may be corrected without rewriting that
history.
