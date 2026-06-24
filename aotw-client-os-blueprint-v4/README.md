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
