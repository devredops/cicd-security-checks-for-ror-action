# cicd-security-checks-for-ror-action

## Setting up this action


1. If you haven't already done so, create a `.github/workflows` folder in your
  repository (_this is where your actions will live_).
2. Now create a `.github/workflows/security-checks.yml` file with these contents:

    ```yaml
    name: security-checks

    on:
      push:
        branches:
          - main

    jobs:
      security-checks:
        runs-on: ubuntu-latest
        steps:
          - uses: devredops/cicd-security-checks-for-ror-action@main

    ```
