---
description: description: Universal kickoff: Discovery interview -> PRD -> handoff to orchestration
---

# /kickoff

## Operating mode
- NO CODING in this workflow.
- Ask max 5 questions per batch.
- After each batch, restate understanding + assumptions.
- Prefer making reasonable assumptions over stalling, but label them clearly.

## Step 1 — Ask for the initial pitch
Ask the user:
"Give me a 2–4 sentence pitch: what is it, for whom, and why now?"

Then continue with interview questions.

## Step 2 — Discovery interview (repeatable loop)
Use this checklist to guide your questions:
- Problem & value proposition
- Target users & contexts
- Core flows (happy path)
- Must-have vs nice-to-have features
- Data involved (entities, roles, permissions)
- Success criteria (what “done” means)
- Constraints (budget=0, tech preferences, timeline)
- Risks, unknowns, out-of-scope

Rules for questions:
- Ask up to 5 questions at a time
- If the user is unsure, propose 2–3 options and ask them to pick
- After each batch, output:
  1) Current understanding (bullets)
  2) Assumptions (if any)
  3) Next questions (max 5)

Stop the interview when you can write a complete PRD.

## Step 3 — Write docs/PRD.md
Create/overwrite `docs/PRD.md` with:

- Summary (5 bullets max)
- Target users (1 primary persona, 1 secondary)
- User journeys (3–5)
- Features: Must / Should / Could
- Non-goals
- Success metrics (north star + 2 supporting)
- Constraints (budget/time/platform/security/legal)
- Risks & unknowns
- Open questions (max 5)

## Step 4 — Handoff
Say: "PRD generated. Next: /orchestrate"
Then run: /orchestrate