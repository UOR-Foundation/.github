# Contributing to the UOR Foundation

Thank you for your interest in contributing. This guide covers the workflow, conventions, and expectations for all contributors.

Canonical references: [Foundation entry point](./README.md) · [Canonical sources](./CANONICAL_SOURCES.md)

## Quick Start

1. Pick an issue or open one.
2. Create a branch from `main`.
3. Open a PR linked to the issue.

## Before You Start

1. Read the [Code of Conduct](CODE_OF_CONDUCT.md).
2. Read the [Governance Framework](governance/GOVERNANCE.md), especially Sections 2 (Glossary), 3 (Principles), and 7 (Change Control).
3. Read the repository-specific README for build instructions and context.

## Contribution Workflow

Every change follows this pipeline:

1. **Issue** — File or find a GitHub Issue describing the bug, feature, or improvement.
2. **Branch** — Create a feature branch from `main`:
   - Features: `feat/{issue#}-{short-description}`
   - Fixes: `fix/{issue#}-{short-description}`
   - Docs: `docs/{issue#}-{short-description}`
3. **Develop** — Make changes in small, logical commits following the commit standard below.
4. **Pull Request** — Open a PR against `main` using the [PR template](/.github/pull_request_template.md). Link the originating Issue.
5. **Review** — Address reviewer feedback. All CI checks must pass.
6. **Merge** — A Maintainer merges via squash-and-merge. The Issue auto-closes.

## Commit Message Standard

All commits follow [Conventional Commits v1.0.0](https://www.conventionalcommits.org/):

```
type(scope): description
```

| Element | Required | Values |
|---------|----------|--------|
| **type** | Yes | `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `proof`, `ci`, `perf` |
| **scope** | Recommended | Module or subsystem name |
| **description** | Yes | Imperative mood, lowercase, no trailing period, max 72 chars |

Example: `feat(atlas): add E7 augmentation construction`

## License

By submitting a Pull Request, you represent that you have the right to license your contribution under the repository's license (MIT by default) and that it does not infringe any third-party intellectual property rights.

## Getting Help

Post questions in the repository's Discussion tab or in the [organization-level Discussions](https://github.com/orgs/UOR-Foundation/discussions).
