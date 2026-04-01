# Repository Boundary: `.github` and `UOR-Framework`

This document defines how the foundation governance repository (`.github`) and the framework implementation repository (`UOR-Framework`) fit together.

Canonical references:

- [Foundation entry point](./README.md)
- [Canonical sources](./CANONICAL_SOURCES.md)
- [UOR-Framework repository](https://github.com/UOR-Foundation/UOR-Framework)

## Purpose Split

| Repository | Primary Purpose | Canonical For |
|---|---|---|
| `.github` | Foundation governance and contributor policies | Governance rules, lifecycle process, contribution policy, code of conduct, security policy, standards |
| `UOR-Framework` | Framework specification and implementation | Framework spec, ontology artifacts, conformance logic, generated docs/site for the framework |

## Canonical Ownership

| Topic | Canonical Source |
|---|---|
| Foundation governance and decision process | [governance/GOVERNANCE.md](./governance/GOVERNANCE.md) |
| Project lifecycle stages and reviews | [toc/README.md](./toc/README.md) |
| Foundation-wide contribution and behavior policy | [CONTRIBUTING.md](./CONTRIBUTING.md), [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md), [SECURITY.md](./SECURITY.md) |
| UOR framework specification and artifacts | [UOR-Framework](https://github.com/UOR-Foundation/UOR-Framework) |

## Cross-Linking Rules

1. `.github` policy pages may reference framework docs, but policy authority remains in `.github`.
2. `UOR-Framework` docs should link back to `.github` for governance, lifecycle, conduct, and security policies.
3. Do not duplicate policy text in `UOR-Framework`; link to canonical `.github` files.
4. Do not duplicate framework spec details in `.github`; link to canonical `UOR-Framework` sources.

## Contributor Navigation

- Start at [README.md](./README.md)
- For policy/process questions, stay in `.github`
- For framework/spec/implementation questions, go to [UOR-Framework](https://github.com/UOR-Foundation/UOR-Framework)

## Rule

If documents conflict, the canonical source listed in `CANONICAL_SOURCES.md` prevails.
