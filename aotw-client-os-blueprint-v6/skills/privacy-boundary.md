---
purpose: route-important-information-between-private-and-client-facing-lanes
version: 6.1
trigger: Run before App Export, external uploads, public examples, sensitive sharing, or any uncertain data-handling decision.
---

# Privacy Boundary

Privacy is a routing decision, not a command to erase useful client context.
The private repository is the internal engagement memory. The App Export is
the client-facing projection. AOTW service IP belongs in the internal AOTW
knowledge lane.

## Classify the material

### Keep in private session memory

Keep important details that improve future preparation or delivery, including
client language, emotional context, technical failures, commercial context,
relationship dynamics, and the reasoning behind decisions.

### Summarize or redact

Summarize credentials, financial identifiers, personal contact details,
unnecessary third-party names, raw attachments, or details that are not needed
to operate the engagement.

### Keep out of App Export

Exclude internal coaching observations, consultant self-critique, raw
transcripts, private third-party information, internal commercial analysis,
unagreed proposals, and operational details the client does not need.

### Keep out of AOTW internal knowledge

Do not move client-identifying details, private language, raw source material,
or relationship intelligence into generalized methods or reusable service IP.

## Live EAIC profile publication

- Publish only the validated, client-safe `app/profile.json`; never upload raw
  transcripts or the private repository as a substitute.
- Resolve the exact visible client account in the EAIC admin panel and re-check
  its name and email before loading the profile.
- Leave login email, passwords, access controls, danger-zone controls, and
  library materials unchanged.
- Ask for confirmation immediately before `Save changes`, even when
  `Process` was requested. If publication cannot be verified, report it as
  pending rather than claiming the client profile changed.

## Checklist

Before sharing or exporting:

1. Is the information important for future work?
2. Is it in the correct lane?
3. Is the identity and source confidence clear?
4. Does the wording disclose more than the recipient needs?
5. Are secrets or raw credentials absent?
6. Are third-party details necessary and permitted?
7. Are proposals clearly marked as proposals?
8. Is client-facing language understandable and useful?

For connected-source processing, also verify:

9. Was the source found under the configured client root?
10. Was identity verified from the source body or participant data rather than
    title alone?
11. Are source IDs and private Drive URLs kept only in the private client
    repository, never in the public blueprint or AOTW-wide knowledge?
12. Were ambiguous or other-client sources skipped without copying their
    content into this client lane?

Before EAIC publication, also verify:

13. Is the payload exactly the validated `app/profile.json`?
14. Is the visible EAIC account an exact name/email match?
15. Has David confirmed the write immediately before `Save changes`?
16. Was the post-save generated/profile-updated state verified?

Record a boundary or uncertainty when the answer is unclear. Do not silently
discard important evidence.
