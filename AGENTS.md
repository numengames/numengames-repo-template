# Working in this repository

<!-- Replace every line marked TODO the day the repository is created from the template. -->

- **What it is:** TODO, one line (the same as the GitHub description).
- **Project:** TODO (Summa, Assets, Fleet, Engine, numinia.com, Numen Games or Hermes).
- **Human owner:** Pablo (@PabloFMM). He merges; agents open pull requests.
- **Published at:** TODO (a URL, or "not published").

## Rules

- The organisation's rules live in the Summa:
  [numinia-archive/AGENTS.md](https://github.com/numengames/numinia-archive/blob/main/AGENTS.md).
  This file only says what is particular to this repository.
- Pull requests, commits and comments are written in English.
- Work on a branch and open a pull request; never push to `main`.
- Changes under `.github/workflows/` need the CI gate app (`numinia-ci-puerta`); ask Pablo.
- Never commit a secret, key or personal data. The `secrets` check scans every pull request.
- Dependabot: security alerts only (repository settings). There is no `dependabot.yml`.

## Checks

- `secrets`: gitleaks over the commits of each pull request and over `main`.
- `workflow-lint`: actionlint when a workflow changes.
- When the repository gets a lockfile, add the shared `audit` workflow
  (`numengames/.github/.github/workflows/audit.yml`, pinned to a commit).
