---
purpose: update-persistent-client-facing-app-profile
version: 6.1
trigger: Run automatically after every successful source-processing batch and whenever David explicitly asks for App Export.
---

# App Export

App Export creates the complete client-facing profile JSON used by the
application admin panel. It is an update to a living profile, not a new
profile generated from zero.

The canonical file is app/profile.json. Git history provides previous
versions. Do not create a new date-stamped export file for every run.

## Read before generating

1. The existing app/profile.json, if present
2. context/client.md
3. context/engagement.md
4. status/current.md
5. status/actions.md
6. status/decisions.md
7. privacy.md
8. status/source-registry.json when connected-source processing is enabled
9. every newly created detailed session in the completed batch
10. active workstreams, practice, outcomes, and tools only when those
   capabilities are enabled
11. schemas/app-profile-export-v1.schema.json

Never summarize raw transcript material directly into the App Export. Use the
durable session and current-state records.

## Update rules

1. Preserve the existing schema and all required top-level fields.
2. Preserve stable IDs for goals, practices, homework, prompts, milestones,
   workstreams, and other repeated items.
3. Keep useful existing client-facing language unless new evidence changes it.
4. Update status, wording, and next steps only when supported by evidence.
5. Do not turn a demonstration into independent adoption.
6. Do not turn a proposal into an agreement.
7. Replace superseded content instead of duplicating it.
8. Keep internal coaching observations, raw source material, private
   third-party details, secrets, and unagreed internal commercial analysis out
   of the client-facing payload.
9. Use stable clientId and displayName values from context/client.md, never
   from the repository slug alone.
10. Keep generatedAt current and source references accurate.

## Process behavior

After a new source or catch-up batch:

1. Load the previous profile.
2. Compare it with the final newly updated internal state and every accepted
   session in the batch.
3. Apply the smallest evidence-supported changes.
4. Validate the complete object.
5. Write the complete object to app/profile.json.
6. Return that exact object in one clean JSON block for drag-and-drop.
7. Give a short change summary outside the JSON when the surrounding workflow
   permits it.

If there is no new accepted source, do not create content churn. The existing
profile remains the current baseline.

## Validation

The JSON must:

- parse with no comments or trailing commas
- validate against schemas/app-profile-export-v1.schema.json
- use schemaVersion client-profile-export/v1
- contain exactly the schema's required top-level fields
- use allowed enum values
- contain no internal-only material
- preserve continuity with the previous profile

The human-facing capability name is App Export. My Next Step Export is legacy
terminology. Do not rename the wire schema without confirming an application
contract change.
