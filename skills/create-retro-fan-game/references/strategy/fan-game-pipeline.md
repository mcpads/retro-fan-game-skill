# Fan-game Decision Flow

Fan-game work is a graph of judgments, not a universal sequence. Start from the
current decision and seek the cheapest evidence that could change it. Open
independent branches in parallel when useful, but respect the dependency gates
that protect build integrity and runtime claims.

## Judgment Branches

| Branch | Question it owns | Typical next evidence |
| --- | --- | --- |
| Intent and authority | What does the person want to play, and which choices remain theirs? | bounded creative target and approval boundary |
| Component semantics | Which independently sourced or authored components compose the work, and which specialized claims constrain them? | component graph and optional capability handoffs |
| Structure | Is the relevant game surface understood well enough for the proposed mutation? | identity, extraction/rebuild proof, measured constraints, or one resolved gap |
| Creative overlay | What is being changed without silently widening the work? | brief, approved option, or narrow unit inventory |
| Execution | Can the declared input be transformed deterministically and safely? | expected writes, static checks, and execution receipt |
| Observation | What evidence would distinguish the runtime claim from failure? | route-specific raw observation and interpretation |
| Optional sharing | Can another owner build the declared target without receiving original game material? | manifest and clean-workspace reconstruction |

## Dependency Edges

- Intent may be explored before structure is complete, but build-bound content
  for a surface depends on that surface's structure proof.
- Components may use different source relationships and domain capabilities.
  Broad production for a specialized claim depends on that capability's scoped
  readiness assessment, not on a project-wide mode label.
- Broad build-bound generation depends on a creative-unit PoC through the real
  game-consumption path.
- Resource insertion depends on proof of the complete runtime asset chain, not
  merely on available storage space.
- A private-playable claim depends on execution and observation for the intended
  personal route.
- Sharing is a separate branch. It depends on private playability across the
  declared shareable scope, but private playability never depends on packaging.

Exact pass conditions belong to `references/strategy/workflow-gates.md`.

## Choosing The Next Move

Prefer an action that resolves a live fork: inspect an unknown field before
building around it, prove one representative unit before generating a corpus,
or observe the route before diagnosing from intermediate data. Do not perform a
large downstream task merely because it is easy to automate.

When a result is ambiguous, preserve it as evidence, narrow the claim, and pick
a more discriminating action. Do not weaken a gate to fit an available tool.

## Invalidation

New evidence invalidates only the judgments that depend on it. A changed
creative brief does not erase base identity; a corrected pointer rule may
invalidate affected builds and observations without erasing unrelated surface
proof. Record the affected identities so the next action can be scoped rather
than restarting the whole project.
