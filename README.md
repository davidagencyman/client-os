---
title: AOTW Client OS Blueprints
purpose: package-entry-point
updated: 2026-08-27
---

# AOTW Client OS

This repository contains versioned blueprints for creating private,
AI-readable operating repositories for Ahead of the Wave client engagements.

## Current default

Use aotw-client-os-blueprint-v6/ for all new client repositories.

v6 is built around detailed, AI-optimized session records as the durable
replacement for retained raw transcripts. It also provides persistent,
update-aware App Export and conversational session supervision.

Start with:

1. aotw-client-os-blueprint-v6/MASTER-BLUEPRINT.md
2. aotw-client-os-blueprint-v6/templates/
3. aotw-client-os-blueprint-v6/skills/
4. aotw-client-os-blueprint-v6/schemas/

## Legacy package

aotw-client-os-blueprint-v5/ remains available for existing repositories that
still use the v5 structure. Do not use it for new client repositories.

The standalone V5 complete file is retained for compatibility.

## Repository boundary

This public package contains generic build instructions and sanitized
templates. Client context, internal AOTW service IP, consultant retrospectives,
and raw source material belong in private repositories.
