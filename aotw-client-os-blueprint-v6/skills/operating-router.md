---
purpose: default-entry-and-minimum-useful-routing
version: 6.1
trigger: Start here for any unclear request, “transcript and process”, source processing, session preparation, follow-up, App Export, or repository update.
---

# Operating Router

Use this as the default entry point. Its job is to identify the situation,
read only the context needed, and choose the smallest useful capability chain.

## Read first

1. README.md
2. context/client.md
3. context/engagement.md
4. status/current.md
5. status/actions.md
6. status/decisions.md
7. status/source-registry.json when connected-source processing is enabled
8. privacy.md
9. capabilities.md

Read detailed sessions and workstreams only when they are relevant to the
request. Do not treat the repository slug as proof of client identity.

## Route by situation

| Situation | Run |
|---|---|
| “Transcript and process” / process transcripts | process-session in connected-source catch-up mode; then App Export automatically |
| Directly attached new transcript, notes, email, or source | process-session, then App Export |
| Prepare for a session | session-supervisor |
| Draft a recap or follow-up | follow-up |
| Explicit App Export request | app-export |
| Sharing, uploading, or sensitive material | privacy-boundary |
| Tool question or current product fact | use technical research only if enabled and necessary |
| General cleanup | update current state only; do not create workstreams by default |

## Routing rules

- “Transcript and process” is a command to search the configured source root;
  do not ask David to attach each transcript when the connector is available.
- Discover all eligible unprocessed sources, not only the newest source.
- Use stable source IDs and revision fingerprints to deduplicate; do not rely on
  filenames or dates alone.
- Verify identity from document content/participants before processing. A title
  match is not enough.
- Do not run every capability because a source exists.
- Do not create an action from vague curiosity.
- Do not create a workstream unless it has an outcome, owner, and next step.
- Keep important source-derived detail in the session record.
- After a successful new-source processing run, App Export is part of the
  completed chain.
- After a catch-up batch, run App Export once from the final durable state in
  the same request.
- If a connector fails or identity cannot be verified, report that boundary
  instead of claiming the source was checked.

## Router report

Keep the internal routing note concise:

1. situation
2. source detected
3. files read
4. capabilities run
5. capabilities skipped and why
6. main uncertainty
7. expected files changed
