# Resource Insertion

Resource insertion adds something the base has no replaceable slot for. The game
must discover and consume it, which storage space alone does not show.

## Choose A Method For The Intended Work

Compare reuse or repurposing, table or archive extension, relocation to free or
appended storage, additional entries, and loader hooks as they apply, and prefer
the method with fewer unproven dependencies that still delivers the intended
work. Insert when the intended work needs a new resource, and keep required
original content intact; when reuse would overwrite content the person may
want, return that tradeoff under [Intent And Authority](intent-and-authority.md).

## Investigate The Runtime Asset Chain

Map the chain, marking measured links and unknowns:

`storage -> discovery -> load or transform -> residence -> consumption -> retirement`

Cover the owning table or lookup, identities and counts, format rules, memory
destination and lifetime, failure behavior, and adjacent resources that could
shift or be shadowed. Record it in the
[inserted-resource record](../conventions/structure-map-fields.md#conditional-inserted-resource-record).
Each unknown link is a bounded investigation target.

## Minimal Insertion Experiment

Admit one small observable insertion under
[Experimental Work](workflow-gates.md#experimental-work); it may itself establish
the unknown discovery, load, or retirement behavior. Observe the new resource and
an adjacent old one through the real consumption path, including cache,
fallback, and retirement, and choose the next experiment from the links still
open.

## Persistent State

New saved state is an insertion into the save format. Establish the ownership
and lifetime of existing flags before taking one that looks unused. Test new
game, load, copy, delete, and a corrupt record, seeding non-default values so a
pass reflects the new state. State what each value means, and decide corruption
recovery before it gates anything the player would lose. Append fields to keep
the layout stable, and refuse incompatible saves while keeping them intact.

## Promotion

The insertion PoC supports expansion once the affected chain and adjacent
behavior have evidence under
[Workflow Gates](workflow-gates.md#creative-unit-poc-gate), scoped to the tested
loader, resource type, and states.
