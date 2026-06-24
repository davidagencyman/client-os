---
purpose: extract-reusable-aotw-service-patterns-from-client-work
updated: 2026-06-19
trigger: Run when a session, source material, workflow, prompt, coaching move, or implementation pattern could become reusable AOTW service IP.
---

# Service IP Extractor

## Purpose

Extract reusable AOTW delivery patterns from client work while protecting client privacy.

The output should strengthen `playbooks/personal-ai-upgrade-playbook.md` without copying private client details.

## Required Read

Read:

1. `playbooks/personal-ai-upgrade-playbook.md`
2. relevant `sessions/`
3. relevant `workstreams/`
4. `status/service-retrospective-log.md` if present
5. `privacy/data-boundaries.md`
6. source material that contains the pattern

Run `privacy-boundary-check.md` if the pattern may include client-identifying or sensitive material.

## What Counts As Reusable IP

Extract patterns such as:

- diagnostic questions
- consulting sequences
- adoption coaching moves
- prompt structures
- learning asset formats
- privacy boundary patterns
- tool governance rules
- stakeholder explanation patterns
- habit-building techniques
- technical implementation checklists
- failure modes and prevention rules

## What Does Not Count

Do not add:

- one-off client facts
- private strategy
- confidential examples
- tool recommendations without general usefulness
- long transcript quotes
- patterns not yet tested or reasoned through

## Generalization Rules

Before adding to the playbook:

- remove client names
- remove company names
- remove private facts
- replace specific context with a general use case
- keep the underlying consulting move
- mark confidence if the pattern is early

## Playbook Entry Structure

Add entries like:

```markdown
## [Pattern Name]

**When to use:**  
**Client signal:**  
**Consulting move:**  
**Example phrasing:**  
**AI workflow pattern:**  
**Risks:**  
**Proof level:**  
**Source type:**  
```

## Proof Level

Use:

- `Observed once`
- `Observed repeatedly`
- `Client adoption evidence`
- `AOTW delivery standard`
- `Needs more testing`

## Output

Update `playbooks/personal-ai-upgrade-playbook.md`.

Then report:

```markdown
# Service IP Update

## Pattern Added

## Source

## Privacy Handling

## Proof Level

## Where It May Be Reused

## Needs More Testing
```

## Quality Check

Before finishing, verify:

- no private client detail was copied
- the pattern is useful outside one client
- risks are included
- proof level is honest
- the playbook remains practical

