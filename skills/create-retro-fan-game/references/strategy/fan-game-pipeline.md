# Fan-game Decision Flow

Start from the intended playable and the current unresolved decision. Choose
the smallest action whose result can change what happens next. Work may branch
or return to investigation; it is not a universal linear schedule.

## Select The Branch

| Uncertainty | Useful next result | Read |
| --- | --- | --- |
| What does the person want to experience or preserve? | A contextual sample or consequential choice | [Intent And Authority](intent-and-authority.md) |
| What work and evidence are currently selected? | Verified current-state entry | [Project State](../conventions/project-state.md) |
| Which source meanings and host surfaces constrain the work? | Bounded components and dependencies | [Creative Overlay](creative-overlay.md) |
| What does the relevant engine path actually allow? | Measured fact or bounded experiment | [Technical Investigation](technical-investigation.md) |
| Which technical operation and evidence does the next decision need? | Work role with explicit input and claim boundaries | [Work Roles](../conventions/work-roles.md) |
| Can the selected changes form one reproducible game image? | Cumulative product build and verification receipt | [Execution Records](../conventions/execution-records.md#product-build-path) |
| Does the game use the change correctly? | Evidence distinguishing expected behavior from failure | [Runtime Observation](runtime-observation.md) |
| Is the work ready to expand or complete? | Scoped evidence assessment | [Workflow Gates](workflow-gates.md) |
| Can the declared work be shared? | Package inventory and reconstruction evidence | [Optional Patch Package](patch-package.md) |

## Choose Work That Changes The Decision

Inspect an unknown field before building around it, prove a representative unit
before generating a corpus, and observe a failing route before diagnosing from
intermediate data alone. Do not perform a large downstream task merely because
it is easy to automate.

Use [Workflow Gates](workflow-gates.md) to distinguish experimental work from
production expansion. One successful surface does not establish the readiness
of a different loader, format, or route dependency. Independent branches may
advance while another awaits evidence or a human decision.

When a result is ambiguous, preserve it and choose an observation that distinguishes
the remaining explanations. Narrowing a technical question must not shrink the
person's completion target. Investigate missing evidence or present the actual
tradeoff rather than weakening the pass condition.

After a result, update its owning record and the current entry under
[Project State](../conventions/project-state.md). Adopt only supported results,
invalidate affected dependencies when needed, and choose the next unresolved
decision against the intended playable.
