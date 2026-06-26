---
purpose: prepare-a-humane-high-leverage-client-coaching-session
updated: 2026-06-26
trigger: Run when preparing for an upcoming client coaching call, session, check-in, workshop, or renewal conversation.
---

# Call Prep

## Purpose

Create a session prep file that lets the AOTW consultant run a focused, humane, genuinely useful coaching session.

The bar is high: the prep file should be good enough that even a consultant who is not a technical expert can run the session like a seasoned, certified coach. The instructions carry the expertise so the human does not have to.

The prep file has two jobs:

1. A short, scannable strategy brief so the consultant knows exactly where the session is going and why.
2. A full, authentic, read-aloud script for the entire session so the consultant is never stranded, even with a brain freeze.

## How To Use This Skill (Order Matters)

Run these steps in order. Do not skip steps 2 and 3, and do not draft the file before they are done.

1. Confirm session duration (90 minutes by default).
2. Gather live context from connected tools and the repo. Hard gate before anything else.
3. Form a clear point of view, then ask the consultant a few questions and wait for answers. Hard gate before drafting.
4. Do real technical research so every instruction is accurate and current.
5. Draft the prep file: short summary first, then the brief, then the full read-aloud script.
6. Report what you did.

## Step 1 - Confirm Duration

A standard AOTW one-on-one coaching session is 90 minutes (one and a half hours).

Plan for the full 90 minutes unless Calendar or `context/engagement.md` proves a different duration.

If the duration is uncertain, build a 90-minute plan and state that the duration was assumed.

Never default to a 30-minute call. Never produce a plan that cannot realistically fill the confirmed duration.

## Step 2 - Gather Live Context Before Anything (Required)

Do not draft the file, and do not even ask the consultant your questions, until you know what is actually true right now.

When connected tools are available:

1. Read `context/client-contact.md` first for canonical names, emails, company, aliases, and meeting title patterns.
2. Check Calendar first. Find the upcoming session's real date, time, duration, title, guests, location, and any attachments. Note reschedules or new invites.
3. Check Gmail second. Look for recent client messages, unreturned asks, promised materials, scheduling changes, new questions, and tone shifts since the last session.
4. Check Drive and other connected tools when relevant. Look for new shared documents, materials, or notes tied to this client.

Then read the repo files in the Required Read list below.

Reconcile live truth against repo state. Connected tools usually hold newer truth than the repo. If they disagree, trust the live source and note the conflict.

Do not infer the client from the repo slug.

If connected tools are unavailable, say so in the freshness section and continue from repo evidence and any attached source material.

### Required Read

Read:

1. `context/client-contact.md`
2. `context/client-profile.md`
3. `context/engagement.md`
4. `context/stakeholders.md`
5. `context/writing-style-profile.md`
6. `status/current-status.md`
7. `status/action-registry.md`
8. `status/outcomes-scorecard.md`
9. `status/practice-plan.md`
10. `tools/tool-stack.md`
11. `privacy/data-boundaries.md`
12. recent `sessions/`
13. active `workstreams/`
14. relevant `research/` or `learning/` files

## Step 3 - Form A Point Of View, Then Ask The Consultant (Required, Do Not Skip)

This is the most important behavior. Never draft the agenda before checking direction with the consultant.

First, build a clear recommendation from everything you gathered:

- the long-term arc this engagement is moving toward
- the one main focus you would choose for this session, and why
- the smallest practice step that would create real adoption
- anything risky, stuck, or sensitive to handle with care

Then ask the consultant a few short questions and wait. Address the consultant directly and by name.

Ask 3 to 5 questions. Each question should:

- state your recommended direction or assumption first, so the consultant can simply confirm
- explicitly invite a better idea the consultant may already have
- be answerable in one line

Cover at least:

- the main focus for this session (your pick, open to theirs)
- the long-term goal you are steering toward (confirm or correct)
- anything the consultant already wants to do or show on this call
- the client's current mood, pressure, or constraints you cannot see in the files
- anything to avoid or not open yet

Example phrasing:

> David, here is the direction I am leaning for this session. Tell me if you agree or if you have a better move.
>
> 1. Main focus: I would spend the working block on getting [X] running end to end, because [reason]. Agree, or is there something you would rather drive?
> 2. Long-term goal: I am steering toward [Y] over the next few sessions. Still the right arc?
> 3. Anything you already have in mind you want to do on this call that I should build around?
> 4. How is the client doing right now? Anything tender, busy, or frustrating I should plan around?
> 5. Anything we should not open yet?

Present the questions, then stop. Do not draft the file until the consultant answers.

If the consultant says to just draft it, or gives the go-ahead without details, proceed using your stated assumptions and label them clearly in the brief.

## Step 4 - Research For Technical Accuracy (Required When Teaching A Tool)

Everything the consultant will teach must be correct and current. A confident-sounding wrong instruction breaks trust faster than anything.

When the session involves any platform, tool, feature, or workflow:

1. Read official documentation, the vendor help center, and release notes. Prefer primary sources over blog posts or memory.
2. Verify the current interface: exact menu names, button labels, where things sit on the screen, and the real order of steps. Products change their UI often.
3. Write precise, on-screen, click-by-click navigation the consultant can both follow and narrate to the client. For example: "click your profile picture in the top right, then Settings, then Connected Apps." This is what lets a non-expert confidently guide the client's mouse on screen.
4. Note the version or date you verified, and flag anything that may have moved since.
5. For deep or volatile questions, run `technical-research-brief.md` and cite it.

Do not write navigation or UI steps from memory when the product behavior may have changed. Verify, then write.

## Step 5 - Draft The Prep File

### Output Location

Create or update:

```text
sessions/YYYY-MM-DD-call-prep.md
```

If the call date is unknown, use:

```text
sessions/next-call-prep.md
```

### Readability Rules

- Open with a short Bottom Line the consultant can read in under a minute. A few lines only: the focus, the long-term goal, the one practice step, and the headline of what changed. No long preamble.
- Keep the brief scannable. Short sections, short lines, and bold only the few things that matter.
- Put the full read-aloud script after the brief, so the consultant gets the point fast and has the script ready when needed.

### Output Structure

```markdown
# Session Strategy Brief - [Client / Date]

## Bottom Line (Read This First)

- Session: [date, time, duration]
- Main focus: [one line]
- Long-term goal this serves: [one line]
- The one practice step to land: [one line]
- What changed since last time: [one line]

## Freshness Check

## Direction Confirmed With Consultant

## Long-Term Arc

## Current Client State

## What Changed Since Last Session

## Commitments To Close (AOTW And Client)

## Main Session Focus

## Secondary Threads (At Most Two)

## Do Not Open Unless Necessary

## Session Flow ([duration] Minutes)

## Technical How-To (Verified Steps)

## Full Session Script (Read Aloud If You Freeze)

### 0-10 min - Reconnect
### 10-20 min - Close Loops
### 20-60 min - Main Working Block
### 60-75 min - Apply To A Real Task
### 75-85 min - Decide The Practice Step
### 85-90 min - Recap And Close

## Tiny Practice Step

## Follow-Up To Prepare

## Privacy Or Trust Watchouts

## Research Needed / Sources Verified

## Desired Impression To Leave
```

## The Read-Aloud Script (Most Important New Part)

The script is what lets a non-expert run an expert session. Write it so the consultant can read any part out loud and still sound like a real, warm human.

Requirements:

- Cover the entire confirmed duration, block by block, matching the session flow. No block left without words to say.
- Write it in natural spoken language, in the consultant's own voice. Pull tone and phrasing from `context/writing-style-profile.md` when it captures how the consultant speaks.
- Make it authentic, not robotic. Warm, plain, and real. No corporate filler, no hype, no "AI transformation" language.
- The consultant should be able to read any line verbatim if they freeze, and it should still sound like them.
- Write out the exact words for teaching each step, tied to the verified click-by-click navigation from Step 4, so the consultant narrates the screen accurately.
- Write out the actual questions to ask the client, in full sentences, woven into the right blocks.
- Write out how to introduce and assign the practice step, and the warm recap and close.
- Use light stage directions in brackets for actions, such as *[share your screen]*, *[pause and let them try it]*, *[wait for their answer]*.
- For likely client reactions, include a short alternative line or two, such as if the client is stuck, skeptical, or excited, so the consultant is never stranded.
- Keep it realistic for the time. Do not over-pack the script. Leave room for the client to talk.

## Session Flow Shape

Scale this to the confirmed duration. For a normal 90-minute session:

- 0 to 10 minutes: reconnect, confirm what changed, surface urgent context
- 10 to 20 minutes: close loops from prior commitments
- 20 to 60 minutes: main working block
- 60 to 75 minutes: apply it to one real client task
- 75 to 85 minutes: decide the next tiny practice and ownership
- 85 to 90 minutes: recap, confirm follow-up, leave calm

Adjust only when the client context demands it. Do not make a packed agenda that cannot fit.

## Strategy Rules

A good session brief should answer:

- What is the long-term arc of this client engagement?
- What changed since the last session?
- What did AOTW promise?
- What did the client promise?
- What is stuck?
- What should not be opened yet?
- What is the highest leverage focus for this session?
- What will make the client feel seen and not overwhelmed?
- What small practice step would create real adoption?
- What needs research before the call?
- What privacy or trust boundary matters?

## Focus Selection

Choose one primary session focus. Choose at most two secondary threads.

Rank by:

1. time-sensitive client commitment
2. trust or privacy risk
3. blocker preventing adoption
4. workflow the client is likely to use this week
5. high-value but contained automation or assistant behavior
6. long-term capability building
7. interesting research or tool exploration

If there are too many active threads, recommend running `workstream-pruner.md`.

## Tone

The brief and the planning notes are for the AOTW consultant, not the client. Use direct, practical language.

The read-aloud script is for the client's ears. Use the consultant's warm, human voice.

Keep the client human throughout. Include stress, confidence, trust, and working style where relevant.

Avoid hype, generic AI transformation language, and long lists of possible tools.

## Freshness Check Wording

Be specific:

- Calendar checked: yes/no/unavailable
- Gmail checked: yes/no/unavailable
- Drive/other tools checked: yes/no/unavailable
- meeting date and duration found: exact value or assumed 90 minutes
- most recent relevant email date if available
- consultant questions asked and answered: yes/no, with the direction confirmed
- source files used

## Quality Check

Before finishing, verify:

- duration is confirmed and the source is stated
- live tools were checked before drafting
- the consultant's questions were asked and answered, or an explicit go-ahead was given, before drafting
- the Bottom Line is readable in under a minute
- every technical step was verified against current documentation, with source and date
- the read-aloud script covers the whole session and sounds like a real human
- there is one clear practice step
- privacy and trust boundaries are respected

## Do Not Do

Do not:

- draft the file before checking live connected tools
- draft the file before asking the consultant and getting answers, unless told to proceed
- assume a 30-minute call unless evidence says so
- write UI or navigation steps from memory when the product may have changed
- produce a robotic, teleprompter-sounding script
- bury the point under a long summary
- prepare a generic agenda
- ignore unreturned email asks
- ignore open AOTW commitments
- fill the call with tool demos
- suggest too many parallel experiments
- use client-facing language without checking privacy and tone
- make research claims without current verification when product behavior may have changed
