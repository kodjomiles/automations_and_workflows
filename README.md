# Automations and Workflows

> Source: automations_and_workflows / README.md

This repository contains reusable GitHub Actions workflows and automation scripts for the platform team.

## Contents

| Directory       | Description                              |
|-----------------|------------------------------------------|
| `.github/`      | Reusable workflow definitions            |
| `scripts/`      | Automation scripts for CI/CD pipelines   |
| `docs/`         | Usage guides and contribution guidelines |

## Usage

Reference workflows from other repositories:

```yaml
jobs:
  deploy:
    uses: kodjomiles/automations_and_workflows/.github/workflows/deploy.yml@main
    with:
      environment: production
```

## Contributing

See `docs/contributing.md` for guidelines on adding new workflows.
