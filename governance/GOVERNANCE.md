# UOR Foundation - GitHub Governance Framework

| Property | Value |
|----------|-------|
| Version | 2.1 |
| Status | Active |
| Scope | `github.com/UOR-Foundation` |
| Owner | UOR Foundation Organization Owners |
| Review cycle | Quarterly |

Related docs: [README.md](../README.md) · [CONTRIBUTING.md](../CONTRIBUTING.md) · [SECURITY.md](../SECURITY.md)

---

## 1. Purpose & Scope

This document defines how the UOR Foundation runs projects on GitHub.

It exists to keep the process clear, fair, and fast so contributors can build with confidence.

It applies to:

- all repositories in `UOR-Foundation`
- all contributors and maintainers
- code, docs, and release artifacts

## 2. Glossary

| Term | Meaning |
|------|---------|
| Issue | A tracked task, bug, or proposal. |
| Pull Request (PR) | A proposed change to merge. |
| Maintainer | A person responsible for a repository. |
| Owner | A foundation admin with final authority. |
| Tier | A repository class that sets minimum controls. |

## 3. Guiding Principles

- **Open by default** - decisions and process are visible.
- **Clear ownership** - every repo has maintainers.
- **Review before merge** - no direct pushes to protected branches.
- **Bias for action** - small PRs, fast feedback, practical decisions.

## 4. Roles, Teams & Escalation

### 4.1 Roles

| Role | Core responsibility |
|------|---------------------|
| Organization Owner | Final governance decisions and escalations |
| Repository Maintainer | Day-to-day repo health, review, and release |
| Contributor | Proposes and ships improvements through PRs |

### 4.2 Escalation

| Situation | Path |
|-----------|------|
| PR stalled | Ping maintainers, then escalate to owners |
| Technical disagreement | Maintainer decides; owners resolve tie/dispute |
| Conduct issue | Report via `SECURITY.md`; owners handle response |

## 5. Repository Classification

| Tier | Use case | Minimum expectation |
|------|----------|---------------------|
| Tier 1 | Core framework and critical specs | Strong review and verification |
| Tier 2 | Implementations and integrations | Standard review and CI |
| Tier 3 | Docs, websites, and presentation repos | Basic review and CI |
| Tier 4 | Early experiments | Clear status and basic hygiene |

## 6. Repository Standards

### 6.1 Required Files

| File | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|------|:------:|:------:|:------:|:------:|
| `README.md` | Req | Req | Req | Req |
| `LICENSE` | Req | Req | Req | Req |
| `CONTRIBUTING.md` | Req | Req | Rec | Opt |
| `CODE_OF_CONDUCT.md` | Req | Req | Rec | Opt |
| `SECURITY.md` | Req | Req | Opt | Opt |
| `.github/CODEOWNERS` | Req | Req | Opt | Opt |
| CI workflow | Req | Req | Rec | Opt |

### 6.2 Branch Protection Rules

| Rule | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|------|:------:|:------:|:------:|:------:|
| PR required | Yes | Yes | Yes | Rec |
| Review required | 2 | 1 | 1 | Opt |
| Status checks required | Yes | Yes | Yes | Opt |
| Force push allowed | No | No | No | No |

## 7. Change Control & Contribution Workflow

### 7.1 Standard Workflow

1. Open or pick an issue.
2. Create a branch from `main`.
3. Make focused commits.
4. Open a PR linked to the issue.
5. Pass review and CI.
6. Merge and close.

### 7.2 Branch Naming

Use:

- `feat/{issue#}-{description}`
- `fix/{issue#}-{description}`
- `docs/{issue#}-{description}`
- `chore/{issue#}-{description}`

### 7.3 Commit Messages

Use [Conventional Commits](https://www.conventionalcommits.org/):

`type(scope): description`

### 7.4 Emergency / Hotfix Procedure

For critical issues:

1. Declare severity and notify maintainers/owners.
2. Open a minimal fix PR.
3. Require at least one reviewer and green CI.
4. Release patch quickly.
5. Add follow-up notes within 48 hours.

## 8. Version Management & Releases

- Use [Semantic Versioning](https://semver.org/) for Tier 1-2 repositories.
- Keep `CHANGELOG.md` updated.
- Publish release notes for every tagged release.

## 9. Peer Review & Quality Assurance

| Requirement | Tier 1 | Tier 2 | Tier 3 |
|-------------|:------:|:------:|:------:|
| Minimum reviewers | 2 | 1 | 1 |
| CI required | Yes | Yes | Yes |
| Documentation update when needed | Yes | Yes | Yes |

## 10. Cross-Repository Coherence

- Use consistent naming and topic tags.
- Keep README links current.
- Prefer shared workflow patterns where practical.

## 11. Repository Lifecycle Management

| Stage | Description |
|-------|-------------|
| Proposal | New repo or project idea under review |
| Active | Normal development |
| Maintenance | Limited updates and fixes |
| Archived | Read-only historical state |

Archive only when inactive or superseded, and keep context in README.

## 12. Security & Incident Response

Security policy lives in [SECURITY.md](../SECURITY.md).

Baseline response targets:

| Severity | Acknowledge | Patch target |
|----------|-------------|--------------|
| Critical | 24h | 72h |
| High | 24h | 7 days |
| Medium | 48h | 30 days |

## 13. Intellectual Property & Licensing

- Default license policy is MIT across foundation repos.
- Exceptions require owner approval and clear documentation.
- Current known exception: [UOR-Framework](https://github.com/UOR-Foundation/UOR-Framework) uses Apache-2.0.

---

For day-to-day work, start at [README.md](../README.md) and [CONTRIBUTING.md](../CONTRIBUTING.md).
