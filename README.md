# minimal-reproduction-template

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).

Then replace the current `h1` with the Renovate Issue/Discussion number.

## Current behavior

The `bun.lock` file is not being updated when Renovate creates a PR to update a dependency in `package.json`, causing the CI workflow that ensures `bun.lock` is up to date to fail. ([#3](../pull/3), [#5](../pull/5))

## Expected behavior

The `bun.lock` file should be updated to reflect the changes made to the `package.json` file by Renovate. So that the CI workflow passes.

## Logs

Relevant logs from the Renovate run that created the PR.
- [jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_09-19_7857da10-1d34-4e99-94fe-11e8a31156de.log](revonate_logs/jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_09-19_7857da10-1d34-4e99-94fe-11e8a31156de.log) for [#2](../pull/2) and [#3](../pull/3)
- [jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_11-52_bd25bd1b-f12f-4ece-bb4a-1f544928596d.log](revonate_logs/jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_11-52_bd25bd1b-f12f-4ece-bb4a-1f544928596d.log) for [#5](../pull/5)
