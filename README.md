# 37230

Reproduction repo for discussion [37230](https://github.com/renovatebot/renovate/discussions/37230).

## Current behavior

The `bun.lock` file is not being updated when Renovate creates a PR to update a dependency in `package.json`, causing the CI workflow that ensures `bun.lock` is up to date to fail. ([#3](../../pull/3), [#5](../../pull/5))  
Failing CI Log:  
<img width="675" height="219" alt="Failing CI Log" src="https://github.com/user-attachments/assets/8f094e02-c7fd-480f-a7f5-b67a23b76cfe" />


## Expected behavior

The `bun.lock` file should be updated to reflect the changes made to the `package.json` file by Renovate. So that the CI workflow passes.

## Logs

Relevant logs from the Renovate run that created the PR.

- For [#2](../../pull/2) and [#3](../../pull/3)
  - Minimal (Only [#3](../../pull/3) is included): [minilog_2025-09-11_09-19.log](revonate_logs/minilog_2025-09-11_09-19.log)
  - Full: [jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_09-19_7857da10-1d34-4e99-94fe-11e8a31156de.log](revonate_logs/jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_09-19_7857da10-1d34-4e99-94fe-11e8a31156de.log)
- For [#5](../../pull/5)
  - Minimal: [minilog_2025-09-11_11-52.log](revonate_logs/minilog_2025-09-11_11-52.log)
  - Full: [jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_11-52_bd25bd1b-f12f-4ece-bb4a-1f544928596d.log](revonate_logs/jimchen5209_renovate-bun-monorepo-reproduction_2025-09-11_11-52_bd25bd1b-f12f-4ece-bb4a-1f544928596d.log)
  
