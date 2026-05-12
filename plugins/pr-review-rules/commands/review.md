---
description: "Run the team PR review checklist against $ARGUMENTS"
---

Apply the team's PR review conventions to the pull request referenced by `$ARGUMENTS` (a GitHub PR URL or PR number). Walk every rule below and report violations with file paths and line numbers; if clean, say so explicitly.

- CHANGELOG entry required for any change touching `src/` or public API
- No `console.log`, `print()` debug calls, or commented-out code blocks
- Test coverage required for every new branch in business logic — at least one happy path and one error path
- No unrelated formatting churn — reject PRs that mix logic with bulk reformatting
- Security checklist for any change touching auth, PII, or external network calls — list the threat model in the PR description

Output a numbered list of violations grouped by rule. End with a one-line verdict: `APPROVE`, `REQUEST_CHANGES`, or `COMMENT`.
