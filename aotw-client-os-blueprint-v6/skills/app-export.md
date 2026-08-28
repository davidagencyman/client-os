---
purpose: update-persistent-client-facing-app-profile
version: 6.1
trigger: Run automatically after every successful source-processing batch, whenever David explicitly asks for App Export, or when a live EAIC profile sync is requested.
---

# App Export

App Export creates the complete client-facing profile JSON used by the
application admin panel. It is an update to a living profile, not a new
profile generated from zero. When the EAIC app is in scope, the same workflow
also publishes the validated profile to the matching live client account after
David's action-time confirmation.

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
8. When at least one source was accepted or David explicitly requested a live
   sync, continue with the publication section
   below after the complete repository update is finished.

## Publish to the live EAIC profile

The repository's `app/profile.json` is the only payload to publish. After the
export is written and validated, continue with this publication step in the
same `Process` request when at least one source was accepted, or when David
explicitly requests a live sync. This is not a second export and does not add a new skill.

1. Run `privacy-boundary.md` and use the current file, not an earlier chat
   copy.
2. Use `browser-session-router` to connect to David's Brave session. If Brave
   is closed, launch Brave and retry the extension bridge; keep the same Brave
   session and do not switch browsers.
3. Open `https://app.aheadofthewave.ai/admin`, search the exact
   `displayName` or another verified lookup value, and open the visible client
   row. Re-check the detail page's exact name and email; never infer the
   account from the repository slug or a similar name.
4. Touch only the Profile section: load the final `app/profile.json` into the
   profile JSON editor. Do not change the login email, password or access
   controls, danger-zone controls, or client materials.
5. Wait for `Profile is valid` and
   `Unsaved changes — save to publish them to the client`. Re-check
   `schemaVersion`, `clientId`, `displayName`, and the generated/source
   dates.
6. Immediately before the external write, ask David to confirm the exact client
   account and that this profile should be published. This confirmation is
   required even when `Process` was requested.
7. Click `Save changes` once. Verify the new generated/profile-updated date
   and that the unsaved notice is gone.

If the repository batch still has a failed or needs-review source, or if the
Brave bridge is unavailable, the account is not an exact identity match, the
JSON is invalid, or David has not confirmed the write, do not save. Report the
repository processing result and mark the EAIC publication as pending; never
claim that the live client profile was updated.

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
