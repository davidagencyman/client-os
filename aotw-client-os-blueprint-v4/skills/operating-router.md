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

