# GitHub Metrics Setup

The profile README works without this workflow.

To enable `assets/github-metrics.svg`:
1. Create a GitHub personal access token with the required repository/read permissions.
2. In the `KdMenon007` profile repository go to Settings → Secrets and variables → Actions.
3. Add a repository secret named `METRICS_TOKEN`.
4. Run the `GitHub Metrics` workflow manually once.

Do not commit the token into any file.
