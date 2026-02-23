---
description: description: Execute BACKLOG incrementally. Builders must follow PRD/SPEC/API contract.
---

# /build

## Guardrails
- Builders MUST NOT invent requirements beyond PRD/SPEC/API.
- If blocked by missing info:
  1) propose 2 options
  2) pick one as an explicit assumption
  3) record it in `docs/SPEC.md` under "Assumptions & decisions"
- Keep changes incremental (small PR-sized steps).
- After each batch, ensure the project can run locally.

## Step 1 — Select tasks
Pick the next 1–3 unchecked tasks from `docs/BACKLOG.md`.

## Step 2 — Execute tasks
Implement them in the codebase (create files, edit, run commands as needed).

## Step 3 — Update BACKLOG
Mark completed tasks as done.
Add brief notes if decisions were made.

## Step 4 — Stop condition (important)
Stop building when:
- MVP core flow works end-to-end
- `npm install` + `npm run dev` works for the relevant apps
- basic smoke test passes

Then run: /qa