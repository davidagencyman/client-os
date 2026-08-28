---
title: AOTW Client OS Master Blueprint
purpose: reusable-build-instruction
audience: Ahead of the Wave team and AI coding agents
version: 6.1
updated: 2026-08-27
---

# AOTW Client OS Master Blueprint v6.1

## Objective

Build a private, AI-readable operating repository for one AOTW client
engagement. The repository must help David remember the client, prepare
thoughtfully, keep promises, preserve important session evidence, and maintain
the client-facing App Export without retaining raw transcripts. When the EAIC
app is in scope, the validated export must also be publishable to the matching
live client profile through the existing Brave workflow after confirmation. When a source
connector is configured, David must be able to say “Process” and have the
agent discover and process the unprocessed sources without a manual attachment
step. “Transcript and process” remains an explanatory variant.

This is not a normal codebase, a transcript dump, a generic skill library, or
the AOTW internal playbook. It is the durable client-specific memory and
operating surface.

## Design principles

1. The detailed session record is the canonical history.
2. Raw transcripts and raw source material are not required to remain in the
   repository.
3. Important source-derived evidence should be preserved in the session
   record, even when it is sensitive to the engagement.
4. Current status is a short projection of history, not a second history log.
5. App Export is a persistent client-facing projection with update continuity.
6. Session preparation is a live supervision conversation, not a PDF by
   default.
7. Add folders and capabilities when the work requires them, not in advance.
8. AOTW-internal methods and reusable service IP stay in a separate internal
   repository.
9. Every factual claim needs a source date, source reference, or explicit
   uncertainty.
10. Fewer, more useful updates are better than a cascade that touches every
    file after every session.
11. Source discovery and identity checks are explicit; a meeting title alone
    is never proof that a source belongs to this client.
12. A process command catches up all eligible unprocessed sources, not only the
    newest one.

## Data lanes

### Private session memory

This lane contains detailed, internal session records and the client context
needed for future work. It may include important client language, emotional or
relationship context, technical failures, commercial context, and other
engagement detail when it has future operational value.

Do not store passwords, API keys, authentication tokens, recovery codes, or
unnecessary raw third-party data. Summarize those safely and record the
boundary or blocker instead.

### App Export

This lane contains the exact client-facing JSON that is imported into the
client application. It must be useful to the client and must not expose
internal coaching observations, private third-party details, raw transcripts,
or unagreed internal commercial analysis.

The current file is the baseline for the next export. Git history provides
previous versions; do not create a new random export filename on every run. When
EAIC publication is enabled, this exact validated file is the only payload to
stage in the matching live client profile.

### AOTW internal knowledge

Generalized methods, service IP, consultant retrospectives, reusable playbooks,
and cross-client learning belong in a separate private AOTW repository. Never
copy private client details into that lane.

## Initial repository

Create only these files for a new engagement:

~~~
README.md
CLAUDE.md
AGENTS.md
context/
  client.md
  engagement.md
status/
  current.md
  actions.md
  decisions.md
  source-registry.json        # required when a connected source is enabled
privacy.md
capabilities.md
_skills/
  operating-router.md
  process-session.md
  app-export.md
  session-supervisor.md
  follow-up.md
  privacy-boundary.md
~~~

Create these only when the first real artifact requires them:

~~~
sessions/
workstreams/
tools/
deliverables/
learning/
~~~

Do not create empty directories, .gitkeep files, or a required _inbox folder.
When a connected source is enabled, source material is discovered through the
explicit source configuration and tracked in status/source-registry.json.
When no connected source is enabled, a directly attached source remains a
supported fallback.

## Required file roles

### README.md, CLAUDE.md, and AGENTS.md

README.md explains the repository purpose and short reading order.
AGENTS.md is the canonical operating instruction for capable coding agents.
CLAUDE.md is a thin compatibility pointer to README.md and AGENTS.md. Do not
duplicate the operating rules in three places.

### context/client.md

Store the canonical identity, professional role, working style, goals,
constraints, useful language, and confidence/uncertainty. Never infer the
identity from the repository slug alone.

### context/engagement.md

Store the confirmed engagement stage, scope, session rhythm, success
criteria, working agreements, and source-backed commercial or operational
terms. Mark proposals, hypotheses, and pending confirmations explicitly.

### status/current.md

Keep a concise current-state snapshot:

- active now
- blocked
- planned
- completed recently
- next useful focus

Link to detailed sessions and workstreams instead of repeating them. Keep this
file short enough to read before a session.

### status/actions.md

Track only concrete commitments, questions, blockers, and ownership changes.
Every active item needs an ID, owner, status, next step, and source/date.
Archive or close completed items rather than allowing the list to grow without
limit.

### status/decisions.md

Append explicit decisions with date, decision, rationale, conditions, and
source. Brainstorming and possibilities do not belong here.

### privacy.md

Describe the repository, App Export, and external-tool boundaries in plain
language. Treat privacy as routing and placement: preserve useful internal
evidence, but prevent secrets and unsafe disclosures.

### capabilities.md

List the installed capabilities and why they are enabled. The default core is
the six files in _skills/. Optional capabilities are added only when the
engagement needs them.

Each capability entry must state:

- what it does
- when to use it
- what it reads
- what it writes
- whether it is client-facing, internal, or conditional

## Connected-source discovery and catch-up

“Process”, “transcript and process”, “process transcripts”, and equivalent
requests mean run the connected-source catch-up routine. They do not mean “wait for David to
attach a file.” The client repository must record the source configuration in
the private repository, either in the processing skill or a referenced context
file, and must maintain status/source-registry.json.

### Required source configuration

For every connected client source, record:

- provider and connector name
- canonical root folder ID and URL
- folder structure and maximum scan depth
- supported MIME types or file extensions
- the client identity keys and evidence required for acceptance
- the timestamp/date field used as the meeting date
- fallback behavior when the connector is unavailable

Never put a private client’s source URL or folder ID into this public
blueprint. Put the concrete values in the private client repository.

### Google Drive procedure

Use the connected Google Drive plugin as the source of truth:

1. Read the client identity, source configuration, source registry, current
   state, and recent session frontmatter.
2. List the configured root folder. For a Google Meet root, list its dated
   meeting subfolders and then list the files inside each candidate folder.
3. Read metadata before fetching content. Compare the stable file ID and
   modified-time/revision fingerprint with the source registry before fetching.
   Reuse a prior terminal identity decision for an unchanged source; fetch
   readable content only for new, changed, or unresolved candidates. Consider
   native Google Docs and supported text/markdown sources; do not download or
   store raw source files.
4. Treat names, titles, and folder labels as candidate signals only. For a new
   or changed candidate, fetch the readable document text and verify the
   participant/client identity from the body or participant block. A
   same-looking meeting title is not enough.
5. If identity is clear, classify the source as accepted. If identity is
   ambiguous, record needs-review and do not process it. If it belongs to a
   different client, skip it without copying that client’s details into this
   repository.

### Selecting unprocessed sources

The source registry is the deduplication authority. A source is unprocessed if
its stable provider file ID is not recorded as processed, or if the provider’s
modified time/revision fingerprint changed after processing. The latest
processed date is an optimization and a human-readable cursor; it is not a
reason to discard an older source that arrived late.

After identity checks, sort accepted sources by meeting date and time and
process every eligible unprocessed source in ascending order. For example, if
the latest processed session is on the 18th and eligible sources exist on the
21st, 21st, and 22nd, process all three in that order. Do not process only the
single newest source.

### Resume and completion behavior

After each accepted source, persist its source ID, source fingerprint, meeting
date, session path, and processing result in the registry. If one source fails,
continue with independent sources, mark the failure, and report it. A later
run retries only pending or failed sources whose identity and fingerprint still
require work.

When the batch has at least one accepted source, run App Export automatically
as the final repository step of the same request, after all durable session and
state updates. Then run App Export's live EAIC publication section: resolve the
exact account in Brave, stage the final validated JSON, ask for action-time
confirmation immediately before `Save changes`, and verify the post-save state.
If no eligible source exists, report a clean no-op, leave the existing profile
unchanged, and do not publish.

The completion report must include: root scanned, candidate count, accepted
count, processed count, skipped/ambiguous count, failed count, session files
created, state files changed, App Export result, EAIC publication state, and the
source IDs or paths that still need attention. Never claim a scan when Drive was unavailable.

## Detailed session record

Create one file for each substantive call or source:

~~~
sessions/YYYY-MM-DD-[topic].md
~~~

The session record is deliberately detailed. It is the compressed replacement
for the raw transcript and must be useful to an AI months later.

Required frontmatter:

~~~
---
session_id: YYYY-MM-DD-topic
date: YYYY-MM-DD
session_type: discovery | coaching | implementation | troubleshooting | other
source_type: transcript | meeting-notes | email | document | mixed
source_reference: source-id-or-title
participants: []
duration: unknown
confidence: confirmed | mixed | provisional
---
~~~

Required sections:

1. Executive summary
2. What actually happened
3. Client language and important quotes
4. Work, pain, and context revealed
5. Decisions and reasoning
6. Commitments and ownership
7. Blockers, failed attempts, and what they teach us
8. Tools and workflow state
9. Emotional and relationship context
10. Adoption and outcome evidence
11. Privacy and data-boundary decisions
12. Open questions and uncertainty
13. What must carry forward
14. Suggested follow-on capabilities

Write specific evidence rather than generic summaries. Preserve the details
that explain why the next session should be different. Do not copy the raw
transcript or create a second full history in status files.

## Processing lifecycle

When a new source is accepted, either from connected-source catch-up or a
direct attachment:

1. Complete the source-discovery and identity steps above when the request is
   a catch-up command.
2. Read the client identity, engagement, current status, actions, decisions,
   privacy rules, source registry, and recent sessions.
3. Create one detailed session record per accepted source.
4. Update only the current-state files supported by the source.
5. Create or update a workstream only when the topic spans sessions and has a
   clear outcome, owner, and next step.
6. Update the source registry after each result.
7. Run App Export after durable batch processing is complete.
8. Stage and, after David's action-time confirmation, publish the final App
   Export to the exact EAIC client account through Brave; verify the live state.
9. Validate the App Export JSON and the session metadata.
10. Report what was captured, what changed, what was skipped, what was published,
    and what remains uncertain.

The process command must never claim that a source was checked when the
connector was unavailable or identity could not be verified.

## App Export lifecycle

The canonical payload is stored at:

~~~
app/profile.json
~~~

The app/profile.json file is created when App Export is enabled. It must be
valid according to schemas/app-profile-export-v1.schema.json.

When exporting:

1. Read the existing app/profile.json first.
2. Read current status, actions, practice, outcomes, tools, privacy, the source
   registry, the newest sessions in the completed batch, and active workstreams
   as applicable.
3. Preserve stable IDs and existing client-facing content unless evidence
   changes it.
4. Update only fields supported by the latest durable evidence.
5. Keep unresolved items unresolved; do not invent a client-facing completion.
6. Mark superseded content by replacement or status, not by duplicating it.
7. Validate the complete JSON against the schema.
8. Write the same complete JSON to app/profile.json and show that exact JSON in
   chat for drag-and-drop import.
9. When at least one source was accepted and EAIC publication is enabled, run
   the existing App Export publication procedure in Brave. Match the exact
   client account, touch only the Profile section, require confirmation
   immediately before `Save changes`, and verify the saved state. Do not alter
   access, passwords, danger-zone controls, or materials.

The export is an update to a living client profile, not a new profile created
from zero. If processing finds no new accepted source, avoid unnecessary
content churn and keep the existing profile unchanged.

The capability is called App Export. Do not use the legacy human-facing name
My Next Step Export. Keep the wire schema stable unless the application owner
changes the import contract.

## Session supervision

When David asks for preparation, run the session-supervisor capability as a
conversation.

The supervisor should:

- synthesize the current client situation
- identify unfinished loops and relationship risks
- ask a small number of high-value questions
- challenge weak assumptions
- help choose one realistic session outcome
- suggest a humane consulting move
- adapt to the client's needs and adoption stage
- research current technical facts only when they affect the decision
- help David rehearse exact language only when useful

Do not create a PDF or a minute-by-minute protocol by default. At the end,
offer a short focus note only if it would help.

## Optional capabilities

Add an optional capability only when its use is clear:

- practice plan — one between-session behavior
- tool register — active, blocked, fallback, parked, or unknown tools
- outcome scorecard — adoption and value evidence
- client style profile — repeated language and communication preferences
- technical research — current external product or implementation facts
- learning bundle — a guide or practice asset
- NotebookLM — an explicitly requested source pack or video/audio workflow
- connected source sync — a configured Drive/Gmail or other source boundary

Internal-only capabilities such as service-IP extraction and consultant
retrospectives do not belong in client repositories.

## Workstream rule

Create a workstream only when:

- the topic matters beyond one conversation
- the desired outcome is clear
- an owner exists
- there is a concrete next step

Keep no more than three active workstreams without an explicit reason. Park
or archive the rest. A list of ideas is not a workstream.

## Quality gate

Before declaring a new repository or processing run complete, verify:

- client identity and engagement stage are explicit
- uncertainty is labelled
- at least one detailed session exists when source material was processed
- no raw transcript is stored unless explicitly authorized
- important evidence is not lost through over-summarization
- current.md is genuinely current and concise
- actions and decisions have owners/sources where applicable
- App Export reads and updates the previous profile
- App Export validates against the import schema
- connected-source runs read and update the source registry
- all eligible sources newer than the processing cursor are either processed,
  explicitly skipped for identity/privacy reasons, or recorded as needing
  review
- the App Export JSON contains no internal-only detail
- the EAIC publication path matches the exact client account, requires final
  confirmation before `Save changes`, and reports a pending state when it cannot
  verify publication
- no empty placeholder directories were created
- only enabled capabilities are present
- internal AOTW knowledge is not mixed into client memory
- all file references resolve

## Build procedure

1. Create a private repository with the client slug.
2. Add the initial files from this blueprint and the core skills.
3. Add verified discovery context only; preserve unknowns.
4. Configure the canonical connected source when one is available and create
   status/source-registry.json.
5. Enable App Export and create the initial valid profile when the app is part
   of the engagement.
6. Use the existing App Export publication procedure for the live EAIC profile;
   do not add a second standalone sync skill, and never store credentials.
7. Run the first catch-up scan; process every eligible backlog source, not just
   the newest one.
8. Run the quality gate.
9. Record the blueprint version in README.md.

Do not migrate older client repositories automatically. Use this blueprint as
the new default, then create a deliberate migration map that preserves their
history.
