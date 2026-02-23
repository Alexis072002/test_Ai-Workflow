---
description: description: Convert PRD -> SPEC + BACKLOG (architecture, API contract, tasks). No coding.
---

# /orchestrate

## Operating mode
- NO CODING in this workflow.
- Use `docs/PRD.md` as source of truth.
- If PRD is missing info: add explicit assumptions in SPEC.

## Step 1 — Restate scope
Summarize PRD into 5 bullets:
- what we build
- who it serves
- core flows
- must-have features
- constraints

## Step 2 — Write docs/SPEC.md
Create/overwrite `docs/SPEC.md` with:

- Overview (one paragraph)
- Architecture (frontend/backend + folder/module plan)
- Data model (entities + relationships)
- API contract (routes, auth, payloads, errors)
- Non-functional requirements (performance, security basics)
- Assumptions & decisions (explicit)
- Definition of Done (DoD)

### Default stack (unless PRD says otherwise)
- Frontend: Next.js (App Router) + Tailwind + TypeScript
- Backend: NestJS + TypeScript
- Validation: Zod (FE), class-validator or Zod (BE)
- Auth: JWT (if needed)
- DB: SQLite for local dev (Prisma optional)

## Step 3 — Write docs/BACKLOG.md
Create/overwrite `docs/BACKLOG.md`:

Rules:
- Ordered by dependencies
- Tasks are small and testable
- Each task includes:
  - Owner: Frontend | Backend | QA | Release
  - Acceptance criteria
  - Likely files/folders

## Step 4 — Handoff
Say: "SPEC + BACKLOG generated. Next: /build"
Then run: /build