# UOR Technical Oversight Committee (TOC) Process

v1.1 — UOR Foundation Project Lifecycle and Review Process

This document defines how projects enter, progress, and exit lifecycle stages in the UOR Foundation. It follows a structure similar to the CNCF TOC process while remaining specific to UOR governance, standards, and operating practices.

## Table of Contents

- [Project Stages](#project-stages)
- [Project Lifecycle Process](#project-lifecycle-process)
- [How to Apply to Move Levels](#how-to-apply-to-move-levels)
- [Timelines](#timelines)
- [Project Resources and Guideposts](#project-resources-and-guideposts)
- [Additional Information](#additional-information)

## Project Stages

The UOR TOC defines four lifecycle stages:

- **Sandbox** - Early-stage projects with promising UOR relevance.
- **Incubation** - Projects showing stability, active maintenance, and growing adoption.
- **Graduated** - Mature, production-ready projects with strong governance and multi-organization confidence.
- **Archived** - Inactive, superseded, or no longer recommended projects.

| Stage | Primary Signal | Typical Evidence | Decision Method |
|---|---|---|---|
| **Sandbox** | Early fit and potential | Clear use case, active maintainer, basic repo hygiene | TOC review and approval |
| **Incubation** | Increasing maturity | Versioned releases/APIs, contribution activity, early adopters | TOC vote (simple majority) |
| **Graduated** | Production readiness | Multi-org maintainership, security posture, demonstrable adoption | TOC vote (supermajority, 2/3) |
| **Archived** | Inactivity or replacement | Sustained inactivity, maintainer request, or supersession | TOC vote (simple majority) |

## Project Lifecycle Process

Projects typically enter at **Sandbox**, then may apply to move to **Incubation** and **Graduated**. At each transition, the TOC performs due diligence appropriate to the stage.

High-level process:

1. **Application submitted** in [UOR Foundation `.github` issues](https://github.com/UOR-Foundation/.github/issues).
2. **TOC triage** for completeness and stage fit.
3. **Sponsor assignment** for Incubation/Graduation applications.
4. **Due diligence review** of governance, quality, security, and adoption evidence.
5. **Public comment period** (required for Graduation).
6. **TOC vote** and decision publication.

All process decisions and escalations align with:

- [UOR Governance Framework](../governance/GOVERNANCE.md)
- [UOR Foundation Bylaws](https://github.com/UOR-Foundation/.github/blob/main/governance/The_UOR_Foundation_Bylaws.pdf)

## How to Apply to Move Levels

### Applying to Sandbox

Submit a Sandbox request via [new issue](https://github.com/UOR-Foundation/.github/issues/new/choose) and include:

- Project purpose and UOR relevance
- Repository URL
- Named maintainer(s)
- Current state and expected next milestones

Minimum expected repository baseline:

- `README.md`
- `LICENSE`
- `CODE_OF_CONDUCT.md`

Reference standards: [Repository Standards](../STANDARDS.md).

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

Graduation applications include a **public comment period of at least 2 weeks** before voting.

## Timelines

The TOC targets the following service levels:

| Action | Target Timeline |
|---|---|
| Sandbox initial triage | Within 7 days |
| Incubation sponsor assignment | Within 14 days |
| Incubation vote after sponsor assignment | Within 14 days |
| Graduation public comment period | Minimum 14 days |
| Graduation vote after comment closes | Within 7 days |
| Archival response window | 30 days notice to maintainers |

These are target timelines, not guarantees. Complexity, evidence quality, and reviewer availability may extend review duration.

## Project Resources and Guideposts

Core UOR governance and operational references:

- [Governance Framework](../governance/GOVERNANCE.md)
- [Governance Changelog](../governance/CHANGELOG.md)
- [Contributing Guide](../CONTRIBUTING.md)
- [Code of Conduct](../CODE_OF_CONDUCT.md)
- [Security Policy](../SECURITY.md)
- [Repository Standards](../STANDARDS.md)
- [Foundation Governance Overview](../README.md)

Community and collaboration channels:

- [UOR Foundation GitHub Discussions](https://github.com/orgs/UOR-Foundation/discussions)
- [UOR Foundation Discord](https://discord.gg/ZwuZaNyuve)

## Additional Information

### Conflict of Interest

Any TOC member directly affiliated with a project under review must declare the conflict and abstain from voting on that decision.

### Governance Authority

The TOC operates under delegated authority within UOR Foundation governance. Final organizational authority remains with the Board of Directors, as defined by the Bylaws.

### Amendments to This Process

Changes to this process should be proposed through a pull request in `.github`, reviewed publicly, and approved through the TOC governance process.
