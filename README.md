# ci-smoke-lab-40
Throwaway sandbox for verifying the contribution + CI loop end to end.

## Build artifact

The CI workflow (`.github/workflows/ci.yml`) runs on demand via `workflow_dispatch`,
generates a short text file (`demo-build.txt`), and uploads it as a build artifact
named exactly **demo-build**. The prerequisite artifact for tomorrow's release-readiness
review is the `demo-build` artifact produced by this smoke-test run.
