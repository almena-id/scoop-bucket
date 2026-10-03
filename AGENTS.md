# scoop-bucket — notes for contributors and agents

The Scoop bucket of Almena ID: `scoop bucket add almena https://github.com/almena-id/scoop-bucket`, then `scoop install almena/<manifest>`.

## Layout

- `bucket/almena.json` — the CLI. Written by the `distribute.yml` workflow of `almena-id/almena` (run by hand for a chosen release) from its `packaging/scoop/almena.json`, one commit per distribution (`almena <version>`), after installing it with Scoop from a local copy of this bucket.

## Rules

- Manifests are not edited here: change the template in the project's repository, and the next distribution brings it over.
- A manifest installs the project's released, signed binary untouched; nothing is built from source.
- Everything is written in English.
