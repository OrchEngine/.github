# OrchEngine organization defaults

This public repository holds organization-wide GitHub defaults for repositories in the
[OrchEngine](https://github.com/OrchEngine) organization.

## Issue types

Issue types are defined at the organization level: `Task`, `Bug`, and `Feature`.

- **Feature** — new capability or meaningful improvement.
- **Bug** — unexpected behavior or a regression.
- **Task** — chore, docs, quality, tooling, refactor, or gate.

The forms in `.github/.github/ISSUE_TEMPLATE` apply to every repository that does not
define its own templates. The extra `.github` level is required for organization-wide
defaults; this is not a normal repository's `.github/ISSUE_TEMPLATE` path. Each form sets
the matching issue type automatically, and blank issues are disabled. CLI and API callers
bypass the forms, so they must pass the type explicitly.

## Labels

Issue types own "kind". Labels own area (`runtime`, `editor`, `storage`, `build`,
`tooling`, `docs`, `zig`, `quality`), priority (`p0`, `p1`, `p2`), and phase (`demo`,
`migration`, `design`).

Do not add `feature`, `bug`, or `chore` labels to new issues. Keep existing labels for
history and saved filters.

## Notes

This repository must remain **public** for GitHub to use it as an organization-wide
default. It contains no secrets or private project material.

The canonical issue policy is in [AGENTS.md](AGENTS.md).
