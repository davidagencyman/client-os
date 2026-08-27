---
purpose: client-os-v6-core-file-templates
version: 6.0
updated: 2026-08-27
---

# Client OS v6 Core File Templates

These are starting templates, not excuses to fill every section with generic
text. Replace placeholders with evidence or mark the field unknown.

## context/client.md

~~~
---
purpose: client-context
updated: YYYY-MM-DD
status: prospective | active | paused | closed
confidence: confirmed | mixed | provisional
---

# Client

## Canonical identity

- Name:
- Company / role:
- Contact and lookup information:
- Identity evidence:

## What the client actually does

## Work, pain, and goals

## Working style and communication

## Constraints and sensitivities

## Important language

## Unknowns to confirm
~~~

## context/engagement.md

~~~
---
purpose: engagement-context
updated: YYYY-MM-DD
stage: discovery | proposed | active | paused | closed
---

# Engagement

## Confirmed scope

## Proposed or unconfirmed scope

## Session rhythm and duration

## Success criteria

## Working agreements

## Commercial and operational terms

## Timeline

## Open questions
~~~

## status/current.md

~~~
---
purpose: current-status
updated: YYYY-MM-DD
---

# Current Status

## Active now

## Blocked

## Planned

## Completed recently

## Next useful focus

## Sources checked and freshness
~~~

## status/actions.md

~~~
---
purpose: action-registry
updated: YYYY-MM-DD
---

# Actions

| ID | Owner | Status | Next step | Source/date |
|---|---|---|---|---|
| | | | | |

Status values: active, waiting, blocked, parked, complete.
~~~

## status/decisions.md

~~~
---
purpose: decisions-log
updated: YYYY-MM-DD
---

# Decisions

## YYYY-MM-DD

- Decision:
- Why:
- Conditions:
- Source:
~~~

## privacy.md

~~~
---
purpose: data-boundaries
updated: YYYY-MM-DD
---

# Privacy and Data Boundaries

## Private session memory

Preserve important evidence needed for future consulting work. Do not store
passwords, API keys, authentication tokens, recovery codes, or unnecessary raw
third-party material.

## App Export

Only client-safe material belongs in app/profile.json. Exclude internal
coaching observations, raw source material, sensitive third-party details, and
unagreed internal analysis.

## External tools

Record what may be uploaded, what requires approval, and what is not allowed.

## Current boundaries and unknowns
~~~

## capabilities.md

~~~
---
purpose: capability-catalog
updated: YYYY-MM-DD
---

# Capabilities

## Core

| Capability | Use when | Reads | Writes | Status |
|---|---|---|---|---|
| Operating Router | Any unclear request | README, status, context | Routing decision | enabled |
| Process Session | New source material | Current context and recent sessions | Detailed session and necessary state | enabled |
| App Export | After successful processing or explicit export request | Internal state and prior profile | app/profile.json and chat JSON | enabled |
| Session Supervisor | Preparing for a session | Current state and recent sessions | Conversation, optional focus note | enabled |
| Follow-up | After a session or explicit request | Session and actions | Draft message | enabled |
| Privacy Boundary | Before sharing or uploading | Data-boundary rules | Boundary decision | enabled |

## Optional

Add only when needed. Record the reason and the date enabled.

| Capability | Reason enabled | Date | Status |
|---|---|---|---|
~~~
