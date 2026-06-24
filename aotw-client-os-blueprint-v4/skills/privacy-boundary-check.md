---
purpose: check-client-privacy-trust-and-sharing-boundaries
updated: 2026-06-19
trigger: Run before client-facing outputs, public examples, third-party uploads, NotebookLM packs, screenshots, recordings, sensitive workflows, or new tool recommendations involving client data.
---

# Privacy Boundary Check

## Purpose

Protect client trust by identifying what information can be used, shared, transformed, uploaded, quoted, summarized, or generalized.

This skill should be run before producing anything client-facing, third-party-facing, public, or reusable across clients.

## Required Read

Read:

1. `privacy/data-boundaries.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `context/stakeholders.md`
5. relevant source material
6. relevant output draft
7. `tools/tool-stack.md` if third-party tools are involved

## Risk Categories

Classify the material:

- public
- client-approved
- internal AOTW only
- confidential client material
- sensitive personal material
- regulated or high-risk material
- credentials or access material
- unknown sensitivity

If sensitivity is unknown, treat as confidential until confirmed.

## Checkpoints

Ask:

- Who originally provided this information?
- Did the client approve this use?
- Is this needed for the output?
- Can it be summarized instead of quoted?
- Can it be anonymized?
- Can it be generalized into service IP?
- Will it be uploaded to a third-party tool?
- Does the third-party tool retain, train on, or expose data in a way that matters?
- Could this damage trust if seen by the client or a stakeholder?
- Could this reveal private strategy, weakness, or relationship dynamics?
- Could this expose customers, employees, finances, health, legal, or HR details?

## Redaction Rules

Redact or generalize:

- full names when not needed
- email addresses
- phone numbers
- private links
- customer names
- employee names
- financial details
- legal details
- health details
- passwords or credentials
- private stakeholder concerns
- raw transcript sections
- proprietary process details

Keep:

- the minimum context required to make the output useful
- client-approved names when necessary for direct client-facing work
- generalized patterns for internal playbooks

## Third-Party Tool Rules

Before using a third-party tool with client material:

1. Identify the data being uploaded.
2. Identify why upload is necessary.
3. Confirm whether the data can be reduced or anonymized.
4. Check whether the tool is approved or already in the stack.
5. Mark uncertainty if tool terms or access are not verified.
6. Recommend the safer version.

## Output

Produce:

```markdown
# Privacy Boundary Check

## Intended Use

## Material Reviewed

## Sensitivity Classification

## Allowed

## Not Allowed

## Needs Client Approval

## Redactions Required

## Third-Party Tool Concerns

## Safer Alternative

## Final Recommendation
```

For simple low-risk cases, a short version is acceptable:

```markdown
Privacy check: low risk. No sensitive client details included. Safe to share as drafted.
```

## Decision Values

Use:

- `Safe as drafted`
- `Safe after redaction`
- `Internal only`
- `Needs client approval`
- `Do not use`
- `Needs more information`

## Quality Check

Before finishing, verify:

- sensitive data is not accidentally included
- client-facing output does not reveal internal assessment
- reusable service IP is anonymized
- third-party upload is justified
- uncertainty is visible

