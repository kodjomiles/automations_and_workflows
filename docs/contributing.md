# Contributing Guide

> Source: automations_and_workflows / docs/contributing.md

Guidelines for adding or modifying workflows in this repository.

## Workflow Standards

1. **Naming**: Use kebab-case for workflow files (e.g., `deploy-to-prod.yml`).
2. **Inputs**: Document all inputs with descriptions and defaults.
3. **Secrets**: Never hardcode secrets; use `secrets` context.
4. **Outputs**: Export meaningful outputs for downstream jobs.

## Testing

Before merging:

1. Test the workflow in a feature branch.
2. Verify it works with `workflow_call` from a test repository.
3. Check for security issues with `actionlint`.

## Review Process

- All changes require approval from the platform team.
- Breaking changes must be announced in Slack before merging.
