<!--
Org-wide PR template for QS-AlgoTrading (inherited from the .github repo).
Individual repos may override with their own .github/pull_request_template.md.
QuantStand is a live real-money platform — the checklist is the point.
-->

## What this PR does

<!-- 1–2 sentences. Explain the WHY, not just the what. -->

## Checklist

- [ ] **CI green** on this branch; branch updated from `main` before merge.
- [ ] **CHANGE_CHECKLIST** run for anything that alters platform behavior
      (`QuantStand-Ant/docs/CHANGE_CHECKLIST.md`): single source of truth,
      every consumer reads it, live path provably untouched when only
      paper/shadow changed.
- [ ] **Docs updated in this PR** (same-PR rule): roadmap/task list, runbooks,
      decision records, and any index/registry row for artifacts added here.
- [ ] **No secrets** — templates ship blank; real values only in
      `/etc/quantstand/*.env` on the server.
- [ ] **Pre-registered criteria respected** — for strategy/research changes:
      acceptance thresholds frozen before evaluation; the holdout stays sealed.

## Related

- Decision record (`DEC-QNT-NNN`) / task / session id:
- Compass principle or ADR touched (if any):

## Risk and rollback

<!-- Name the rollback path. Default: `git revert <merge-sha>` (auto-deploys the
     previous state). If a migration/server unit/live-money surface is touched,
     state the specific rollback steps. -->
