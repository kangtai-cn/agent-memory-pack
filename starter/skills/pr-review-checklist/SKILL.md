# Skill: pr-review-checklist

## Name
`pr-review-checklist`

## When to use
User asks to review a PR/diff, prepare a review comment, or self-check before opening a PR. Works for React/TS and Java/Spring changes.

## Inputs
- Diff, PR URL, or list of changed files
- Intended behavior / linked issue

## Outputs
- Structured review: Summary / Blockers / Suggestions / Nits / Test gaps
- Explicit go / no-go recommendation

## Steps
1. Restate the PR goal in one sentence; flag scope creep if files unrelated to the goal changed.
2. Walk the checklist:
   - [ ] Correctness & edge cases
   - [ ] Input validation at boundaries
   - [ ] AuthZ on new/changed endpoints
   - [ ] Secrets / PII in diff or logs
   - [ ] Error handling & user-visible messages
   - [ ] N+1 / obvious perf footguns
   - [ ] a11y for new UI controls
   - [ ] Tests updated for behavior changes
   - [ ] Migrations safe for rolling deploy
   - [ ] API breaking changes documented
3. Separate **blockers** (must fix) from **suggestions**.
4. Do not bikeshed naming unless it harms clarity or breaks conventions in AGENTS.md.
5. End with: Approve / Approve with nits / Request changes.

## Done when
- Review is actionable and tied to evidence in the diff
