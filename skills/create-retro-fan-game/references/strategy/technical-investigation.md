# Technical Investigation

Use this when the host game or an affected engine path is not understood,
including when the project has only original game files. Choose the next
question from the segment's intended change and its open dependencies.

## Establish A Working Baseline

Recover the desired change and protected behavior under
[Intent And Authority](intent-and-authority.md). Identify the local game revision
and representation before interpreting offsets, and distinguish file offsets,
mapped addresses, banks, and media coordinates where the path uses them. Assign
roles to additional originals under
[Input Scope](../conventions/execution-records.md#input-scope).

Use available project tools and evidence first, then choose or adapt a parser,
disassembler, debugger, or small probe for the question. Take platform and format
specifications from primary sources and verify game-specific interpretations
against the local revision. Establish how to reach and observe the original
behavior with [Runtime Observation](runtime-observation.md); while observation is
unavailable, continue analysis and keep the runtime claim open.

## Follow The Affected Game Path

Investigate the questions that can change feasibility, implementation, or proof:

| Question | Evidence to seek |
| --- | --- |
| Where does the content or behavior come from? | The files, regions, code, and references that select it |
| How does the game use it? | The lookup, loading, decoding, rendering, playback, execution, or persistence path |
| What constrains the change? | Consumer-enforced limits, reference rules, live state, and protected adjacent behavior, separating observed usage from proven capacity; memory that looks free must stay free across boot, dialogue, menus, battle, and scene reloads |
| What else does a reused identity carry? | Behavior the host attaches to a reused map, index, or flag, such as themes, music, or events; select presentation explicitly |
| How far does a finding apply? | The entries sharing the rule, evidence of that membership, exceptions, and unexplored scope |

Byte patterns, plausible addresses, another game's layout, and names from older
tools or documents are hypotheses. Establish meaning through the reader or
handler that uses the data, or through an observation that separates the
explanations. Confirm what a field means against an independent observable, such
as the screen, sound, or manual; a test reading the implementation's own
definition shares its mistakes. For code changes, trace the affected control flow
and state, including displaced instructions and returns.

## Resolve A Bounded Question

Choose a small experiment under
[Workflow Gates](workflow-gates.md#experimental-work) and state what each result
would support before running it. A copied image may be used to probe an unknown
loader.

For reconstruction, declare whether identical bytes or equivalent consumption is
required. Check a parser and serializer, or compressor and decompressor, against
source evidence or the game's consumer, since their round trip can share a wrong
assumption.

A representative experiment may come before full enumeration; record its
observed scope and the remaining population. Extend a finding to other entries
with evidence of their shared consumer and identified exceptions. A
contradictory result reopens the explanation.

## Retain The Result

Record facts, candidates, rejected explanations, scope, and gaps in
[Structure-map Fields](../conventions/structure-map-fields.md), judge the
proposed use with [Structure-map Readiness](structure-map.md), and adopt results
under [Project State](../conventions/project-state.md#research-experiments-and-adopted-work).
