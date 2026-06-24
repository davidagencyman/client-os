---
title: Research Principles for AOTW Client OS Repos
purpose: research-backed-design-notes
version: 4.0
updated: 2026-06-19
---

# Research Principles

This note records the design principles behind the v4 blueprint.

It is not client-facing. It helps the AOTW team and AI agents understand why the package is structured the way it is.

## Sources Used

- LangGraph workflows and agents: https://docs.langchain.com/oss/python/langgraph/workflows-agents
- OpenAI Agents SDK handoffs: https://openai.github.io/openai-agents-python/handoffs/
- OpenAI prompt engineering guide: https://developers.openai.com/api/docs/guides/prompt-engineering
- OpenAI reasoning best practices: https://developers.openai.com/api/docs/guides/reasoning-best-practices
- Claude Code skills: https://code.claude.com/docs/en/skills
- Claude Code subagents: https://code.claude.com/docs/en/sub-agents
- Anthropic prompt engineering best practices: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices
- Anthropic Agent Skills article: https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills
- Anthropic context engineering for agents: https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- Google People + AI Guidebook: https://pair.withgoogle.com/guidebook/

## Design Conclusions

### 1. Use a Router, Not Manual Skill Guessing

Modern agent systems use routing, handoffs, or orchestrator-worker patterns.

For this repo system, the practical equivalent is `_skills/operating-router.md`.

The router:

- classifies the situation
- decides which skills to run
- runs the minimum useful cascade
- explains what it ran and why

This avoids requiring the AOTW team member to say "run process, then follow-up, then update action registry."

### 2. Use Complete Skill Files, Not Skill Names

Claude skills and agent skill systems work best when procedural knowledge is packaged as explicit instructions and resources.

Therefore, the blueprint must include full skill bodies. A generated repo should not ask the model to invent skill instructions.

### 3. Separate Operating Memory From Source Material

The old `_inbox/` pattern forced an unnecessary manual step: upload transcript into the repo, then run a skill.

The better workflow is:

- attach transcript directly to Codex or Claude Code
- let the router classify it
- run `process-source-material`
- write structured repo memory

### 4. Check Live Context Before Preparing

Calendar and Gmail often contain newer truth than the repo.

Any session prep should:

1. read `context/client-contact.md`
2. check Calendar
3. check Gmail
4. reconcile with repo state

This prevents wrong names, wrong meeting duration, stale agendas, and missed client updates.

### 5. Make Human Tone an Operating Requirement

The system should not produce dry consulting agendas.

It should infer:

- emotional state
- trust level
- frustration
- confidence
- overwhelm risk
- how the client should feel by the end

The call prep output should protect the client from overload and create one clear adoption step.

### 6. Track Adoption, Not Demos

A tool working during a session is not adoption.

The repo must distinguish:

- built with consultant
- used alone by client
- not yet habitual
- blocked by tool
- blocked by behavior
- ready for automation
- not ready for automation

### 7. Treat Privacy as a First-Class Workflow

Privacy checks should not be afterthoughts.

Any sharing, NotebookLM source, client-facing artifact, new connector, sensitive transcript, or public example should trigger `_skills/privacy-boundary-check.md`.

### 8. Keep Session Duration Explicit

AOTW one-on-one sessions default to 90 minutes.

Call prep should not silently produce a 30-minute agenda unless Calendar or engagement terms prove the session is shorter.

### 9. Make Output Verifiable

Each skill should say:

- what it read
- what it changed
- what it skipped
- what needs attention

This makes the system auditable and easier to improve.

