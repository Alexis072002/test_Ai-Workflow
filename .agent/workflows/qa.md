---
description: description: QA gate. Verify against SPEC + DoD. Block release if failing.
---

# /qa

## Step 1 — Verify
Check against `docs/SPEC.md` and DoD:
- correctness & edge cases
- typing & linting
- validation & error handling
- auth checks (if applicable)
- secrets safety (no .env committed)


## Step 2 — Output issues
Return:
- Ranked issues
- Exact fixes (file-level)
- Minimal tests to add

## Step 3 — Gate
- If issues exist: apply fixes (or send back to /build) then re-run /qa.
- If clean: run /release