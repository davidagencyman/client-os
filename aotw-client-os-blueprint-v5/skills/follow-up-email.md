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

