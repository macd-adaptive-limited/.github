## What
<!-- One or two clear sentences: what does this PR change? -->

## Why
<!-- The reason for the change. Link the issue, spec or task. -->

## How it was tested
<!-- Commands run and their results (e.g. `npm test`: 43/43 pass), CI status, manual checks. -->

## Publication and side effects
- [ ] Files, history, metadata and test data intended for publication were checked for secrets, personal data, customer data and internal information.
- [ ] Money movement, email sending and other external effects stay behind their existing controls (OFF by default), or are N/A.
- [ ] Deployment or operations scripts remain marked PREPARATION/custody and are not wired to run automatically, or are N/A.

## Review needed
- [ ] Server review covers the exact final head SHA (record the SHA in a comment).
- [ ] BO review covers commercial, money, sending-authority or legal text changes, or is N/A.

## Risk and rollback
<!-- What could break and how to revert (revert commit, feature flag, migration rollback). -->

## Related
<!-- Issues, PRs, docs. -->

## Screenshots
<!-- Required if this changes UI. Delete this section otherwise. -->

## Batch and Actions minutes
<!-- Group the complete related task in this PR. Explain any split or exclusion. Avoid edit-by-edit pushes and obsolete reruns. -->
- [ ] Related changes are batched; unrelated risks are not mixed merely to enlarge the PR.
- [ ] Final head SHA and CI results are recorded; independent review covers that exact head.
- [ ] No required checks or security coverage are skipped. Workflow changes, if any, explain equivalent coverage and safe concurrency/path filtering.
- [ ] Merge does not authorize deployment, higher budgets or permission changes.

### Documentation-only repositories without CI

If the repository has no CI and no required checks, and the diff is documentation only, it may close with independent exact-head review and documented local validation, recording CI as N/A with the reason. This exception does not apply to code, configuration/workflows, permissions, or repositories with required checks.
