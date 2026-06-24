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

