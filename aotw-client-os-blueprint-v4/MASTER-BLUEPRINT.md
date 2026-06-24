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
