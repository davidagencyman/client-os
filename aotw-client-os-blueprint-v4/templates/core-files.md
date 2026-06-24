---
title: Core File Templates
purpose: repo-file-templates
version: 4.0
updated: 2026-06-19
---

# Core File Templates

Use these templates when building a new AOTW Client OS repository.

Replace bracketed placeholders with client-specific evidence. Do not invent facts.

---

## README.md

```markdown
---
purpose: ai-entry-point
updated: YYYY-MM-DD
---

# Client OS - [Client Name]

This repository is an AI-readable operating system for an Ahead of the Wave AI consulting engagement.

It helps the AOTW team prepare sessions, process source material, track commitments, preserve client context, measure adoption, protect privacy, and choose the next useful step.

## Reading Order

1. `_skills/operating-router.md`
2. `method/personal-ai-upgrade-method.md`
3. `context/client-contact.md`
4. `context/client-profile.md`
5. `context/engagement.md`
6. `context/stakeholders.md`
7. `status/current-status.md`
8. `status/action-registry.md`
9. `status/outcomes-scorecard.md`
10. `tools/tool-stack.md`
11. `privacy/data-boundaries.md`
12. relevant `workstreams/`
13. relevant `sessions/`

## Repo Map

```text
_skills/       Complete operating skills for AI agents
context/       Client identity, contact lookup, profile, engagement, stakeholders, voice
status/        Current status, actions, decisions, outcomes, practice plan
workstreams/   Concrete recurring work topics
sessions/      Processed session and discovery notes
method/        Consulting method and adoption philosophy
tools/         Tool stack and tool roles
privacy/       Data boundaries and safety rules
research/      Dated technical research briefs
learning/      Micro-SOPs, prompt cards, learning bundles
client-facing/ Client-safe outputs when explicitly requested
playbooks/     Internal reusable service IP
templates/     Repo templates
```

## Source Material Workflow

Do not require an `_inbox/` folder.

When a transcript, email, document, screenshot, or note is attached directly to Codex or Claude Code, start with `_skills/operating-router.md`. The router decides whether to run `_skills/process-source-material.md` and which follow-on skills are useful.

## Connected Tools

For session prep and any task where recent context matters:

1. Check Calendar first.
2. Check Gmail second.
3. Check other connected tools only when useful.

Always use `context/client-contact.md` for search terms.

## Usefulness Rule

New files or sections should only be added if they improve session preparation, client outcomes, privacy, tool clarity, adoption tracking, or service reuse.
```

---

## CLAUDE.md

```markdown
# Client OS - [Client Name]

This is not code. This is an AI-readable operating repository for an Ahead of the Wave AI consulting engagement.

Read `README.md` first.

Start with `_skills/operating-router.md` unless the user explicitly names a narrower skill.

For attached transcripts, notes, emails, or documents, use `_skills/process-source-material.md`.

For session preparation, use `_skills/call-prep.md`.

For the consulting method, read `method/personal-ai-upgrade-method.md`.

Before searching Calendar, Gmail, or other connected tools, read `context/client-contact.md`.

Do not infer the client name from the repo slug unless `context/client-contact.md` lists it as an alias.

Do not treat this repository as a task dump. It exists to help the AOTW team deliver humane, practical, high-quality AI consulting that compounds over time.
```

---

## method/personal-ai-upgrade-method.md

```markdown
---
purpose: consulting-method
updated: YYYY-MM-DD
---

# Personal AI Upgrade Method

This repository supports a long-term one-on-one AI consulting and coaching engagement.

The service is not generic AI training. It is practical transformation for a professional whose real work is spread across communication, documents, relationships, memory, tools, and organizational constraints.

## Core Belief

AI should adapt to the client’s work, language, responsibilities, standards, and human style.

The client should not feel forced to become an "AI person" or reorganize life around tools.

The goal is not to impress the client with AI tricks. The goal is to make real work lighter, clearer, faster, and better while preserving professional quality and human judgment.

## Long-Term Transformation Arc

1. Trust and AI literacy
2. One painful workflow improved
3. Repetition until habit
4. Reusable context
5. Complex work
6. Automation and agents

## Adoption Ladder

| Level | Name | Meaning |
|------|------|---------|
| 0 | Interested but dependent | Client likes the idea but needs guidance |
| 1 | Assisted success | Works with consultant present |
| 2 | Solo repetition | Client can repeat it alone a few times |
| 3 | Stable habit | Workflow becomes part of normal routine |
| 4 | Workflow redesign | Old process changes because AI is trusted |
| 5 | Automation readiness | Agent or automation can be considered safely |

Do not jump from Level 1 to Level 5.

## Session Design Principle

A good session is not the session where the consultant covers the most topics.

A good session is the session where the right next thing becomes clearer, lighter, and more repeatable.

## Do Not Overbuild

Do not add dashboards, agents, automations, files, or prompts simply because they are possible.

The right next step is usually the smallest step that creates relief, confidence, or repeated use.

Automation comes after clarity and habit.

## Human Tone

The AOTW consultant’s tone should be warm, direct, patient, honest, practical, calm when tools fail, serious about quality, and respectful of the client’s dignity.

Avoid hype, guilt, buzzwords, overpromising, tool overload, and making the client feel behind.

## Recommendation-Worthy Service

The client recommends the service when they feel remembered, understood, not judged, protected from complexity, helped on real work, safer with AI, and more confident after sessions.
```

---

## context/client-contact.md

```markdown
---
purpose: client-contact-lookup
updated: YYYY-MM-DD
---

# Client Contact and Lookup

## Canonical Identity

- Full name:
- Preferred name:
- Pronunciation:
- Company / organization:
- Role / title:
- Timezone:
- Primary language:
- Secondary languages:

## Contact Details

| Type | Value | Notes |
|------|-------|-------|
| Primary email | unknown | |
| Secondary email | unknown | |
| Assistant / scheduler email | unknown | |
| Phone / WhatsApp | unknown | |
| LinkedIn | unknown | |

## Calendar Lookup

- Primary search terms:
- Alternate search terms:
- Meeting title patterns:
- Known attendee emails:
- Standard session duration: 90 minutes unless Calendar or engagement file proves otherwise
- Standard cadence:
- Usual meeting platform:
- Scheduling notes:

## Gmail Lookup

- Email search query terms:
- Known aliases:
- Company domains:
- Stakeholder emails to include:
- Threads likely to matter:

## Repo / Internal Aliases

- Repo slug:
- Internal short name:
- Other aliases:

## Important Rule

Do not use the repo slug as the client name unless it is listed above as an alias.

## Unknowns To Confirm

-
```

---

## context/client-profile.md

```markdown
---
purpose: client-profile
updated: YYYY-MM-DD
---

# Client Profile: [Client Name]

## Identity

## Professional Role

## Responsibilities

## Business / Organizational Context

## Technology Environment

## Work Style and Pain Points

## Personality and Working Style

## AI Readiness

## Emotional / Trust Signals

## Health, Time, or Life Constraints

## Communication Style

## Notable Quotes

## Unknowns / Needs Confirmation
```

---

## context/engagement.md

```markdown
---
purpose: engagement-context
updated: YYYY-MM-DD
---

# Engagement: [Client Name]

## Deal Terms

Not captured yet.

## What Is Included

## Session Rhythm

- Standard session duration: 90 minutes unless Calendar or engagement terms prove otherwise.

## Support Channels

## Privacy and Data Access

## Timeline

## Known Promises

## Open Questions
```

---

## context/stakeholders.md

```markdown
---
purpose: stakeholders
updated: YYYY-MM-DD
---

# Stakeholders

## [Stakeholder Name or Group]

- **Role:**
- **Why they matter:**
- **Influence on AI adoption:**
- **Constraints / dependencies:**
- **Communication notes:**
```

---

## context/writing-style-profile.md

```markdown
---
purpose: writing-style-profile
updated: YYYY-MM-DD
confidence: low
---

# Writing Style Profile

## Current Confidence

low

## Overall Voice

Not enough evidence yet.

## What The Client Wants

## Phrases Or Patterns The Client Naturally Uses

## Phrases That Sound Too AI-Generated

## Tone By Situation

### Executive / Serious

### Warm Relationship

### Short Operational Reply

### Sensitive Or Difficult Message

## Words To Avoid

## Good Instruction Pattern

## Example Prompt

## Evidence Used

## Evidence Needed
```

---

## status/current-status.md

```markdown
---
purpose: current-status
updated: YYYY-MM-DD
last_session: unknown
next_session: unknown
---

# Current Status

This file is a current snapshot, not the full task database.

For full open commitments, see `status/action-registry.md`.

For adoption and value signals, see `status/outcomes-scorecard.md`.

## Active Right Now

## Blocked

## Planned

## Completed

## Next Session Time / Duration / Source

## Next Session Opener

## Latest Freshness Check

- Calendar checked:
- Gmail checked:
- Other tools checked:
- Newer information found:
```

---

## status/decisions-log.md

```markdown
---
purpose: decisions-log
updated: YYYY-MM-DD
---

# Decisions Log

## YYYY-MM-DD

- **Decision:**
  - Why:
  - Conditions:
  - Source:
```

---

## status/action-registry.md

```markdown
---
purpose: action-registry
updated: YYYY-MM-DD
---

# Action Registry

## Status Definitions

- **active** - should be worked on soon
- **waiting** - blocked by client, stakeholder, admin, tool, or outside dependency
- **parked** - real idea, but not useful right now
- **done** - completed
- **superseded** - replaced by a newer decision or workflow

## Active Actions

| ID | Owner | Action | Source | Workstream | Status | Next review | Notes |
|----|-------|--------|--------|------------|--------|-------------|-------|

## Waiting / Blocked

| ID | Owner | Action | Blocker | Source | Next move |
|----|-------|--------|---------|--------|-----------|

## Parked

| ID | Idea | Why parked | Revisit when |
|----|------|------------|--------------|

## Done Recently

| ID | Completed action | Date | Evidence |
|----|------------------|------|----------|

## Superseded

| ID | Old action | Superseded by | Date |
|----|------------|---------------|------|
```

---

## status/outcomes-scorecard.md

```markdown
---
purpose: outcomes-scorecard
updated: YYYY-MM-DD
---

# Outcomes Scorecard

## North Star Outcome

The client uses AI to reduce work complexity and time while preserving or improving professional quality, human style, and trust.

## Current Outcome Signals

| Area | Baseline / old state | Current signal | Target direction | Evidence | Confidence |
|------|----------------------|----------------|------------------|----------|------------|

## Latest Wins

## Latest Frictions

## Adoption Level By Workflow

| Workflow | Adoption level | Evidence | Next step |
|----------|----------------|----------|-----------|

## Next Measurable Experiment

- Experiment:
- Success looks like:
- Evidence to capture:
```

---

## status/practice-plan.md

```markdown
---
purpose: client-practice-plan
updated: YYYY-MM-DD
---

# Client Practice Plan

## Current Tiny Practice

- Practice:
- Why this matters:
- Fallback if too heavy:
- Evidence to bring next time:
- Consultant framing:

## Previous Practice Checks

| Date | Practice | Completed? | Evidence | Friction |
|------|----------|------------|----------|----------|
```

---

## status/service-retrospective-log.md

```markdown
---
purpose: internal-service-retrospective-log
updated: YYYY-MM-DD
visibility: internal
---

# Service Retrospective Log

This file captures internal AOTW delivery lessons from client sessions.

Do not use this as a client-facing report.

## Entries

No retrospective entries yet.
```

---

## tools/tool-stack.md

```markdown
---
purpose: tool-stack
updated: YYYY-MM-DD
---

# Tool Stack

## Status Definitions

- **active** - use now
- **fallback** - use if active path fails
- **blocked** - wanted but blocked by access, license, admin, or policy
- **parked** - not useful right now
- **experimental** - test only in controlled situations
- **retired** - replaced by a better workflow

## Current Tool Roles

| Tool | Status | Use for | Do not use for | Current blocker / risk | Notes |
|------|--------|---------|----------------|------------------------|-------|

## Current Tool Decision
```

---

## privacy/data-boundaries.md

```markdown
---
purpose: data-boundaries
updated: YYYY-MM-DD
---

# Data Boundaries

## Core Rule

Do not move client or organizational data into a tool, notebook, video, demo, public example, or external workflow unless the boundary is understood and the use is appropriate.

## Current Consent / Known Boundaries

| Data type | Can be stored in repo? | Can be used in AI tools? | Client-facing safe? | Notes |
|----------|------------------------|--------------------------|---------------------|-------|

## Tool-Specific Notes

## Client-Facing Safety Rule

Before producing anything client-facing, remove:

- internal service strategy
- pricing
- referral strategy
- sensitive personal details
- raw transcript content
- private emotional notes
- third-party sensitive names
- consultant self-critique

## Client-Safe Explanation
```

---

## Workstream Template

```markdown
---
purpose: workstream-tracker
status: active
updated: YYYY-MM-DD
---

# [Workstream Name]

## Problem Statement

## Current State

## Goal

## Technical Notes

## Next Smallest Action

- **Action:**
- **Why now:**
- **Success evidence:**

## Open Items

## Related Sessions
```

---

## Session Template

```markdown
---
date: YYYY-MM-DD
duration: approximate
attendees: []
topics: []
source: attached-source
---

# Session: YYYY-MM-DD

## Summary

## Key Discussion Points

## Decisions Made

## Action Items

## Open Questions

## Mood And Dynamics

## Quotes Worth Preserving
```
