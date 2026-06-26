---
purpose: capture-a-session-with-enough-durable-context
updated: 2026-06-26
trigger: Run when a discovery call, coaching session, meeting, or working call needs to be written into the repo as a session note.
---

# Session Note

## Purpose

Turn one call or meeting into a durable session note that preserves the real context of what happened.

The note is the long-term memory of the engagement. Months later, an AI agent or a different consultant should be able to read it and understand exactly what happened, what was decided, what the client said, and how the client felt, without the transcript.

This skill exists because thin, one-line session summaries lose the context that makes the next session good. Capture what matters. Do not bloat the repo.

## The Core Tension

Keep enough context to fully reconstruct the session. Cut everything that does not change a future decision, action, or tone.

A good session note is usually one to three screens. Long enough to rebuild the session from memory. Short enough to read before the next call.

When in doubt, keep specifics (what was tried, what the client said, why a choice was made) and drop filler (greetings, repeated small talk, transcript noise, generic AI commentary).

## One File Per Call

Create one note per call or meeting:

```text
sessions/YYYY-MM-DD-[type].md
```

`[type]` is one of: `discovery`, `session`, `strategy`, `troubleshooting`, `check-in`.

If the date is unknown, use `sessions/undated-[type]-[short-topic].md` and mark the date as unknown.

## Required Read Before Writing

Read enough to place this session in context:

1. `context/client-contact.md`
2. `context/client-profile.md`
3. the previous `sessions/` note
4. `status/current-status.md`
5. `status/action-registry.md`
6. relevant active `workstreams/`

## Frontmatter

```yaml
---
date: YYYY-MM-DD
duration: approximate (e.g., "~90 min")
type: discovery | session | strategy | troubleshooting | check-in
attendees: [Name 1, Name 2]
topics: [specific-topic-1, specific-topic-2]
source: filename or description of the raw source
---
```

Use specific topic slugs, not vague ones. `gmail-filters-setup` is useful. `productivity` is not.

## Body Structure

```markdown
# Session Note - [Client] - YYYY-MM-DD

## Summary

## Context Going In

## Key Discussion Points

### [Topic 1]
### [Topic 2]

## Decisions Made

## Action Items

## Open Questions

## Client Language To Preserve

## Mood And Dynamics

## Carry Into Next Session
```

### Summary

A real paragraph, roughly 5 to 8 sentences. Not one or two lines.

Say what happened, what mattered, what changed, and where things stand now. Be specific and concrete, not abstract. Name the real workflows, tools, and moments.

Someone who was not on the call should understand the session from this paragraph alone.

### Context Going In

2 to 4 sentences. What was happening before this call, what this session was meant to address, and what carried over from last time.

This is what lets a future reader rebuild the thread, not just the single session.

### Key Discussion Points

This is the heart of the note. Use an `###` subsection per major topic.

For each topic, capture the real detail:

- what was discussed
- what was tried
- what worked
- what failed or confused the client
- what the client actually said, with short direct quotes
- any technical specifics that matter (settings, names, steps, numbers)

Write enough that an AI reading this months later understands exactly what happened, not just the headline.

Use short quotes, not large transcript dumps.

### Decisions Made

A bullet list of actual decisions. Also add each to `status/decisions-log.md`.

Log decisions, not brainstorming. A decision has commitment behind it ("we decided", "we will", "we will not").

### Action Items

Format each as:

```text
- **Owner**: description (context or due date if known)
```

Also push these into `status/action-registry.md` via `action-registry-maintainer.md`. The note records them; the registry tracks them.

### Open Questions

Unresolved items, blockers, or things to confirm before or during the next session.

### Client Language To Preserve

Notable phrases, vocabulary, metaphors, or quotes that show how the client thinks and talks.

Send useful examples to `client-style-profile-builder.md` so the client's voice is preserved over time.

### Mood And Dynamics

2 to 4 sentences on client energy, frustration, enthusiasm, confidence, and trust.

This is critical for AI tone calibration on the next session and follow-up. Be honest and specific. Do not blame the client.

### Carry Into Next Session

What to revisit, the likely next focus, and the tiny practice step the client agreed to. This feeds `call-prep.md` and `client-practice-plan.md`.

## Follow-On Updates

After the note, make sure the rest of the repo reflects it:

- `status/current-status.md` - update active priorities, blockers, what changed
- `status/decisions-log.md` - add decisions
- `status/action-registry.md` - add or update commitments
- `status/outcomes-scorecard.md` - add adoption or value evidence if present
- relevant `workstreams/` - update progress and next steps

Do not duplicate the full action list forever. The note is the record of the call; the status files are the live trackers. Cross-reference rather than copy everything twice.

## Quality Check

Before finishing, verify:

- the summary is a real paragraph, not one line
- a reader could reconstruct the session from the note alone
- real client quotes and language are preserved
- decisions and actions are captured and mirrored to their trackers
- mood and dynamics are recorded for tone calibration
- the note is detailed where it matters and not padded where it does not
- evidence is separated from inference, and uncertainty is marked

## Do Not Do

Do not:

- write a one or two line summary
- paste large transcript sections
- strip out the context that makes the next session good
- pad the note with generic AI consulting language
- invent precision the source does not support
- bury sensitive details in a client-facing place (this note is internal)
