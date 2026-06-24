---
purpose: produce-current-technical-research-for-client-workflows
updated: 2026-06-19
trigger: Run when a client decision depends on current tool behavior, current product facts, APIs, pricing, privacy terms, integration options, or implementation feasibility.
---

# Technical Research Brief

## Purpose

Create a current, source-backed technical brief for a client workflow or tool decision.

Use this when correctness depends on facts that may have changed.

## Required Current Research

Use current web research or authoritative documentation when investigating:

- product features
- pricing
- API behavior
- model capabilities
- usage limits
- privacy or data retention
- authentication
- integrations
- export/import behavior
- third-party connectors
- compliance claims
- platform restrictions

Prefer primary sources:

- official documentation
- official pricing pages
- official security/privacy pages
- release notes
- vendor help centers
- standards or policy pages

Use secondary sources only when primary sources are unavailable or insufficient, and label them clearly.

## Required Read

Read:

1. `context/client-profile.md`
2. `status/current-status.md`
3. relevant `workstreams/`
4. `tools/tool-stack.md`
5. `privacy/data-boundaries.md`
6. any attached technical notes or screenshots

## Research Question

Start by writing the exact decision question.

Examples:

- Can this client safely upload these documents to this tool?
- Which automation platform best fits this workflow?
- Does this tool support the required export?
- What is the current limitation that blocks this integration?
- Is this feature available on the client’s likely plan?

## Output Location

Create:

```text
research/YYYY-MM-DD-[topic].md
```

## Brief Structure

Use:

```markdown
# Technical Research Brief - [Topic]

## Decision Question

## Short Answer

## Recommendation

## Current Facts Verified

## Options Compared

## Implementation Notes

## Risks And Unknowns

## Privacy And Data Notes

## What To Test Next

## Sources

## Last Verified
```

## Source Rules

For each source, include:

- title
- URL
- publisher/vendor
- date if visible
- what fact it supports

Do not paste long copyrighted excerpts.

Summarize in your own words.

## Recommendation Style

Recommendations should be practical:

- use this now
- test this first
- wait
- park this
- avoid this
- needs client approval
- needs more information

Tie the recommendation back to client value, privacy, adoption, and current tool stack.

## Follow-On Updates

After the brief:

- update `tools/tool-stack.md` if a tool status changes
- update `privacy/data-boundaries.md` if a data boundary changes
- update relevant `workstreams/` if implementation steps become clear
- update `status/action-registry.md` if someone must act

## Quality Check

Before finishing, verify:

- the answer is current
- primary sources were preferred
- uncertainty is visible
- the recommendation is tied to the client’s actual workflow
- privacy implications are not buried
- next test is concrete

