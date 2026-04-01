# UOR Technical Oversight Committee (TOC) Process

v1.2 — UOR Foundation Project Lifecycle and Review Process

This document defines how projects move through lifecycle stages in the UOR Foundation.

Related docs: [README.md](../README.md) · [governance/GOVERNANCE.md](../governance/GOVERNANCE.md)

## Project Stages

- **Sandbox** - Early-stage projects with promising UOR relevance.
- **Incubation** - Projects showing stability, active maintenance, and growing adoption.
- **Graduated** - Mature, production-ready projects with strong governance and multi-organization confidence.
- **Archived** - Inactive, superseded, or no longer recommended projects.

| Stage | Primary Signal | Typical Evidence | Decision |
|---|---|---|---|
| **Sandbox** | Early fit and potential | Clear use case, active maintainer, basic repo hygiene | TOC approval |
| **Incubation** | Increasing maturity | Versioned releases/APIs, contribution activity, early adopters | TOC vote (simple majority) |
| **Graduated** | Production readiness | Multi-org maintainership, security posture, demonstrable adoption | TOC vote (2/3) |
| **Archived** | Inactivity or replacement | Sustained inactivity, maintainer request, or supersession | TOC vote (simple majority) |

## Project Lifecycle Process

Projects usually enter at **Sandbox** and then apply to **Incubation** and **Graduated**.

Core process:

1. **Application submitted** in [UOR Foundation `.github` issues](https://github.com/UOR-Foundation/.github/issues).
2. **TOC triage** for completeness and stage fit.
3. **Due diligence** on governance, quality, security, and adoption evidence.
4. **Public comment period** for Graduation.
5. **TOC decision** and publication.

Authority references:

- [UOR Governance Framework](../governance/GOVERNANCE.md)
- [UOR Foundation Bylaws](https://github.com/UOR-Foundation/.github/blob/main/governance/The_UOR_Foundation_Bylaws.pdf)

## How to Apply to Move Levels

### Applying to Sandbox

Submit a Sandbox request via [new issue](https://github.com/UOR-Foundation/.github/issues/new/choose). Include:

- Project purpose and UOR relevance
- Repository URL
- Named maintainer(s)
- Current state and expected next milestones

Minimum repository baseline:

- `README.md`
- `LICENSE`
- `CODE_OF_CONDUCT.md`

Standards reference: [Repository Standards](../STANDARDS.md).

### Applying to Incubation

Submit an issue titled: `[Incubation] <Project Name>`

Include evidence for:

- Ongoing maintenance and contributor activity
- Basic governance/contribution docs (`CONTRIBUTING.md`, maintainership clarity)
- Versioned release/API practices
- At least one adopter or clear integration usage

### Applying to Graduation

Submit an issue titled: `[Graduation] <Project Name>`

Include evidence for:

- Multi-organization maintainership
- Strong security posture and documented vulnerability handling
- Proven adoption and production-oriented operation
- Consistent release and review discipline

Graduation requires a **public comment period of at least 2 weeks** before voting.

## Timelines

Target service levels:

| Action | Target Timeline |
|---|---|
| Sandbox initial triage | Within 7 days |
| Incubation sponsor assignment | Within 14 days |
| Incubation vote after sponsor assignment | Within 14 days |
| Graduation public comment period | Minimum 14 days |
| Graduation vote after comment closes | Within 7 days |
| Archival response window | 30 days notice to maintainers |

Timelines are targets, not guarantees.

## Core References

- [Governance Framework](../governance/GOVERNANCE.md)
- [Contributing Guide](../CONTRIBUTING.md)
- [Code of Conduct](../CODE_OF_CONDUCT.md)
- [Security Policy](../SECURITY.md)
- [Repository Standards](../STANDARDS.md)
- [Discussions](https://github.com/orgs/UOR-Foundation/discussions)
