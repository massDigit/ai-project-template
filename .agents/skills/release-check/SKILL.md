---
name: release-check
description: Procedure for executing pre-release checklist and production readiness audit
---

# Release Check Procedure

## 1. Static Verification
- Run typecheck and linter via `.ai/WORKFLOW.md`.
- Ensure zero errors or warnings.

## 2. Test Suite Completion
- Run full test suite (unit, integration, e2e).
- Confirm 100% pass rate.

## 3. Build & Artifact Verification
- Execute production build command (`npm run build` or equivalent).
- Verify bundle size and absence of build warnings.

## 4. Documentation & State Synchronization
- Confirm `docs/` and `.ai/DECISIONS.md` are up to date.
- Update `.ai/STATE.md` with new release version tag.
