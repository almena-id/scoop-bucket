# Security policy

## Reporting a vulnerability

Please report vulnerabilities privately through GitHub: on the repository of
the project a manifest installs (for the CLI,
[almena-id/almena](https://github.com/almena-id/almena)), open the
**Security** tab and choose **Report a vulnerability**. Do not open a public
issue, pull request or discussion about it.

Include what you can of:

- the manifest and its version;
- what an attacker can do, and under which configuration;
- steps or a proof of concept to reproduce it.

We aim to acknowledge a report within 3 working days and to agree on a
disclosure date with you once the issue is understood. We credit reporters in
the release notes unless you prefer otherwise.

## Supported versions

Only the latest version of each manifest receives fixes.

## Scope

In scope, among others:

- a manifest that downloads from somewhere other than the project's GitHub
  releases, or with a checksum that does not match the release's
  `SHA256SUMS`;
- a manifest that installs files beyond what its package needs, or with unsafe
  permissions.

Out of scope:

- vulnerabilities in the programs installed, which belong to their own
  repositories;
- vulnerabilities in Scoop itself.
