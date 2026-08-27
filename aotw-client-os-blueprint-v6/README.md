---
title: AOTW Client OS Blueprint v6
purpose: reusable-build-instruction
version: 6.0
updated: 2026-08-27
---

# AOTW Client OS Blueprint v6

This is the default blueprint for new Ahead of the Wave client operating
repositories.

v6 is built around one practical fact: the raw transcript is not retained.
The detailed, AI-optimized session record is therefore the durable memory of
the engagement. Current status, actions, decisions, and the client-facing App
Export are projections of that memory.

## What changed from v5

- Detailed session records remain first-class and are not aggressively
  shortened.
- App Export is a persistent, update-aware profile rather than a stateless
  one-off JSON response.
- Session preparation is an interactive mentor/supervisor conversation by
  default, not a PDF or a minute-by-minute script.
- Folders and capabilities are created on demand.
- AOTW-internal methods, retrospectives, and service IP stay outside the
  client repository.
- Privacy routes information to the correct lane instead of removing useful
  internal session evidence.

## Package contents

- MASTER-BLUEPRINT.md — the build and lifecycle contract.
- skills/ — the small v6 core skill set.
- templates/ — initial repository and detailed-session templates.
- schemas/app-profile-export-v1.schema.json — the existing App Export import
  contract, kept stable for compatibility.

## Default rule

Create the smallest repository that can support the next real consulting
decision. Add a capability only when the client engagement needs it, the
capability has a clear owner, and its output is understood.

Do not create empty directories or copy every possible skill into every
client repository.
