---
purpose: process-directly-attached-transcripts-notes-and-source-material
updated: 2026-06-26
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

For discovery or session transcripts, create a session note with `session-note.md`.

That skill defines the full session-note format and is the source of truth for it. Do not write a thin one-line summary here. Capture enough context that a future AI agent or consultant can reconstruct the session without the transcript, while keeping the repo from bloating.

Create:

```text
sessions/YYYY-MM-DD-[type].md
```

If the date is unknown, use `sessions/undated-[type]-[short-topic].md` and mark the date as unknown.

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

