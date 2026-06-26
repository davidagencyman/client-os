---
purpose: prevent-tool-sprawl-and-maintain-client-tool-stack-status
updated: 2026-06-19
trigger: Run when tools, platforms, automations, integrations, access issues, or tool choices are mentioned or changed.
---

# Tool Stack Governor

## Purpose

Maintain `tools/tool-stack.md` as the practical record of tools in play, tools under consideration, blocked tools, parked tools, and retired tools.

The goal is to prevent shiny-tool chasing and help the client use the smallest effective tool stack.

## Required Read

Read:

1. `tools/tool-stack.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `status/current-status.md`
5. `status/outcomes-scorecard.md`
6. `privacy/data-boundaries.md`
7. active `workstreams/`
8. latest relevant `sessions/`
9. current web sources when tool behavior, pricing, access, limits, or policies may have changed

## Tool Status Values

Use:

- `Active`
- `Testing`
- `Recommended`
- `Considering`
- `Blocked`
- `Parked`
- `Retired`
- `Rejected`
- `Unknown`

## Tool Record Template

Maintain entries like:

```markdown
## [Tool Name]

**Status:**  
**Use case:**  
**Owner:**  
**Client value:**  
**Current blocker:**  
**Privacy considerations:**  
**Adoption evidence:**  
**Next decision:**  
**Last verified:**  
```

## Governance Questions

For each tool, answer:

- What real client job does this tool serve?
- Is it replacing, augmenting, or duplicating something?
- Who will use it?
- What data will pass through it?
- Is access already available?
- Is the client likely to use it between sessions?
- Is there a simpler option?
- What would prove it is worth keeping?
- What would trigger retirement?

## Current Research

Use current web research when a decision depends on:

- pricing
- feature availability
- API limits
- data retention
- privacy terms
- product changes
- integration support
- current authentication behavior

If current research is needed but not performed, mark the tool as `Needs verification`.

## Privacy Link

If a tool handles client data, update or reference `privacy/data-boundaries.md`.

Run `privacy-boundary-check.md` before recommending uploads of sensitive data to third-party tools.

## Output

Update `tools/tool-stack.md`.

Then report:

```markdown
# Tool Stack Update

## Tools Added

## Tools Updated

## Tools Parked Or Retired

## Access Or Integration Blockers

## Privacy Notes

## Current Research Needed

## Recommended Next Tool Decision
```

## Quality Check

Before finishing, verify:

- no tool is recommended without a client job
- blocked tools have a clear blocker
- parked tools are not silently active
- tool status reflects evidence
- privacy concerns are visible
- the stack is getting simpler where possible

