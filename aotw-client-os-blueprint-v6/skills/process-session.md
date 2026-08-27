---
purpose: preserve-detailed-session-memory-from-new-source
version: 6.0
trigger: Run for a directly attached transcript, meeting note, email, document, screenshot notes, or other substantive source.
---

# Process Session

Turn new source material into one detailed, AI-optimized session record and
the smallest necessary current-state updates. The raw source is evidence, not
the repository deliverable.

## Before extracting

Read:

1. context/client.md
2. context/engagement.md
3. status/current.md
4. status/actions.md
5. status/decisions.md
6. privacy.md
7. capabilities.md
8. the newest relevant session and workstream files

For connected sources, verify the canonical client identity before processing.
If identity is ambiguous, stop processing that source and record the
uncertainty.

## Create the detailed session record

Create sessions/YYYY-MM-DD-topic.md using templates/session-template.md.
The record is the compressed replacement for the raw transcript, so preserve
all detail that will change future consulting work:

- what actually happened and in what sequence
- the client's concrete work, pain, and goals
- important wording and quotes
- decisions and the reasoning behind them
- every meaningful commitment and owner
- blockers, failed attempts, and their consequences
- tool and workflow state
- emotional and relationship signals
- adoption and outcome evidence
- privacy or consent boundaries
- open questions and what must carry forward

Compress repetition, filler, and transcript mechanics. Do not compress away
meaning, a failed attempt, a client reaction, or a condition attached to a
decision.

## Update the operating state

Update only files supported by the source:

- status/current.md for the present situation
- status/actions.md for concrete commitments or blockers
- status/decisions.md for explicit decisions
- context/client.md for durable client facts or preferences
- context/engagement.md for confirmed scope or working agreements
- workstreams/ only when a durable thread has an outcome, owner, and next step

Do not copy the entire session into those files. Link back to the session.
Do not automatically update internal AOTW playbooks or consultant retrospectives
from a client source.

## Required next step

When the source was accepted and durable updates completed, run
app-export.md. App Export must read the previous app/profile.json before
creating the next client-facing profile.

## Completion report

Report:

- source and classification
- session file created
- current-state files updated
- actions and decisions found
- workstreams created or changed
- important uncertainty
- App Export result
- capabilities deliberately skipped

Never store passwords, API keys, tokens, recovery codes, or raw source files.
