---
purpose: maintain-open-actions-commitments-blockers-and-ownership
updated: 2026-06-19
trigger: Run when source material, call prep, follow-up, or repo cleanup reveals commitments, next steps, blockers, questions, or ownership changes.
---

# Action Registry Maintainer

## Purpose

Keep `status/action-registry.md` accurate, useful, and small enough to act on.

The action registry is the operational memory for commitments.

It should prevent dropped balls without becoming a graveyard of vague tasks.

## Required Read

Read:

1. `status/action-registry.md`
2. `status/current-status.md`
3. latest relevant `sessions/`
4. active `workstreams/`
5. `context/stakeholders.md`
6. `context/engagement.md`
7. any newly attached source material

## What Counts As An Action

Add or update an action when there is:

- a clear owner
- a clear next move
- a reason it matters
- a source or evidence trail

Actions may belong to:

- AOTW
- client
- stakeholder
- unknown owner requiring clarification

## What Does Not Count

Do not add:

- vague ideas
- possible future automations
- generic "explore AI" items
- completed actions unless they need historical recording
- implied tasks without evidence
- reminders that belong only inside a workstream note

## Registry Format

Maintain sections:

```markdown
# Action Registry

## Active

| ID | Owner | Action | Source | Due / Timing | Status | Next Check |
|---|---|---|---|---|---|---|

## Waiting On Client

## Waiting On AOTW

## Blocked

## Parked

## Completed

## Superseded
```

Use stable IDs:

```text
A-001
A-002
A-003
```

Do not renumber existing actions.

## Status Values

Use:

- `Active`
- `Waiting on client`
- `Waiting on AOTW`
- `Blocked`
- `Parked`
- `Completed`
- `Superseded`
- `Needs clarification`

## Maintenance Rules

When processing new evidence:

1. Match new action candidates against existing actions.
2. Merge duplicates.
3. Update status instead of creating a second item.
4. Preserve source references.
5. Add a short note if the action changed materially.
6. Close completed items only when evidence supports completion.
7. Park actions that are real but not currently worth attention.
8. Supersede actions replaced by a better plan.

## Priority Guidance

Highlight:

- promises made by AOTW
- client asks that are waiting
- blockers that stop adoption
- time-sensitive scheduling or access issues
- actions needed before the next session

Avoid highlighting:

- interesting but non-urgent tool ideas
- open-ended research unless it blocks a decision

## Output

Update `status/action-registry.md`.

Then report:

```markdown
# Action Registry Update

## Added

## Updated

## Completed

## Parked Or Superseded

## Needs Clarification

## Highest-Risk Open Commitment

## Before Next Session
```

## Quality Check

Before finishing, verify:

- every active action has an owner
- every active action has a next move
- AOTW commitments are easy to find
- client commitments are not framed as blame
- old duplicates were merged
- no action was invented from weak evidence

