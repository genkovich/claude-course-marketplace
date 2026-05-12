# Changelog

All notable changes to this marketplace are documented here. Format follows
[Keep a Changelog 1.1.0](https://keepachangelog.com/en/1.1.0/) and the project
adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2026-05-12

### Added

- `/review` command for inline PR reviews in pr-review-rules plugin
- Automated release-notes workflow using Claude project analysis and workflow_call triggers

## [1.0.0] - 2026-05-12

### Added

- Marketplace bootstrap via `.claude-plugin/marketplace.json` (name, owner, plugins[])
- `deploy-checklist` 1.0.0 — pre-deploy checklist enforcer (env diff, migrations dry-run, smoke endpoints, rollback plan, oncall heads-up)
- `pr-review-rules` 1.0.0 — PR review conventions (changelog entry, no console.log, test coverage, no formatting churn, security checklist)
- GitHub Actions `validate-plugins` workflow — marketplace.json schema check plus `claude plugin validate` matrix per plugin
