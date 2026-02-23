---
description: description: Prepare local release instructions + optional CI/Docker. No paid services required.
---

# /release

## Step 1 — Write docs/RELEASE.md
Create/overwrite `docs/RELEASE.md` with:
- How to run locally (dev)
- How to run locally (prod-like)
- Env vars template (no secrets)
- Scripts to run: lint/test/build/start
- Optional Docker steps (if you created Dockerfiles)
- CI outline (GitHub Actions): lint + test + build
- Smoke tests checklist
- Ready-to-ship checklist

## Step 2 — Final summary
Summarize:
- What’s ready
- How to test locally
- Next improvements