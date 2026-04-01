# Documentation Spec

This spec standardizes terminology, structure, and linking for this repository.

## Standard Terms

- **Canonical Source**: The authoritative document for a document type.
- **Entry Point**: The main page contributors should read first (`README.md`).
- **Policy Page**: Foundation-wide rule or process document (`GOVERNANCE`, `CODE_OF_CONDUCT`, `SECURITY`, `CONTRIBUTING`, `STANDARDS`, `TOC`).
- **Repository Boundary**: The explicit ownership split between `.github` (policy/process) and `UOR-Framework` (spec/implementation).

## Linking Standard

- Every policy page should link back to `README.md`.
- Every policy page should link to `CANONICAL_SOURCES.md`.
- Use relative links for local files.
- Use full `https://` links for external pages.

## Governance Standard

1. Update the canonical source first.
2. Update dependent links and references.
3. Keep language concise and consistent.
4. If documents conflict, the canonical source listed in `CANONICAL_SOURCES.md` prevails.
