# Technical Investigation

Use this guidance when the host game or an affected engine path is not understood,
including projects that have only original game files. Choose the next question
from the intended change and its unresolved dependencies. An existing structure
map, patch, or specialized skill is not a prerequisite.

## Establish A Working Baseline

Recover the desired change and protected behavior under
[Intent And Authority](intent-and-authority.md). Identify the local game revision
and representation before interpreting offsets or changing bytes. Distinguish
file offsets, mapped addresses, banks, and media coordinates where the path uses
them. Apply [Input Scope](../conventions/execution-records.md#input-scope) to any
additional originals used for research or reconstruction.

Inspect available project tools and evidence before building another analyzer.
Choose or adapt a parser, disassembler, debugger, or small probe for the question.
Look up recoverable platform and format specifications in primary sources; verify
game-specific interpretations against the local revision. Establish how to reach
and observe the original behavior using [Runtime Observation](runtime-observation.md).
If an observation is unavailable, continue independent analysis and keep that
runtime claim open.

## Follow The Affected Game Path

Investigate only questions that can change feasibility, implementation, or proof:

| Question | Evidence to seek |
| --- | --- |
| Where does the relevant content or behavior come from? | The files, regions, code, and references that select it; inspect outer containers only when the change depends on them |
| How does the game use it? | The applicable lookup, loading, decoding, rendering, playback, execution, or persistence path |
| What constrains the change? | Consumer-enforced limits, reference rules, live state, and protected adjacent behavior; distinguish observed usage from proven capacity |
| How far does a finding apply? | The entries and paths sharing the rule, evidence of that relationship, exceptions, and unexplored scope |

Byte patterns, plausible addresses, and another game's layout suggest candidates.
Establish their meaning through the actual reader, selection logic, or a controlled
observation that distinguishes competing explanations. For code changes, inspect
the affected control flow and state, including displaced instructions and returns
when relevant. A tool's plausible output is not evidence of completeness.

## Resolve A Bounded Question

Choose a small experiment under [Workflow Gates](workflow-gates.md#experimental-work).
State what each possible result would support before running it. A copied image
may be used to investigate an unknown loader or resource path without already
having proof of that path. Bound writes and isolate outputs as the gate requires.

For reconstruction, declare whether unchanged bytes or equivalent game consumption
is required and why. A parser and serializer, or compressor and decompressor, may
agree while sharing an incorrect assumption. Check against source evidence or the
game's consumer; their own round trip alone does not establish compatibility.

A representative experiment may precede expensive enumeration. Keep its observed
scope and remaining population explicit. Extending a finding to other entries
requires evidence of their membership and shared consumer, with exceptions
identified; one successful sample is not full coverage. Contradictory results
reopen the explanation rather than justify exceptions merely to preserve it.

## Retain The Result

Record supported facts, candidates, rejected explanations, evidence scope, and gaps
in [Structure-map Fields](../conventions/structure-map-fields.md). Use
[Structure-map Readiness](structure-map.md) to assess the proposed use and
[Project State](../conventions/project-state.md#research-experiments-and-adopted-work)
to adopt results and preserve the next action. Producing an analysis report does
not itself select a finding or build a playable game.
