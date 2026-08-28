---
purpose: discover-and-preserve-detailed-session-memory-from-new-sources
version: 6.1
trigger: Run when David says “Process”, “transcript and process”, “process transcripts”, “process the new transcripts”, or provides a directly attached substantive source.
---

# Process Session

Turn source material into detailed, AI-optimized session records and the
smallest necessary current-state updates. When a connected source is enabled,
this skill starts by discovering the client’s unprocessed sources; it does not
wait for David to attach each file manually. The raw source is evidence, not
the repository deliverable.

## Non-negotiable meaning of the command

“Process” is the canonical catch-up command; “transcript and process” and
other explanatory variants mean the same thing. It means **catch up the repository**:

- find the configured source root through the connected source connector;
- discover all candidate meeting/source files;
- verify that each candidate belongs to this client;
- compare stable source IDs and revisions with the source registry;
- process every eligible unprocessed source, oldest first;
- persist progress and finish with App Export.

If the latest processed session is on the 18th and eligible sources exist on
the 21st, 21st, and 22nd, process all three. “Latest” is not a one-file limit.

## Step 0 — Read the operating state

Read, in this order:

1. context/client.md
2. context/engagement.md
3. status/current.md
4. status/actions.md
5. status/decisions.md
6. privacy.md
7. capabilities.md
8. status/source-registry.json
9. the newest relevant session and workstream files

If the registry does not exist but sessions already do, derive an initial
registry from their frontmatter before scanning and then persist it.

## Step 1 — Discover candidates in the configured source

Use the connected Google Drive plugin when the repository’s source
configuration names Google Drive. Read metadata before content.

1. Read the private source configuration in this repository. It must name the
   canonical root folder, folder ID/URL, folder structure, scan depth, supported
   file types, identity keys, and date rule. Compare each candidate's stable
   file ID and modified-time/revision fingerprint with the source registry
   before fetching content; unchanged sources with a recorded terminal
   decision can reuse that decision.
2. List the configured root folder. For a Google Meet source, list its direct
   dated meeting subfolders, then list each subfolder’s files.
3. Consider native Google Docs and configured text/markdown sources. Do not use
   an unrelated global “Transcripts” folder unless the client configuration
   explicitly says it is the source of truth.
4. Use the meeting timestamp in the source title/metadata as the session date;
   use modified time only for revision/deduplication.
5. If Drive is unavailable, stop the scan, report the connector boundary, and
   do not claim that transcripts were processed.

## Step 2 — Verify client identity before processing

Titles and folder names are candidate signals, not proof. For a new, changed,
or unresolved candidate, fetch the readable document text and verify the
participant block or body against the canonical client identity and aliases in
context/client.md. Do not refetch an unchanged source whose registry entry
already records an accepted, rejected, or needs-review identity decision.

- Accept only when the source clearly belongs to this client.
- Mark ambiguous sources `needs-review` and do not process them.
- Skip sources belonging to another client without copying their names,
  content, or details into this repository.
- Never let a shared meeting title override a body-level identity mismatch.

Record the identity decision and stable provider source ID in the source
registry, with the minimum detail needed to prevent repeated ambiguity.

## Step 3 — Select the unprocessed set

The source registry is authoritative. A candidate is eligible when its stable
source ID has no processed record, or when its provider modified time/revision
fingerprint is newer than the processed record. The latest processed date is a
cursor and optimization, not a filter: late-arriving sources must still be
processed.

After identity filtering, sort eligible sources by meeting date/time ascending
and process all of them in one invocation. Do not stop after the newest file.

## Step 4 — Create the detailed session record for each accepted source

Create `sessions/YYYY-MM-DD-topic.md` using the session template. Include the
stable source ID, source URL when private storage permits it, provider modified
time/revision, and the identity classification in frontmatter. Do not store the
raw transcript.

The record must preserve all detail that will change future consulting work:

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

## Step 5 — Update the operating state and registry

Update only files supported by the source:

- status/current.md for the present situation
- status/actions.md for concrete commitments or blockers
- status/decisions.md for explicit decisions
- context/client.md for durable client facts or preferences
- context/engagement.md for confirmed scope or working agreements
- workstreams/ only when a durable thread has an outcome, owner, and next step

After each candidate result, update status/source-registry.json with the source
ID, source fingerprint, session date, identity status, processing status,
session path, and any failure or review note. This makes the next command
resumable and fast.

## Step 6 — Run App Export automatically

When one or more sources were accepted and the batch’s durable updates are
complete, run app-export.md automatically in the same request. App Export must
read the previous app/profile.json before creating the next client-facing
profile, then stage the final validated file in the exact EAIC client account
through Brave and ask for action-time confirmation immediately before
`Save changes`. If there were no eligible sources, leave the existing profile
unchanged and do not publish.

## Step 7 — Publish the live EAIC profile

After App Export has written and validated `app/profile.json`, run its
`Publish to the live EAIC profile` section. If Brave is unavailable, the
identity match is not exact, the JSON is invalid, or David has not confirmed,
do not save and report EAIC publication as pending. Do not change access,
passwords, danger-zone controls, or client materials.

## Step 8 — Completion report

Report:

- the source root scanned and candidate count
- accepted, processed, skipped, ambiguous, and failed counts
- session files created
- current-state files updated
- source-registry entries updated
- actions and decisions found
- workstreams created or changed
- App Export result
- EAIC profile publication state: published, pending, or not attempted, with the reason when pending
- capabilities deliberately skipped

If the connector was unavailable or a source could not be identity-verified,
say that explicitly. Never report a clean completion for an unverified scan.

Never store passwords, API keys, tokens, recovery codes, or raw source files.
