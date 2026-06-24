---
purpose: reduce-active-workstream-clutter-and-focus-next-actions
updated: 2026-06-19
trigger: Run when the repo has too many active workstreams, call prep feels scattered, priorities are unclear, or older threads need parking, merging, or closing.
---

# Workstream Pruner

## Purpose

Keep the client operating repo focused.

This skill reviews active workstreams, identifies what should stay active, what should be parked, what should be merged, and what should be closed.

It protects the client and consultant from overload.

## Required Read

Read:

1. `status/current-status.md`
2. `status/action-registry.md`
3. `status/outcomes-scorecard.md`
4. all active `workstreams/`
5. recent `sessions/`
6. `context/client-profile.md`
7. `context/engagement.md`
8. `tools/tool-stack.md`

## Active Workstream Test

A workstream should remain active only if it has:

- clear client value
- current relevance
- a next smallest action
- an owner or decision point
- evidence from recent sessions or commitments

If any of these are missing, park, merge, or mark as needs clarification.

## Status Values

Use:

- `Active`
- `Waiting`
- `Blocked`
- `Parked`
- `Completed`
- `Superseded`
- `Needs clarification`

## Pruning Decisions

### Keep Active

Use when the workstream is important now and has a clear next move.

### Park

Use when it is real but not worth attention now.

### Merge

Use when two workstreams represent the same client outcome.

### Close

Use when the outcome is complete, abandoned, or no longer relevant.

### Supersede

Use when a better approach replaces the old one.

## Next Smallest Action

Every active workstream must have one next smallest action:

- specific
- owned
- doable before or during the next session
- not dependent on a vague future plan

## Output

Update relevant `workstreams/` files and `status/current-status.md`.

Then report:

```markdown
# Workstream Pruning Report

## Kept Active

## Parked

## Merged

## Completed Or Closed

## Needs Clarification

## Next Smallest Actions

## Suggested Next Session Focus
```

## Quality Check

Before finishing, verify:

- active workstreams are few enough to reason about
- each active workstream has one next smallest action
- parked workstreams preserve context without demanding attention
- no client commitment was lost
- status files reflect the pruning decision

