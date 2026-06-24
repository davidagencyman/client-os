# AOTW Client OS Blueprint v4 - Complete Single-File Edition

This single Markdown file contains the full reusable blueprint package, including the master build instruction, research principles, core file templates, and every complete skill body. It is generated from `outputs/aotw-client-os-blueprint-v4/`.

Use this file when you want to attach one complete instruction file to Codex, Claude Code, or another AI coding agent. If using the folder package instead, preserve the same file structure.


---

## Included File: `outputs/aotw-client-os-blueprint-v4/README.md`

````markdown
---
title: AOTW Client OS Blueprint v4
purpose: package-readme
version: 4.0
updated: 2026-06-19
---

# AOTW Client OS Blueprint v4

This package is the reusable blueprint for building a new Ahead of the Wave AI client operating repository from zero.

Use it with Codex, Claude Code, or another capable AI coding agent.

## What This Package Contains

```text
MASTER-BLUEPRINT.md          Main instruction for creating a new client repo
skills/                      Complete skill files to copy into the new repo
templates/core-files.md      Templates for required repo files
references/research-principles.md  Research-backed design principles and sources
```

## How To Use

Give the AI agent:

1. `MASTER-BLUEPRINT.md`
2. the entire `skills/` folder
3. `templates/core-files.md`
4. the discovery transcript or source material as a direct attachment
5. access to connected tools if available, especially Calendar and Gmail

Do not require a repo `_inbox/` folder. Source material should be attached directly to the AI agent.

## Important v4 Rule

This package includes 17 full skill bodies.

Do not let the AI agent invent new skill instructions when building a client repo. It should copy or adapt the complete skill files in this package, changing only client-specific names, paths, and evidence.

## Default Workflow

When source material is attached, the new client repo should start from:

1. `_skills/operating-router.md`
2. `_skills/process-source-material.md`
3. follow-on skills chosen by the router

When preparing a session:

1. Read `context/client-contact.md`
2. Check Calendar first
3. Check Gmail second
4. Run `_skills/call-prep.md`
5. Prepare for 90 minutes unless Calendar or engagement terms prove another duration

## Package Quality Target

This package should make the generated repo:

- less random
- less tool-obsessed
- more humane
- more accurate with connected tools
- stronger at deciding which skill to run
- better at preserving client trust, context, and adoption evidence
````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/MASTER-BLUEPRINT.md`

````markdown
---
title: AOTW Client OS Master Blueprint
purpose: reusable-build-instruction
audience: Ahead of the Wave AI team and AI coding agents
version: 4.0
updated: 2026-06-19
---

# AOTW Client OS Master Blueprint

## Use This File With The v4 Package

This master blueprint must be used together with:

- `skills/`
- `templates/core-files.md`
- `references/research-principles.md`
- any attached client source material

The AI agent must not invent skill bodies. It should copy the complete skill files from the `skills/` folder into the generated client repo.

## Objective

Build a new private AI-readable operating repository for an Ahead of the Wave AI client engagement.

The repository is not a normal codebase.

It is a consulting operating system. It stores client context, session history, action commitments, decisions, workstreams, adoption evidence, tool status, privacy boundaries, and session-preparation logic.

The repository should help an AOTW consultant and future AI agents:

- understand the client deeply
- prepare humane and focused sessions
- process attached transcripts and notes
- decide which internal skills to run
- preserve the client’s real language and working context
- track promises and blockers
- measure adoption rather than demos
- prevent tool overload
- protect privacy and trust
- generate useful follow-ups and learning assets

## Core Philosophy

AI should adapt to the client’s work, language, responsibilities, standards, and human style.

The client should not feel forced to become an "AI person" or reorganize their life around tools.

The service is successful when the client becomes calmer, more capable, more independent, and more confident while preserving quality, judgment, privacy, trust, and human relationships.

## Required Repo Structure

Create:

```text
README.md
CLAUDE.md
_skills/
context/
status/
workstreams/
sessions/
method/
tools/
privacy/
research/
learning/
client-facing/
playbooks/
templates/
```

Do not create `_inbox/` as a required workflow folder.

Source material should be attached directly to Codex, Claude Code, or the AI agent and processed through `_skills/process-source-material.md`.

## Required Core Files

Create:

```text
README.md
CLAUDE.md

method/personal-ai-upgrade-method.md

context/client-contact.md
context/client-profile.md
context/engagement.md
context/stakeholders.md
context/writing-style-profile.md

status/current-status.md
status/decisions-log.md
status/action-registry.md
status/outcomes-scorecard.md
status/practice-plan.md
status/service-retrospective-log.md

tools/tool-stack.md
privacy/data-boundaries.md

playbooks/personal-ai-upgrade-playbook.md
templates/new-client-repo-template.md
```

Copy every file in this package’s `skills/` folder into the generated repo’s `_skills/` folder.

## Required Skill Files

The generated repo must include these complete skills:

```text
_skills/operating-router.md
_skills/process-source-material.md
_skills/call-prep.md
_skills/follow-up-email.md
_skills/action-registry-maintainer.md
_skills/outcome-scorecard.md
_skills/client-practice-plan.md
_skills/tool-stack-governor.md
_skills/privacy-boundary-check.md
_skills/session-retrospective.md
_skills/learning-bundle-builder.md
_skills/notebooklm-video-builder.md
_skills/technical-research-brief.md
_skills/workstream-pruner.md
_skills/client-style-profile-builder.md
_skills/monthly-progress-report.md
_skills/service-ip-extractor.md
```

Do not replace these with short summaries.

## Direct-Attachment Workflow

When the AOTW team member attaches a discovery call transcript, session transcript, notes, or email/document source:

1. Start with `_skills/operating-router.md`.
2. The router decides which skills to run.
3. For transcripts and source material, the router runs `_skills/process-source-material.md`.
4. Follow-on skills run only when useful.
5. The agent updates repo files directly.
6. The agent reports what it ran and why.

## Connected Tool Freshness

When connected tools are available and relevant:

1. Check Calendar first.
2. Check Gmail second.
3. Check other connected tools third only when useful.

Always read `context/client-contact.md` before searching connected tools.

Never infer the client’s name from the repo slug unless `context/client-contact.md` lists it as an alias.

## Standard Session Duration

The default AOTW one-on-one session length is 90 minutes.

Call prep must produce a realistic 90-minute session strategy brief unless Calendar or `context/engagement.md` proves a different duration.

## Required Reading Order for General Orientation

1. `README.md`
2. `CLAUDE.md`
3. `_skills/operating-router.md`
4. `method/personal-ai-upgrade-method.md`
5. `context/client-contact.md`
6. `context/client-profile.md`
7. `context/engagement.md`
8. `context/stakeholders.md`
9. `status/current-status.md`
10. `status/action-registry.md`
11. `status/outcomes-scorecard.md`
12. `tools/tool-stack.md`
13. `privacy/data-boundaries.md`
14. relevant workstreams and sessions

## Usefulness Test

Before adding anything, ask:

1. Who will use this?
2. When will it be used?
3. What decision, preparation, or client outcome does it improve?
4. Does another file already do this?
5. Will this reduce complexity or add complexity?
6. Will this help the next session?
7. Will this help long-term client transformation?
8. Will this preserve trust and humane delivery?
9. Will this prevent forgotten promises, overload, or shiny-tool chasing?
10. Is this practical enough that an AOTW consultant or AI agent will actually use it?

If the answer is weak, do not add it.

## Build Steps

1. Create the folder structure.
2. Create the core files from `templates/core-files.md`.
3. Copy all complete skill files from `skills/`.
4. If source material is attached, run `_skills/operating-router.md`.
5. If the attached source is a discovery call, create a discovery session file and initial context files.
6. Create concrete workstreams only when evidence supports them.
7. Create `context/client-contact.md` before any Calendar or Gmail search.
8. Populate `status/current-status.md`, `status/action-registry.md`, `status/outcomes-scorecard.md`, `status/practice-plan.md`, `tools/tool-stack.md`, and `privacy/data-boundaries.md`.
9. Run the quality gate.
10. Report the build result.

## Quality Gate

Before finishing, verify that the repo can answer:

- Who is the client?
- What is the canonical client contact and lookup information?
- What Calendar/Gmail search terms should be used?
- What does the client actually do?
- What is painful right now?
- What is emotionally sensitive?
- What tools are active, blocked, parked, or experimental?
- What did the AOTW team promise?
- What did the client promise?
- What has actually changed?
- What is only an idea?
- What should the next session focus on?
- How long is the next session and what source proves it?
- What should not be opened yet?
- What is the next tiny practice step?
- What data is safe to use?
- Which skills should run for the current situation?

Also verify:

- `_skills/operating-router.md` exists.
- `_skills/process-source-material.md` exists.
- all required skills exist with full bodies.
- no `_inbox/` folder is required.
- attached transcripts are routed through `process-source-material.md`.
- Calendar is checked before Gmail when available.
- call prep defaults to 90 minutes unless proven otherwise.

## Final Report

After building the repo, report:

```markdown
# New Client Repo Build Report

## Files created

## Source material used

## Connected tools checked

## Operating router decisions

## Skills run automatically

## Client contact / lookup summary

## Client profile summary

## Main pain points identified

## Recommended first workstreams

## Current actions

## Blockers

## Privacy concerns

## Suggested next session focus

## Session duration used and source

## Suggested tiny practice step

## What was deliberately not added

## Smoke test result
```

Do not say the repo is complete forever. Say it is ready for the next consulting step.
````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/references/research-principles.md`

````markdown
---
title: Research Principles for AOTW Client OS Repos
purpose: research-backed-design-notes
version: 4.0
updated: 2026-06-19
---

# Research Principles

This note records the design principles behind the v4 blueprint.

It is not client-facing. It helps the AOTW team and AI agents understand why the package is structured the way it is.

## Sources Used

- LangGraph workflows and agents: https://docs.langchain.com/oss/python/langgraph/workflows-agents
- OpenAI Agents SDK handoffs: https://openai.github.io/openai-agents-python/handoffs/
- OpenAI prompt engineering guide: https://developers.openai.com/api/docs/guides/prompt-engineering
- OpenAI reasoning best practices: https://developers.openai.com/api/docs/guides/reasoning-best-practices
- Claude Code skills: https://code.claude.com/docs/en/skills
- Claude Code subagents: https://code.claude.com/docs/en/sub-agents
- Anthropic prompt engineering best practices: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices
- Anthropic Agent Skills article: https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills
- Anthropic context engineering for agents: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- Google People + AI Guidebook: https://pair.withgoogle.com/guidebook/

## Design Conclusions

### 1. Use a Router, Not Manual Skill Guessing

Modern agent systems use routing, handoffs, or orchestrator-worker patterns.

For this repo system, the practical equivalent is `_skills/operating-router.md`.

The router:

- classifies the situation
- decides which skills to run
- runs the minimum useful cascade
- explains what it ran and why

This avoids requiring the AOTW team member to say "run process, then follow-up, then update action registry."

### 2. Use Complete Skill Files, Not Skill Names

Claude skills and agent skill systems work best when procedural knowledge is packaged as explicit instructions and resources.

Therefore, the blueprint must include full skill bodies. A generated repo should not ask the model to invent skill instructions.

### 3. Separate Operating Memory From Source Material

The old `_inbox/` pattern forced an unnecessary manual step: upload transcript into the repo, then run a skill.

The better workflow is:

- attach transcript directly to Codex or Claude Code
- let the router classify it
- run `process-source-material`
- write structured repo memory

### 4. Check Live Context Before Preparing

Calendar and Gmail often contain newer truth than the repo.

Any session prep should:

1. read `context/client-contact.md`
2. check Calendar
3. check Gmail
4. reconcile with repo state

This prevents wrong names, wrong meeting duration, stale agendas, and missed client updates.

### 5. Make Human Tone an Operating Requirement

The system should not produce dry consulting agendas.

It should infer:

- emotional state
- trust level
- frustration
- confidence
- overwhelm risk
- how the client should feel by the end

The call prep output should protect the client from overload and create one clear adoption step.

### 6. Track Adoption, Not Demos

A tool working during a session is not adoption.

The repo must distinguish:

- built with consultant
- used alone by client
- not yet habitual
- blocked by tool
- blocked by behavior
- ready for automation
- not ready for automation

### 7. Treat Privacy as a First-Class Workflow

Privacy checks should not be afterthoughts.

Any sharing, NotebookLM source, client-facing artifact, new connector, sensitive transcript, or public example should trigger `_skills/privacy-boundary-check.md`.

### 8. Keep Session Duration Explicit

AOTW one-on-one sessions default to 90 minutes.

Call prep should not silently produce a 30-minute agenda unless Calendar or engagement terms prove the session is shorter.

### 9. Make Output Verifiable

Each skill should say:

- what it read
- what it changed
- what it skipped
- what needs attention

This makes the system auditable and easier to improve.

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/templates/core-files.md`

````markdown
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
````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/operating-router.md`

````markdown
---
purpose: default-entry-skill-and-skill-router
updated: 2026-06-19
trigger: Run first for any unclear request, attached transcript, new source material, prep request, repo update request, or general "what should we do next" request.
---

# Operating Router

## Purpose

This is the default thinking layer for the client operating repository.

Use it whenever the agent is not already executing one clearly named skill.

Its job is to decide what the current situation is, which source material matters, which files need to be read, which skills should run, and what should deliberately be skipped.

The router prevents random skill use, over-processing, and shallow updates.

## Core Principle

Run the smallest useful chain of skills that improves the next consulting decision, client session, client follow-up, client learning asset, or long-term operating record.

Do not run every skill because a transcript exists.

Do not skip a necessary skill because the user did not name it.

## Inputs

The current request may include:

- a discovery call transcript
- a session transcript
- meeting notes
- email content
- client documents
- screenshots
- a request to prepare for a call
- a request to write a follow-up
- a request to clean the repo
- a request to build a new repo
- a vague instruction such as "process this", "update the repo", or "what should we do next"

Treat attached source material as live input.

Do not require a repo `_inbox/` folder.

## Required First Read

If the repo already exists, read in this order:

1. `README.md`
2. `CLAUDE.md`
3. `context/client-contact.md`
4. `context/client-profile.md`
5. `context/engagement.md`
6. `status/current-status.md`
7. `status/action-registry.md`
8. `status/outcomes-scorecard.md`
9. `tools/tool-stack.md`
10. `privacy/data-boundaries.md`

Then read only the relevant sessions, workstreams, research, learning files, or client-facing files needed for the current request.

If the repo does not exist yet, use the master blueprint and templates to create the baseline before processing source material.

## Connected Tool Freshness

When the request involves a session, follow-up, current client status, recent communication, or upcoming meeting:

1. Read `context/client-contact.md`.
2. Check Calendar first if available.
3. Check Gmail second if available.
4. Check other connected tools only when they are clearly relevant.

Use the canonical client name, email, company, aliases, and meeting titles from `context/client-contact.md`.

Do not infer the client identity from the repo folder name.

If connected tools are unavailable, say so in the router report and continue from repo evidence and attached source material.

## Classification

Classify the request into one or more of these situations.

### New Source Material

Examples:

- "Process this transcript"
- "Here is the discovery call"
- "Update the repo from this"
- attached notes without a specific output request

Run:

1. `process-source-material.md`
2. `action-registry-maintainer.md` if commitments, asks, blockers, or next steps are present
3. `outcome-scorecard.md` if behavior change, adoption, value evidence, or success signals are present
4. `tool-stack-governor.md` if tools, platforms, automations, integrations, or access issues are mentioned
5. `client-practice-plan.md` if the client needs a tiny next practice step
6. `privacy-boundary-check.md` if sensitive data, sharing, recording, public examples, or third-party tools are involved
7. `session-retrospective.md` if the material reflects a client session
8. `service-ip-extractor.md` if reusable AOTW method patterns appear

### Discovery Call

Run:

1. `process-source-material.md`
2. `client-style-profile-builder.md`
3. `action-registry-maintainer.md`
4. `tool-stack-governor.md`
5. `outcome-scorecard.md`
6. `client-practice-plan.md`
7. `service-ip-extractor.md`

Create an initial session file and initial context/status records.

Do not create too many workstreams. Create only workstreams supported by strong evidence.

### Session Preparation

Examples:

- "Prep me for tomorrow"
- "What should we do on the call?"
- "Make a session brief"

Run:

1. connected tool freshness checks
2. `call-prep.md`
3. `technical-research-brief.md` only for volatile tool questions or unknown technical blockers
4. `workstream-pruner.md` if the repo has too many competing active threads

Default session length is 90 minutes unless Calendar or `context/engagement.md` proves otherwise.

### Follow-Up Email

Examples:

- "Write the follow-up"
- "Send recap"
- "Draft the client email"

Run:

1. connected tool freshness checks
2. `follow-up-email.md`
3. `privacy-boundary-check.md` if the follow-up includes sensitive details, tool screenshots, client data, or third-party sharing
4. `action-registry-maintainer.md` if new commitments are created or clarified

### Learning Asset

Examples:

- "Make a quick guide"
- "Create a practice doc"
- "Turn this into training"
- "Build a NotebookLM source pack"

Run:

1. `learning-bundle-builder.md`
2. `privacy-boundary-check.md`
3. `notebooklm-video-builder.md` only if the requested output specifically involves NotebookLM, audio/video overview, or a source pack for NotebookLM

### Technical Research

Examples:

- "Find how this tool works now"
- "Check current API limits"
- "Research best way to automate this"

Run:

1. `technical-research-brief.md`
2. `privacy-boundary-check.md` if the researched workflow touches client data or third-party services
3. `tool-stack-governor.md` if the research changes the recommended tool stack

Use current web research for volatile tools, APIs, pricing, limits, policies, or product behavior.

### Repo Hygiene

Examples:

- "Clean this up"
- "Prune old workstreams"
- "Make it less confusing"

Run:

1. `workstream-pruner.md`
2. `action-registry-maintainer.md`
3. `tool-stack-governor.md`
4. `outcome-scorecard.md` if status changed

### Monthly Or Executive Update

Examples:

- "Make the monthly report"
- "What changed this month?"
- "Send a client progress summary"

Run:

1. `monthly-progress-report.md`
2. `outcome-scorecard.md`
3. `privacy-boundary-check.md`

## Skill Cascade Rules

Use these rules when more than one skill might apply:

- Run `process-source-material.md` before any skill that depends on newly attached transcript or notes.
- Run `privacy-boundary-check.md` before producing client-facing, shareable, public, or third-party-upload material.
- Run `action-registry-maintainer.md` whenever there are promises, owners, blockers, or next steps.
- Run `tool-stack-governor.md` whenever tools are introduced, recommended, blocked, retired, or causing overload.
- Run `outcome-scorecard.md` whenever there is evidence of changed behavior, adoption, confidence, cycle time, quality, or business value.
- Run `client-practice-plan.md` whenever the client needs a small behavior step between sessions.
- Run `technical-research-brief.md` when correctness depends on current product behavior or external facts.
- Run `service-ip-extractor.md` when a repeatable AOTW delivery pattern appears.

## What To Avoid

Do not:

- run all skills by default
- create workstreams for every idea
- create action items from vague curiosity
- overstate client adoption from excitement alone
- turn private client language into public examples
- produce a long follow-up email when a short one will do
- open sensitive tools or documents unless the current task requires them
- use client-facing language before checking privacy boundaries
- overwrite client style with generic AI language

## Router Output

At the start of work, produce a short internal routing note in chat or in the agent's working log:

```markdown
# Operating Router Report

## Situation Classified As

## Source Material Detected

## Files Read First

## Connected Tools Checked

## Skills To Run

## Skills Deliberately Skipped

## Main Risk To Watch

## Expected Repo Updates
```

Keep this report short unless the user asked for a full audit.

## Completion Report

When done, report:

- what source material was processed
- what files changed
- which skills were run
- which skills were skipped and why
- any connected tools checked
- remaining uncertainty
- the next useful consulting step

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/process-source-material.md`

````markdown
---
purpose: process-directly-attached-transcripts-notes-and-source-material
updated: 2026-06-19
trigger: Run when discovery calls, session transcripts, notes, email excerpts, documents, screenshots, or other source materials are attached directly to the AI agent.
---

# Process Source Material

## Purpose

Turn directly attached source material into durable client operating context.

This skill replaces any workflow that requires source material to be placed in an `_inbox/` folder.

The agent should read the attachment, classify it, extract useful evidence, update the right repo files, and trigger follow-on skills only when useful.

## Core Principle

The transcript or source is evidence, not a dumping ground.

Extract decisions, constraints, tone, client language, commitments, risks, opportunities, and repeatable patterns.

Do not turn every sentence into a file update.

## Inputs

Possible source types:

- discovery call transcript
- recurring session transcript
- internal AOTW notes
- client email or message thread
- client document
- screenshot or screen recording notes
- tool export
- stakeholder notes
- implementation notes
- research notes

If the user supplies several attachments, process them in chronological order when dates are known. If dates are unknown, process discovery or strategy material first, then implementation/session material, then follow-up or reference material.

## Required First Read

Before extracting, read:

1. `context/client-contact.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `context/stakeholders.md`
5. `status/current-status.md`
6. `status/action-registry.md`
7. `tools/tool-stack.md`
8. `privacy/data-boundaries.md`
9. relevant recent `sessions/` files
10. relevant active `workstreams/` files

If these files do not exist yet, create them from the blueprint templates before processing.

## Source Classification

Classify the source as one or more of:

- discovery
- strategy
- session
- implementation
- troubleshooting
- client-facing communication
- internal AOTW note
- tool or workflow evidence
- stakeholder or buying context
- privacy-sensitive material
- reusable service IP

Use the classification to choose what to update.

## Extraction Targets

### Client Identity And Lookup

Update `context/client-contact.md` when the source gives:

- canonical client name
- company or organization
- role or title
- email
- phone if relevant
- meeting title patterns
- spelling variants
- aliases
- assistant or stakeholder names
- Calendar/Gmail search hints

Never infer canonical identity from the repo slug.

Mark uncertain fields as `Unknown` or `Needs confirmation`.

### Client Profile

Update `context/client-profile.md` when the source gives:

- what the client does
- what quality standards matter
- what work feels expensive, slow, repetitive, or emotionally loaded
- what the client is already good at
- where AI could help
- where AI could damage trust or quality
- client language worth preserving
- decision style
- learning style
- constraints and preferences

### Engagement

Update `context/engagement.md` when the source gives:

- service scope
- session cadence
- session duration
- intended outcomes
- stakeholders
- working agreements
- boundaries
- success criteria
- known calendar rhythm

If no duration is stated, keep the default one-on-one prep assumption at 90 minutes.

### Stakeholders

Update `context/stakeholders.md` when the source gives:

- direct client contact
- internal team members
- assistant or operator
- decision maker
- influencer
- user of the AI-enabled workflow
- sensitive relationship
- communication preferences

### Current Status

Update `status/current-status.md` with:

- current reality
- active priorities
- open blockers
- risks
- recently completed work
- what changed since the last session
- next session focus candidate

### Decisions

Update `status/decisions-log.md` with actual decisions only.

A decision needs evidence such as:

- "we decided"
- "let's use"
- "we will not"
- "the plan is"
- a clear acceptance or rejection

Do not log brainstorming as a decision.

### Actions

Extract commitments into `status/action-registry.md` through `action-registry-maintainer.md`.

Action candidates include:

- AOTW promised to send, build, research, prepare, connect, or review something
- client promised to share, test, practice, approve, or introduce something
- a blocker needs ownership
- a question needs an answer
- a follow-up is time sensitive

### Workstreams

Create or update `workstreams/` only when the source shows a durable thread of work.

A workstream should have:

- a clear outcome
- a client value reason
- at least one concrete next step
- evidence that it matters beyond one passing idea

Do not create workstreams for every possible automation.

### Sessions

For discovery or session transcripts, create a session note:

```text
sessions/YYYY-MM-DD-[session-type].md
```

Include:

- date
- source type
- participants if known
- purpose
- summary
- important client language
- decisions
- commitments
- blockers
- emotional or relationship signals
- suggested follow-on skills

If the date is unknown, use `sessions/undated-[source-type]-[short-topic].md` and mark the date as unknown.

### Tools

Send tool-related findings to `tool-stack-governor.md` when the source mentions:

- ChatGPT
- Claude
- Gemini
- NotebookLM
- Zapier
- Make
- CRM
- email
- calendar
- document systems
- spreadsheets
- project management
- databases
- custom apps
- browser extensions
- automation platforms
- access issues
- permissions
- integration failures

### Privacy

Send privacy-sensitive findings to `privacy-boundary-check.md` when the source includes:

- personal data
- medical, legal, financial, HR, or employment information
- passwords, credentials, private links, customer data, or proprietary material
- public examples
- third-party tool uploads
- training material using client details
- screenshots or recordings
- confidential stakeholder dynamics

### Outcomes

Send adoption and value evidence to `outcome-scorecard.md` when the source shows:

- client used a workflow independently
- client changed behavior between sessions
- time saved
- quality improved
- stress reduced
- client confidence increased
- avoided risk
- faster drafting, research, analysis, or decision making
- a workflow moved from demo to actual use

Do not count excitement as adoption.

### Practice

Send practice candidates to `client-practice-plan.md` when the source suggests the client should try:

- one tiny prompt
- one repeated behavior
- one workflow in a real task
- one review habit
- one safe experiment

### Style

Send communication examples to `client-style-profile-builder.md` when the source includes:

- client-written emails
- client phrases
- preferred tone
- words to avoid
- examples of how the client gives instructions
- examples of how the client responds to polished or unpolished language

### Reusable AOTW IP

Send reusable service patterns to `service-ip-extractor.md` when the source shows:

- a repeatable consulting move
- a diagnostic question
- a coaching pattern
- a useful prompt architecture
- a client objection pattern
- a risk pattern
- a durable playbook fragment

Remove or generalize private client details before adding to playbooks.

## Required Output

After processing, report:

```markdown
# Source Material Processing Report

## Source Material

## Classification

## Files Created

## Files Updated

## Key Evidence Captured

## Decisions Found

## Actions Found

## Workstreams Created Or Updated

## Tool Stack Signals

## Privacy Signals

## Outcome Signals

## Follow-On Skills Run

## Follow-On Skills Recommended But Not Run

## Uncertainties
```

## Quality Rules

Do:

- preserve client language
- distinguish evidence from inference
- mark uncertainty clearly
- use dates when available
- avoid generic AI consulting language
- keep files useful for future prep
- create fewer, better workstreams
- keep private material out of public or client-facing summaries

Do not:

- require an `_inbox/` folder
- quote huge transcript sections
- create fake precision
- invent missing email addresses
- infer identity from folder names
- turn every idea into an action
- treat a demo as adoption
- expose sensitive details in client-facing outputs

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/call-prep.md`

````markdown
---
purpose: prepare-a-humane-high-leverage-client-session
updated: 2026-06-19
trigger: Run when preparing for an upcoming client call, session, check-in, workshop, or renewal conversation.
---

# Call Prep

## Purpose

Create a session strategy brief that helps the AOTW consultant run a focused, humane, useful client session.

The brief should connect long-term transformation, current client reality, recent communications, active commitments, and the next smallest useful move.

## Default Duration

Assume a standard AOTW one-on-one session is 90 minutes unless Calendar or `context/engagement.md` proves a different duration.

If the duration is uncertain, build a 90-minute plan and state that the duration was assumed.

## Connected Tool Freshness

Before writing the brief, when connected tools are available:

1. Read `context/client-contact.md`.
2. Check Calendar first for upcoming meeting date, time, title, guests, attachments, and duration.
3. Check Gmail second for recent client communication, unreturned asks, promised materials, scheduling changes, or tone shifts.
4. Check other connected tools only if they are clearly tied to the session.

Use canonical names, emails, company names, aliases, and meeting title patterns from `context/client-contact.md`.

Do not infer the client from the repo slug.

If tools are unavailable, state that in the freshness section and continue from repo evidence.

## Required Read

Read:

1. `context/client-contact.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `context/stakeholders.md`
5. `context/writing-style-profile.md`
6. `status/current-status.md`
7. `status/action-registry.md`
8. `status/outcomes-scorecard.md`
9. `status/practice-plan.md`
10. `tools/tool-stack.md`
11. `privacy/data-boundaries.md`
12. recent `sessions/`
13. active `workstreams/`
14. relevant `research/` or `learning/` files

## Strategy Rules

A good session brief should answer:

- What is the long-term arc of this client engagement?
- What changed since the last session?
- What did AOTW promise?
- What did the client promise?
- What is stuck?
- What should not be opened yet?
- What is the highest leverage focus for this session?
- What will make the client feel seen and not overwhelmed?
- What small practice step would create real adoption?
- What needs research before the call?
- What privacy or trust boundary matters?

## Focus Selection

Choose one primary session focus.

Choose at most two secondary threads.

Use this ranking:

1. time-sensitive client commitment
2. trust or privacy risk
3. blocker preventing adoption
4. workflow the client is likely to use this week
5. high-value but contained automation or assistant behavior
6. long-term capability building
7. interesting research or tool exploration

If there are too many active threads, recommend running `workstream-pruner.md`.

## 90-Minute Session Shape

For a normal 90-minute session, use a realistic structure:

- 0 to 10 minutes: reconnect, confirm what changed, surface urgent context
- 10 to 20 minutes: close loops from prior commitments
- 20 to 60 minutes: main working block
- 60 to 75 minutes: apply it to one real client task
- 75 to 85 minutes: decide next tiny practice and ownership
- 85 to 90 minutes: recap, confirm follow-up, leave calm

Adjust this only when the client context demands it.

Do not make a packed agenda that cannot fit.

## Tone

The brief is for the AOTW consultant, not for the client.

Use direct, practical language.

Keep the client human. Include stress, confidence, trust, and working style where relevant.

Avoid hype, generic AI transformation language, and long lists of possible tools.

## Output

Create or update a prep file:

```text
sessions/YYYY-MM-DD-call-prep.md
```

If the call date is unknown, use:

```text
sessions/next-call-prep.md
```

Use this structure:

```markdown
# Session Strategy Brief - [Client / Date]

## Freshness Check

## Session Duration

## Read First

## Long-Term Arc

## Current Client State

## What Changed Since Last Session

## AOTW Commitments To Close

## Client Commitments Or Open Asks

## Main Session Focus

## Secondary Threads

## Do Not Open Unless Necessary

## Suggested 90-Minute Flow

## Questions To Ask

## Things To Show Or Build

## Tiny Practice Step

## Follow-Up To Prepare

## Privacy Or Trust Watchouts

## Research Needed Before Call

## Desired Impression To Leave
```

## Freshness Check Wording

Be specific:

- Calendar checked: yes/no/unavailable
- Gmail checked: yes/no/unavailable
- meeting duration found: exact duration or assumed 90 minutes
- most recent relevant email date if available
- source files used

## Do Not Do

Do not:

- prepare a generic agenda
- assume a 30-minute call unless evidence says so
- ignore unreturned email asks
- ignore open AOTW commitments
- fill the call with tool demos
- suggest too many parallel experiments
- use client-facing language without checking privacy and tone
- create research claims without current verification when product behavior may have changed

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/follow-up-email.md`

````markdown
---
purpose: draft-client-follow-up-emails-after-sessions
updated: 2026-06-19
trigger: Run after a session, transcript, client meeting, or explicit request to write a follow-up email.
---

# Follow-Up Email

## Purpose

Write a concise, human client follow-up that confirms what happened, what matters next, and what each side owns.

The email should sound like a thoughtful consultant, not an automated meeting summary.

## Connected Tool Freshness

When available and relevant:

1. Read `context/client-contact.md`.
2. Check Calendar first to confirm the meeting date, title, attendees, and duration.
3. Check Gmail second for recent related communication, promised files, tone, and open loops.

If connected tools are unavailable, state that internally and proceed from repo evidence and supplied source material.

## Required Read

Read:

1. `context/client-contact.md`
2. `context/client-profile.md`
3. `context/writing-style-profile.md`
4. `status/current-status.md`
5. `status/action-registry.md`
6. `status/practice-plan.md`
7. latest relevant `sessions/`
8. relevant `workstreams/`
9. `privacy/data-boundaries.md`

Run `privacy-boundary-check.md` before including:

- sensitive personal details
- private stakeholder dynamics
- client data
- screenshots
- links to tools with private content
- third-party uploads
- public examples

## Email Strategy

A good follow-up should:

- be short enough to actually read
- confirm the one or two most important decisions
- name AOTW commitments plainly
- name client next steps lightly
- include one tiny practice step when useful
- avoid guilt or homework overload
- avoid generic enthusiasm
- preserve client trust
- make the next session easier

## Style Rules

Use:

- warm direct language
- short paragraphs
- clear ownership
- specific next steps
- client vocabulary where natural

Avoid:

- "as discussed" overload
- "exciting", "transformative", or hype language
- long bullet lists
- excessive recap
- invented deadlines
- sending the client internal strategy or sensitive assessment

## Output

Unless the user requests a file, output the draft in chat.

If a file is requested, create:

```text
client-facing/follow-up-YYYY-MM-DD.md
```

Use this structure internally:

```markdown
# Follow-Up Email Draft - [Date]

## Source Used

## Privacy Check

## Draft

Subject: [subject]

[email body]

## Commitments Captured

## Optional Shorter Version
```

The actual email body should not include the internal headings.

## Commitment Handling

After drafting, update or recommend updating `status/action-registry.md` when the email creates, changes, closes, or clarifies commitments.

## Quality Check

Before finalizing, verify:

- no sensitive internal notes leaked
- no action owner is ambiguous
- no unsupported claim was made
- the email does not make the client feel behind
- the tone matches the client relationship
- the next step is small and concrete

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/action-registry-maintainer.md`

````markdown
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

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/outcome-scorecard.md`

````markdown
---
purpose: track-client-adoption-value-and-behavior-change
updated: 2026-06-19
trigger: Run when source material shows client progress, adoption, business impact, reduced friction, confidence change, workflow usage, or when producing progress reports.
---

# Outcome Scorecard

## Purpose

Maintain `status/outcomes-scorecard.md` as the evidence record for whether the engagement is working.

The scorecard should track actual client adoption and value, not demos, intentions, or hype.

## Required Read

Read:

1. `status/outcomes-scorecard.md`
2. `status/current-status.md`
3. latest relevant `sessions/`
4. active `workstreams/`
5. `status/action-registry.md`
6. `context/client-profile.md`
7. `context/engagement.md`
8. any newly attached source material

## Evidence Types

Track evidence in these categories:

- independent use
- assisted use
- quality improvement
- time saved
- decision speed
- stress reduction
- confidence increase
- reduced rework
- better delegation
- faster drafting or analysis
- improved client service
- better use of existing tools
- reduced tool sprawl
- avoided privacy or quality risk

## Adoption Levels

Use these levels:

- `Not started`
- `Demoed`
- `Tried with AOTW`
- `Tried independently`
- `Repeated independently`
- `Embedded in workflow`
- `Paused`
- `Abandoned`

Do not mark adoption above the evidence.

## Scorecard Format

Maintain:

```markdown
# Outcomes Scorecard

## Current Summary

## Evidence Table

| Date | Area | Evidence | Adoption Level | Value Signal | Source | Confidence |
|---|---|---|---|---|---|---|

## Active Outcome Bets

## Proven Wins

## Weak Or Unproven Claims

## Risks To Adoption

## Next Evidence To Look For
```

## Confidence

Use:

- `High`: directly observed or explicitly stated by client
- `Medium`: strongly implied by evidence
- `Low`: plausible but not yet proven

Low-confidence claims should not appear as client-facing proof unless clearly labeled.

## What Counts As A Win

A win must show one or more:

- the client used something in real work
- the client came back with a result
- the client changed a repeated behavior
- a real task became easier
- a real risk was reduced
- a decision became clearer
- the client trusted the output enough to act on it

## What Does Not Count As A Win

Do not count:

- "client liked the demo"
- "tool looked promising"
- "we showed them"
- "we think this will save time"
- "client said AI is interesting"
- "workflow exists but no one used it"

## Output

Update `status/outcomes-scorecard.md`.

Then report:

```markdown
# Outcome Scorecard Update

## New Evidence Added

## Adoption Level Changes

## Proven Wins

## Claims Still Weak

## Adoption Risks

## Next Evidence To Seek
```

## Quality Check

Before finishing, verify:

- evidence is dated
- source is named
- adoption level is not inflated
- confidence is clear
- value is tied to client behavior or business reality
- client-facing claims are supportable

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/client-practice-plan.md`

````markdown
---
purpose: create-and-maintain-small-client-practice-steps
updated: 2026-06-19
trigger: Run when the client needs a small behavior step between sessions or when a transcript reveals a practical adoption opportunity.
---

# Client Practice Plan

## Purpose

Maintain `status/practice-plan.md` as the client’s small, realistic adoption plan.

The plan should help the client use AI in real work without feeling overloaded or judged.

## Required Read

Read:

1. `status/practice-plan.md`
2. `context/client-profile.md`
3. `context/writing-style-profile.md`
4. `status/current-status.md`
5. `status/outcomes-scorecard.md`
6. active `workstreams/`
7. latest relevant `sessions/`
8. `tools/tool-stack.md`
9. `privacy/data-boundaries.md`

## Practice Design Rules

A good practice step is:

- small
- tied to a real client task
- safe
- repeatable
- easy to remember
- easy to report back on
- not dependent on a complex new setup
- likely to produce evidence before the next session

Prefer one tiny practice over five ambitious ones.

## Practice Step Template

Use:

```markdown
## Current Tiny Practice

**Practice:**  
**When to use it:**  
**Exact first move:**  
**What good looks like:**  
**Time box:**  
**Fallback:**  
**What to bring back:**  
**Privacy note:**  
**Source:**  
```

## Candidate Practice Types

Examples:

- draft one difficult email with an AI assistant, then edit manually
- ask AI to summarize one long document before reading in detail
- use AI to turn messy notes into three next actions
- ask AI for three alternative phrasings before sending a sensitive message
- use AI to create a checklist for a repeated task
- use AI to find risks in a plan before a meeting
- use AI to prepare questions for one upcoming conversation

## Avoid

Do not suggest:

- daily habits that are too broad
- tool-switching for its own sake
- risky uploads of sensitive data
- multi-step automations before the client has a basic habit
- practices that require perfect prompting
- practices disconnected from the client’s real work

## Output

Update `status/practice-plan.md`.

Then report:

```markdown
# Practice Plan Update

## Current Tiny Practice

## Why This Practice

## Evidence It Is Realistic

## Privacy Boundary

## What To Check Next Session

## Practices Parked For Later
```

## Quality Check

Before finishing, verify:

- there is only one primary practice step
- it is tied to a real task
- it can be done in a short time
- it does not require sensitive data unless approved
- it will create useful adoption evidence

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/tool-stack-governor.md`

````markdown
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

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/privacy-boundary-check.md`

````markdown
---
purpose: check-client-privacy-trust-and-sharing-boundaries
updated: 2026-06-19
trigger: Run before client-facing outputs, public examples, third-party uploads, NotebookLM packs, screenshots, recordings, sensitive workflows, or new tool recommendations involving client data.
---

# Privacy Boundary Check

## Purpose

Protect client trust by identifying what information can be used, shared, transformed, uploaded, quoted, summarized, or generalized.

This skill should be run before producing anything client-facing, third-party-facing, public, or reusable across clients.

## Required Read

Read:

1. `privacy/data-boundaries.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `context/stakeholders.md`
5. relevant source material
6. relevant output draft
7. `tools/tool-stack.md` if third-party tools are involved

## Risk Categories

Classify the material:

- public
- client-approved
- internal AOTW only
- confidential client material
- sensitive personal material
- regulated or high-risk material
- credentials or access material
- unknown sensitivity

If sensitivity is unknown, treat as confidential until confirmed.

## Checkpoints

Ask:

- Who originally provided this information?
- Did the client approve this use?
- Is this needed for the output?
- Can it be summarized instead of quoted?
- Can it be anonymized?
- Can it be generalized into service IP?
- Will it be uploaded to a third-party tool?
- Does the third-party tool retain, train on, or expose data in a way that matters?
- Could this damage trust if seen by the client or a stakeholder?
- Could this reveal private strategy, weakness, or relationship dynamics?
- Could this expose customers, employees, finances, health, legal, or HR details?

## Redaction Rules

Redact or generalize:

- full names when not needed
- email addresses
- phone numbers
- private links
- customer names
- employee names
- financial details
- legal details
- health details
- passwords or credentials
- private stakeholder concerns
- raw transcript sections
- proprietary process details

Keep:

- the minimum context required to make the output useful
- client-approved names when necessary for direct client-facing work
- generalized patterns for internal playbooks

## Third-Party Tool Rules

Before using a third-party tool with client material:

1. Identify the data being uploaded.
2. Identify why upload is necessary.
3. Confirm whether the data can be reduced or anonymized.
4. Check whether the tool is approved or already in the stack.
5. Mark uncertainty if tool terms or access are not verified.
6. Recommend the safer version.

## Output

Produce:

```markdown
# Privacy Boundary Check

## Intended Use

## Material Reviewed

## Sensitivity Classification

## Allowed

## Not Allowed

## Needs Client Approval

## Redactions Required

## Third-Party Tool Concerns

## Safer Alternative

## Final Recommendation
```

For simple low-risk cases, a short version is acceptable:

```markdown
Privacy check: low risk. No sensitive client details included. Safe to share as drafted.
```

## Decision Values

Use:

- `Safe as drafted`
- `Safe after redaction`
- `Internal only`
- `Needs client approval`
- `Do not use`
- `Needs more information`

## Quality Check

Before finishing, verify:

- sensitive data is not accidentally included
- client-facing output does not reveal internal assessment
- reusable service IP is anonymized
- third-party upload is justified
- uncertainty is visible

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/session-retrospective.md`

````markdown
---
purpose: capture-internal-consulting-lessons-after-client-sessions
updated: 2026-06-19
trigger: Run after a client session, transcript processing, difficult interaction, successful delivery moment, or notable consulting lesson.
---

# Session Retrospective

## Purpose

Capture internal AOTW learning from a client session without turning every session into a long internal essay.

The retrospective should improve the next session, preserve relationship signals, and extract repeatable delivery lessons.

## Required Read

Read:

1. latest relevant `sessions/`
2. `status/current-status.md`
3. `status/action-registry.md`
4. `status/outcomes-scorecard.md`
5. `context/client-profile.md`
6. `context/stakeholders.md`
7. active `workstreams/`
8. `playbooks/personal-ai-upgrade-playbook.md`

## When To Write A Retro

Write a retrospective when the session includes:

- a major shift in client understanding
- a trust or relationship signal
- a recurring client fear or hesitation
- a strong adoption signal
- a failed or confusing demo
- a tool overload risk
- a useful coaching move
- a repeatable consulting pattern
- a moment where AOTW should change approach

Do not write a retro for routine source processing unless there is a useful lesson.

## Retrospective File

Append to:

```text
status/service-retrospective-log.md
```

If the file does not exist, create it.

## Entry Structure

Use:

```markdown
## YYYY-MM-DD - [Session / Topic]

**Context:**  
**What worked:**  
**What did not work:**  
**Client signal:**  
**AOTW delivery lesson:**  
**Next session adjustment:**  
**Reusable service pattern:**  
**Do not repeat:**  
**Source:**  
```

## What To Capture

Focus on:

- how the client reacted
- where the consultant created clarity
- where the consultant created overload
- which examples landed
- which language helped
- which workflow felt real
- which workflow felt abstract
- what should change next time

## Privacy

This is internal only.

Still avoid unnecessary sensitive details.

If the lesson is reusable across clients, send the generalized version to `service-ip-extractor.md`.

## Output

Update `status/service-retrospective-log.md`.

Then report:

```markdown
# Session Retrospective Update

## Entry Added

## Main Lesson

## Next Session Adjustment

## Reusable Pattern Found

## Follow-On Skill Recommended
```

## Quality Check

Before finishing, verify:

- the retro is useful for future delivery
- it is not just a transcript summary
- it does not blame the client
- it identifies one practical adjustment
- reusable patterns are generalized before being added to playbooks

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/learning-bundle-builder.md`

````markdown
---
purpose: create-small-client-learning-assets-and-practice-bundles
updated: 2026-06-19
trigger: Run when the client needs a guide, micro-SOP, prompt card, practice asset, learning packet, or source bundle for a specific workflow.
---

# Learning Bundle Builder

## Purpose

Create practical learning assets that help the client use AI in their real work.

The asset should be small, specific, and immediately usable.

It should not become a generic AI training manual.

## Required Read

Read:

1. `context/client-profile.md`
2. `context/writing-style-profile.md`
3. `status/current-status.md`
4. `status/practice-plan.md`
5. `status/outcomes-scorecard.md`
6. relevant `workstreams/`
7. latest relevant `sessions/`
8. `tools/tool-stack.md`
9. `privacy/data-boundaries.md`

Run `privacy-boundary-check.md` before including private client material, screenshots, transcript excerpts, examples from real client work, or third-party upload packs.

## Asset Types

Choose one:

- one-page workflow guide
- micro-SOP
- prompt card
- before-and-after example
- checklist
- practice worksheet
- client-safe source pack
- meeting prep aid
- review rubric
- NotebookLM source pack

Do not create multiple asset types unless requested.

## Learning Design Rules

A good bundle:

- starts from the client’s actual work
- shows the first move
- includes a safe example
- explains what good output looks like
- includes a fallback if AI gives a weak answer
- includes one tiny practice step
- avoids jargon
- does not over-teach the tool
- preserves the client’s standards and tone

## File Location

Create:

```text
learning/YYYY-MM-DD-[topic]-bundle.md
```

If the date is not meaningful, use:

```text
learning/[topic]-bundle.md
```

## Bundle Structure

Use:

```markdown
# [Topic] Learning Bundle

## Who This Is For

## When To Use It

## What This Helps With

## The First Move

## Step-By-Step

## Prompt Or Template

## What Good Looks Like

## What To Check Before Using The Output

## Common Failure Modes

## Fallback

## Tiny Practice

## Privacy Notes

## Source And Context
```

## Client-Safe Language

If the asset is client-facing:

- remove internal AOTW assessment
- remove sensitive stakeholder notes
- remove unapproved transcript quotes
- keep the language simple and direct
- avoid implying the client is behind
- do not overstate what AI can do

## NotebookLM Routing

If the user asks specifically for NotebookLM, audio overview, video overview, or a NotebookLM source pack, run `notebooklm-video-builder.md` after the basic learning bundle is scoped.

## Output

Create or update the learning file.

Then report:

```markdown
# Learning Bundle Created

## File

## Intended Use

## Client Task It Supports

## Practice Step

## Privacy Check

## Follow-Up Recommendation
```

## Quality Check

Before finishing, verify:

- the bundle teaches one workflow, not all AI use
- the client can act without a live consultant
- the examples are safe
- the practice is tiny
- the asset matches current tool status

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/notebooklm-video-builder.md`

````markdown
---
purpose: prepare-client-safe-notebooklm-source-packs-and-video-briefs
updated: 2026-06-19
trigger: Run when creating a NotebookLM source pack, audio overview, video overview, client learning video, or source set intended for NotebookLM-style generation.
---

# NotebookLM Video Builder

## Purpose

Prepare a clean, client-safe source pack and production brief for a NotebookLM-style audio or video overview.

This skill is optional and should run only when NotebookLM, audio overview, video overview, or source-pack creation is requested or clearly useful.

## Required Read

Read:

1. `learning/` file related to the topic, if one exists
2. `context/client-profile.md`
3. `context/writing-style-profile.md`
4. `status/current-status.md`
5. relevant `workstreams/`
6. relevant `sessions/`
7. `tools/tool-stack.md`
8. `privacy/data-boundaries.md`

Run `privacy-boundary-check.md` before preparing any source pack for upload.

## Source Pack Goal

The source pack should help generate a short, accurate, client-relevant explanation or learning aid.

It should not include raw transcripts unless explicitly approved.

Prefer distilled, client-safe source documents.

## Inputs To Prepare

Create:

- sanitized source notes
- key concepts
- client-safe examples
- terms to use
- terms to avoid
- desired length
- target audience
- required caveats
- do-not-mention list
- production prompt or briefing note

## File Location

Create:

```text
learning/YYYY-MM-DD-[topic]-notebooklm-pack.md
```

## Pack Structure

Use:

```markdown
# NotebookLM Source Pack - [Topic]

## Intended Audience

## Intended Outcome

## Source Safety Summary

## Approved Source Notes

## Key Concepts To Cover

## Client-Safe Examples

## Terms To Use

## Terms To Avoid

## Do Not Mention

## Suggested Audio / Video Brief

## Quality Checklist

## Privacy Review
```

## Production Brief Rules

The brief should request:

- practical explanation
- calm tone
- no hype
- no unsupported claims
- no exposure of private client context
- clear next step
- short recap of the practice or workflow

## Privacy Rules

Do not include:

- raw transcript
- private names unless approved
- sensitive customer or employee details
- credentials or private links
- internal AOTW strategy
- client weaknesses framed bluntly
- confidential business data

Use generalized examples where possible.

## Output

Create or update the NotebookLM pack.

Then report:

```markdown
# NotebookLM Pack Created

## File

## Intended Use

## Sources Included

## Sources Excluded

## Privacy Decision

## Suggested Generation Brief

## Human Review Needed
```

## Quality Check

Before finishing, verify:

- the pack can stand alone
- source material is sanitized
- the intended output is specific
- private client context is removed
- human review is required before upload if risk remains

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/technical-research-brief.md`

````markdown
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

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/workstream-pruner.md`

````markdown
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

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/client-style-profile-builder.md`

````markdown
---
purpose: capture-client-communication-style-and-language-preferences
updated: 2026-06-19
trigger: Run when source material includes client-written language, emails, message examples, tone preferences, approval feedback, or wording the client likes or dislikes.
---

# Client Style Profile Builder

## Purpose

Maintain `context/writing-style-profile.md` so future follow-ups, client-facing materials, prompts, and templates sound appropriate for the client.

The style profile should be based on evidence, not generic personality guesses.

## Required Read

Read:

1. `context/writing-style-profile.md`
2. `context/client-profile.md`
3. `context/stakeholders.md`
4. recent client emails or message examples
5. relevant session transcripts
6. previous client-facing outputs if available

## Evidence To Capture

Look for:

- words the client uses often
- level of formality
- sentence length
- directness
- humor or no humor
- preferred structure
- decision language
- how they ask for help
- how they approve or reject drafts
- phrases to reuse
- phrases to avoid
- topics that require extra care

## Confidence

Use:

- `High`: multiple direct examples
- `Medium`: one strong direct example
- `Low`: inferred from limited evidence

Do not present low-confidence style claims as rules.

## Profile Structure

Update:

```markdown
# Writing Style Profile

## Current Summary

## Evidence Samples

## Preferred Tone

## Structure Preferences

## Words And Phrases To Use

## Words And Phrases To Avoid

## Client-Facing Email Guidance

## Internal Notes For AOTW

## Confidence And Gaps
```

## Quoting Rules

Use short excerpts only when necessary to preserve style evidence.

Do not paste long private email sections.

Summarize sensitive examples.

## Output

Update `context/writing-style-profile.md`.

Then report:

```markdown
# Style Profile Update

## Evidence Used

## Style Guidance Added

## Confidence

## Gaps

## Impact On Future Follow-Ups
```

## Quality Check

Before finishing, verify:

- style claims are evidence-based
- private examples are not over-quoted
- guidance is useful for writing
- the profile does not stereotype the client
- uncertainty is visible

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/monthly-progress-report.md`

````markdown
---
purpose: create-client-safe-monthly-progress-summaries
updated: 2026-06-19
trigger: Run when producing a monthly update, executive summary, renewal support note, or client-facing progress report.
---

# Monthly Progress Report

## Purpose

Create a concise, client-safe progress report that shows what changed, what was delivered, what adoption evidence exists, what is still in progress, and what should happen next.

The report should be useful to the client, not just flattering.

## Required Read

Read:

1. `context/client-profile.md`
2. `context/engagement.md`
3. `status/current-status.md`
4. `status/action-registry.md`
5. `status/outcomes-scorecard.md`
6. `status/practice-plan.md`
7. recent `sessions/` for the month
8. active and recently completed `workstreams/`
9. `tools/tool-stack.md`
10. `privacy/data-boundaries.md`

Run `privacy-boundary-check.md` before finalizing the client-facing version.

## Report Location

Create:

```text
client-facing/monthly-progress-YYYY-MM.md
```

## Report Structure

Use:

```markdown
# Monthly Progress Report - [Month YYYY]

## Summary

## What We Worked On

## What Changed

## Adoption Evidence

## Decisions Made

## Open Actions

## Current Risks Or Blockers

## Recommended Focus For Next Month

## Tiny Practice For The Client

## Notes
```

## Client-Safe Rules

Include:

- plain progress
- real wins
- honest blockers
- next focus
- practical client action

Avoid:

- internal AOTW doubts
- sensitive stakeholder dynamics
- private transcript excerpts
- overclaiming ROI
- implying the client failed to do homework
- exposing confidential tool or data details

## Evidence Rules

Separate:

- delivered assets
- tried workflows
- independently adopted workflows
- planned work
- parked ideas

Do not collapse them into one success story.

## Output

Create or update the monthly report.

Then report:

```markdown
# Monthly Report Created

## File

## Month Covered

## Evidence Sources

## Client-Safe Wins

## Open Risks

## Privacy Check

## Suggested Send Note
```

## Quality Check

Before finishing, verify:

- all claims are supportable
- sensitive information is removed
- adoption is not overstated
- next month focus is clear
- the report is short enough to read

````


---

## Included File: `outputs/aotw-client-os-blueprint-v4/skills/service-ip-extractor.md`

````markdown
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

````

