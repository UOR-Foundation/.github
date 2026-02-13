# UOR Foundation — Repository and Contribution Standards

This document defines norms for all repositories in the [UOR-Foundation](https://github.com/UOR-Foundation) organization so that naming, versioning, and structure stay consistent.

## Repository naming

- **Format:** Lowercase, hyphenated (e.g. `atlas-embeddings`, `research`, `prism`).
- **Avoid:** CamelCase, underscores, or spaces in repo names.

## Rust crates (when applicable)

- **Package name** (in `Cargo.toml`): `kebab-case` (e.g. `atlas-embeddings`).
- **Library name** (e.g. `[lib] name = "..."`): `snake_case` (e.g. `atlas_embeddings`).

## License

- **Default:** MIT unless a specific project states otherwise (e.g. in its README or LICENSE file).
- Each repository should include a LICENSE file or clearly point to the org default.

## Where to contribute

- **Research monorepo:** [UOR-Foundation/research](https://github.com/UOR-Foundation/research) is the canonical home for research projects (e.g. atlas-embeddings). Open issues and pull requests there; use the project subdirectory (e.g. `atlas-embeddings`) in titles or descriptions when relevant.
- **Other repos** (e.g. `.github`, `prism`): Contribute via issues and PRs on the repository that owns the code.

## Versioning and releases

- **Libraries:** Use [Semantic Versioning](https://semver.org/) (e.g. `0.1.1`, `1.0.0`).
- **Research monorepo:** Versioning is per project (each project has its own `Cargo.toml` or version file). The monorepo itself does not have a single global version.
- **Releases:** Prefer per-project tags when cutting releases (e.g. `atlas-embeddings/v0.1.2` or `v0.1.2` for the sole crate in the repo). Document the tag format in the project’s README if it matters for tooling (e.g. CI).

## Branch strategy

- **Default branch:** `main`.
- **Optional:** Use a `develop` branch for integration if the project maintains one; document it in the repo README or CONTRIBUTING.

---

For the organization profile, tagline, and links, see the [organization profile](https://github.com/UOR-Foundation).
