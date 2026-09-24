# Structure-map Fields

Use the project's existing machine-readable structure record when one exists;
otherwise create one as the source of truth for fields that drive extraction,
mutation, validation, or observation. Documents point to its IDs.

## Base Identity

The execution host is the original game whose engine and surfaces produce the
playable output; other source games keep their roles under [Input
Scope](execution-records.md#input-scope). For the host, record platform, media,
region, revision, expected sizes and hashes, the immutable baseline location,
provenance of inherited facts, and the output identity policy. Unknown values
stay marked unknown in build-driving fields.

## Surface Record

Give each surface the segments need a stable ID and record what applies to it:
location or lookup rule, mutable and protected fields, encoding and format
rules, budgets, pointer, relocation, compression, or checksum rules,
dependencies, extraction and rebuild checks, the minimal PoC, the route that
observes it, and open gaps with the judgments they block.

## Evidence Entry

Each field claim records its value, status (`hypothesis`, `measured`,
`rebuild_proven`, `runtime_proven`), applicability (`current`, `invalidated`,
`superseded`), source and evidence reference, covered scope and exceptions, and
dependents to revisit if it changes. Builds and assessments pin the structure
contents they used.

## Conditional Inserted-resource Record

When the overlay inserts a resource the base had no slot for, record its ID and
provenance, the owning table or loader, affected counts and indices, final
format and hash, and each link of the chain from discovery through consumption
to retirement, plus adjacent resources that could shift, the runtime claim, and
how to disable it for diagnosis. Mark unmeasured links as unknown.
