# GitHub Metrics Setup

The profile README works without the metrics workflow. The metrics panel is optional.

1. Save the workflow as `.github/workflows/github-metrics.yml` in `KdMenon007/KdMenon007`.
2. Create a personal access token with only the permissions required by the Metrics action and the repositories/features you want it to read.
3. In the repository, open **Settings → Secrets and variables → Actions → New repository secret**.
4. Name the secret `METRICS_TOKEN` and paste the token value. Never commit the token to a file.
5. Open **Actions → GitHub Metrics → Run workflow**.
6. Confirm `assets/github-metrics.svg` was generated and committed.
7. The scheduled run is `00:00 UTC` daily, which is `05:30` in India Standard Time.

## Security notes

- Never paste the token into the README or workflow YAML.
- If the workflow fails, inspect the Actions log and verify token scope and repository permissions.
- For stronger supply-chain control, review the third-party action and pin it to a reviewed version or commit SHA instead of using `@latest`.
- This workflow generates GitHub metrics. It does not update TryHackMe or Hack The Box rankings or room counts.
