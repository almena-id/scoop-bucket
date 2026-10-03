# Contributing

Thanks for helping with the Scoop manifest of Almena ID. By taking part you agree
to follow the [Code of Conduct](CODE_OF_CONDUCT.md). Security issues go
through [SECURITY.md](SECURITY.md), never through public issues.

## Where a change goes

The manifests here are not edited by hand. Each one is written by the
`distribute.yml` workflow of the project it installs, from a template in
that project, when a release is distributed. [AGENTS.md](AGENTS.md) lists
which project writes which file.

- A problem with how a package installs or what it installs: open an issue,
  or a pull request against the template in the project's repository (for
  the CLI, `packaging/scoop/almena.json` in
  [almena-id/almena](https://github.com/almena-id/almena)).
- A problem with the program itself: an issue in the project's repository.
- A change to this repository's own files (README, these documents): a pull
  request here.

## Checking a manifest locally

With the template filled in (a real version and its checksum) as
`bucket/almena.json` in a clone of this repository, on Windows:

```powershell
scoop bucket add almena-local "$PWD"
scoop install almena-local/almena
almena --version
```

Scoop adds a local clone through git, so the manifest has to be committed
there first.

## Pull requests

Keep a pull request to one topic, describe what it changes and why, and link
the issue it addresses. Everything is written in English. By contributing you
agree that your contribution is licensed under the
[Apache License 2.0](LICENSE), as the rest of the repository.
