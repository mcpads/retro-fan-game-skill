# Resource Insertion

Resource insertion adds something the base does not expose as a replaceable
slot. Storage space alone does not establish that the game can discover and
consume it.

## Choose A Method For The Intended Work

Compare reuse or repurposing, table or archive extension, relocation to free or
appended storage, additional entries, and loader hooks as applicable. Prefer the
method with fewer unproven dependencies when it preserves the intended work.
This is not a mandatory sequence of implementations to attempt.

Do not overwrite required original content to avoid insertion, or insert merely
for authoring convenience. Investigate the actual content loss and runtime risks.
Return a consequential creative tradeoff under
[Intent And Authority](intent-and-authority.md); select technical means within
that decision autonomously.

## Investigate The Runtime Asset Chain

Map the relevant chain, marking measured links and unknowns:

`storage -> discovery -> load or transform -> residence -> consumption -> retirement`

Cover the owning table or lookup, identities and counts, format and media rules,
memory destination and lifetime, failure behavior, and adjacent resources that
could shift or be shadowed. Records belong to
[Structure-map Fields](../conventions/structure-map-fields.md#conditional-inserted-resource-record).
An unknown link is a bounded investigation target, not a guessed production rule.

## Minimal Insertion Experiment

Use [Experimental Work](workflow-gates.md#experimental-work) to admit one small
observable insertion. The experiment may establish the previously unknown discovery,
load, or retirement behavior; the complete runtime chain need not be proven
before this isolated experiment.

Observe the new resource and a relevant adjacent old resource through the real
consumption path, including affected cache, fallback, and retirement behavior.
A successful write or one displayed frame cannot cover unobserved lifetime or
state dependencies. Keep ambiguous links open and choose the next experiment
from their missing evidence.

## Promotion

The insertion PoC supports production expansion only when the affected chain and
adjacent behavior have sufficient evidence under
[Workflow Gates](workflow-gates.md#creative-unit-poc-gate). Scope that evidence to
the tested loader, resource type, and relevant states; do not generalize it to
unrelated resources.

When sharing is in scope, apply
[Asset Distribution Policy](asset-distribution-policy.md) to the inserted material
and its containing archive.
