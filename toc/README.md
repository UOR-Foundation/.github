# UOR Foundation — Project Lifecycle

> **Maintained by:** [Technical Oversight Committee](../governance/GOVERNANCE.md)  
> **Related:** [GOVERNANCE.md](../governance/GOVERNANCE.md) · [STANDARDS.md](../STANDARDS.md) · [WISHLIST.md](./WISHLIST.md) · [CONTRIBUTOR_LADDER.md](./CONTRIBUTOR_LADDER.md)  
> **Bylaws:** Article VI §6.1 · Article XII  

This document defines how projects enter and advance through the UOR Foundation ecosystem. The lifecycle is modelled on the [CNCF TOC process](https://github.com/cncf/toc/blob/main/process/README.md) and will be immediately familiar to contributors from CNCF, Linux Foundation, and Kubernetes communities.

---

## Project stages

```
                        LOW BARRIER                    SIGNIFICANT BARRIER           CLEAR PATH
                        Low reward                     Due diligence begins          to graduation
                        Not compulsory                 Multi-org encouraged

  ┌──────────┐          ┌─────────────────────┐        ┌──────────────────┐        ┌───────────┐
  │ Wishlist │ ────────▶│       Sandbox        │───────▶│   Incubation     │───────▶│ Graduated │
  │   / idea │          │  Experiments         │        │  Stable + adopted│        │ Production│
  └──────────┘          │  Neutral home        │        │  TOC sponsor     │        │ ready     │
                        └─────────────────────┘        └──────────────────┘        └───────────┘
                               │                                │
                               │ (inactive)                     │ (inactive)
                               ▼                                ▼
                          ┌──────────┐                   ┌──────────┐
                          │ Archived │                   │ Archived │
                          └──────────┘                   └──────────┘
```

| Stage | What it signals | Adopters | Multi-org | Vote required |
|---|---|---|---|---|
| **Sandbox** | Viable UOR use case | None | No | No — TOC member approves |
| **Incubation** | Stable, gaining adoption | 1+ (dev/test) | No | Yes — simple majority |
| **Graduated** | Production-ready, well-governed | 3+ (≥1 production) | Yes (2+ orgs) | Yes — supermajority (⅔) |
| **Archived** | Inactive or superseded | — | — | Yes — simple majority |

---

## Sandbox

**The entry point.** For early-stage ideas, proofs of concept, and direct responses to [Wishlist](./WISHLIST.md) items. Low barrier — the goal is visibility and community feedback, not maturity.

**Criteria:**

- [ ] Clear UOR use case — reference the relevant spec section or API endpoint
- [ ] Public GitHub repository with a `README.md`
- [ ] At least one named maintainer (GitHub handle + organisation)
- [ ] `CODE_OF_CONDUCT.md` adopted (link to [`process/CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) is sufficient)
- [ ] Apache-2.0 licence (or approved alternative — see [`STANDARDS.md §6`](../STANDARDS.md))

**How to apply:**

1. Open a thread in `≡ projects` on the [UOR Foundation Discord](https://discord.gg/ZwuZaNyuve) with the tag `sandbox`
2. Use the [Sandbox application template](./templates/sandbox-application.md)
3. A TOC member responds within **7 days**

**On acceptance:**

- Project listed on `uor.foundation` with a `sandbox` badge
- Maintainer added to [`MAINTAINERS.md`](./MAINTAINERS.md)
- TOC assigns a point of contact

---

## Incubation

**Active building stage.** Projects that have moved beyond experimentation. Incubating projects demonstrate stability — slower rate of change, versioned APIs, and adoption beginning to emerge outside the core team.

**Criteria** — Sandbox criteria, plus:

- [ ] Minimum 30 days in Sandbox
- [ ] Active contributions from at least 2 individuals
- [ ] `GOVERNANCE.md` in the project repository
- [ ] `CONTRIBUTING.md` in the project repository
- [ ] At least one versioned release or versioned API (pre-1.0 is acceptable)
- [ ] At least 1 adopter — dev/test use is sufficient
- [ ] A TOC member willing to sponsor the application

**How to apply:**

1. Open a GitHub issue at [UOR-Foundation/.github](https://github.com/UOR-Foundation/.github/issues) titled `[Incubation] Project Name`
2. Use the [Incubation application template](./templates/incubation-application.md)
3. TOC assigns a sponsor within **14 days**
4. TOC votes within **14 days** of sponsor assignment — simple majority required

**On acceptance:**

- `incubation` badge on `uor.foundation`
- TOC sponsor assigned as the project's foundation point of contact
- [`MAINTAINERS.md`](./MAINTAINERS.md) updated with organisation affiliation

---

## Graduated

**Production-ready.** The signal that a project is stable, well-governed, and trusted for production use. Graduation requires demonstrable adoption across independent organisations, complete governance documentation, and multi-organisation maintainership.

**Criteria** — Incubation criteria, plus:

- [ ] Maintainers from at least 2 independent organisations
- [ ] `GOVERNANCE.md` complete — contributor ladder, voting process, maintainer onboarding/offboarding
- [ ] `MAINTAINERS.md` listing all maintainers with organisations and GitHub handles
- [ ] `SECURITY.md` with a responsible disclosure process
- [ ] `ADOPTERS.md` with at least 3 independent adopters — at least 1 in production
- [ ] Demonstrable ongoing contribution activity (commit history, merged PRs)

**How to apply:**

1. Open a GitHub issue at [UOR-Foundation/.github](https://github.com/UOR-Foundation/.github/issues) titled `[Graduation] Project Name`
2. Use the [Graduation application template](./templates/graduation-application.md)
3. Application open for **public comment — 2 weeks minimum**
4. TOC votes within **7 days** of comment period closing — supermajority (⅔) required

**On acceptance:**

- `graduated` badge and prominent listing on `uor.foundation` as production-ready
- Board notified
- [`MAINTAINERS.md`](./MAINTAINERS.md) updated

---

## Archived

**Inactive or superseded.** Archived projects are preserved and publicly accessible but no longer actively maintained or recommended.

**Archival is triggered by any one of:**

- No maintainer activity for 6 months
- Maintainer(s) request archival
- TOC determines the project is superseded or no longer safe to recommend

**Process:** TOC notifies the maintainer and allows **30 days** to respond. A new maintainer stepping forward within that window may keep the project active. Archived projects may return with a new maintainer and a simple majority TOC vote.

---

## Voting rules

All votes are conducted publicly via GitHub issue. Results are posted in `#governance` on Discord and logged in the [quarterly report](./QUARTERLY_REPORT.md).

| Decision | Threshold | Who votes |
|---|---|---|
| Sandbox acceptance | No formal vote | Single TOC member approves |
| Incubation | Simple majority | All TOC members |
| Graduation | Supermajority — ⅔ | All TOC members |
| Archival | Simple majority | All TOC members |
| TOC member election | Supermajority — ⅔ | Existing TOC + Board |

> **Conflict of interest:** Any TOC member directly affiliated with a project under review must declare the conflict in the GitHub issue and abstain from voting. Required by Bylaws §10.3 — see [`GOVERNANCE.md §9`](../governance/GOVERNANCE.md).

---

## Response-time commitments

| Action | SLA |
|---|---|
| Sandbox review | 7 days |
| Incubation sponsor assignment | 14 days from application |
| Incubation vote | 14 days from sponsor assignment |
| Graduation public comment | 2 weeks minimum |
| Graduation vote | 7 days after comment period closes |
| Archival notice to maintainer | 30 days before archival |

---

## The Wishlist

[`process/WISHLIST.md`](./WISHLIST.md) is the TOC's curated list of open problems the foundation needs the community to solve. Each entry includes a problem statement, a pointer to the relevant spec section or API endpoint, and a status (open / in progress / completed).

Sandbox submissions that address a Wishlist item are reviewed with priority.

To propose a new Wishlist item, open a GitHub issue tagged `wishlist-proposal`.

---

## Submission templates

| Template | Use when |
|---|---|
| [Sandbox application](./templates/sandbox-application.md) | Submitting a new project |
| [Incubation application](./templates/incubation-application.md) | Requesting promotion to Incubation |
| [Graduation application](./templates/graduation-application.md) | Requesting promotion to Graduated |

---

## Document history

| Version | Date | Notes |
|---|---|---|
| 1.0 | April 2026 | Initial version |

*Amendments require a supermajority TOC vote and are announced in `#governance` before merging.*
