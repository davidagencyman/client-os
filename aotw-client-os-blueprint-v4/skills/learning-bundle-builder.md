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

