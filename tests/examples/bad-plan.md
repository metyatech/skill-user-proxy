# Example bad plan

## Objective

Fix a bug in `index.js`.

## Plan

1. Read `index.js`.
2. Edit `index.js` to fix the bug.
3. Report completion.

## Review Results (skill-user-proxy)

- **Completeness**: No. Missing verification steps (tests/manual check).
- **Thoroughness**: Surface-level plan.
- **Known error patterns**:
  - **Shallow analysis**: Declaring work "complete" without evidence.
  - **Missing post-deployment**: If `index.js` is part of a globally linked package, it needs a rebuild/restart check.

**Decision**: FLAG

- **Concern**: The plan lacks any verification steps (e.g., running tests or manual verification) to ensure the bug is actually fixed.
- **Concern**: No mention of post-deployment steps if this is a globally linked tool.
