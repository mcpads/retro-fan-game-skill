# Execution Records

Execution records preserve what a run consumed, wrote, checked, and produced.
Classify operations under [Work Roles](work-roles.md).

## Expected Write

Before mutating a binary or container, record the owning unit, the source
location, the allowed range, the expected source bytes, the final bytes or their
derivation, any alignment, relocation, checksum, or compression update, and a
check that fails if the write is skipped or misapplied. Every final difference
has exactly one owner or an explicit composition rule. Stop the run on a source
mismatch, overlapping owners, a write into a protected range, a missing
dependency or asset, an unknown entry, a failed conversion, or an unowned
difference.

## Input Scope

Record what each task consumes. An additional original is a `build_source` when
adopted material is reconstructed from it; verify its identity and keep that
reconstruction in the product build, even when a cached extract exists. It is
`evidence_only` when it is read to establish facts or guide new work. Identify
borrowed inputs by content hash, since a repository commit does not identify a
dirty working tree.

## Product Build Path

Keep one documented path from the selected inputs to the cumulative game image,
combining every adopted change for the declared route. Every stage that changes
the output, including postprocessing, goes through [Expected Write](#expected-write);
manual fixups after verification break the path. Derive layout and values from
the declared inputs, reparse rebuilt structures, and reject invalid inputs or
output even when tooling and tests pass. Failed or partial outputs stay in a
separate diagnostic location; the selected playable moves only on success.

## Transform Record

For each deterministic transform, record its source revision, consumed input
hashes, configuration, toolchain identities that affect output, declared
outputs, checks, and what happens to partial output on failure.

## Execution Receipt

Each run records its purpose, input and transform identities, expected-write
set, checks with pass, fail, or skipped status, output hashes, unexplained
differences against the baseline, and warnings. A successful receipt has no
skipped required check and no unexplained difference. Failed checks stay
recorded as failures, including in experiments whose results are kept. Runtime
evidence names the receipt of the build it observed.
