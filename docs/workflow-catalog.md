# Workflow Catalog

> Source: automations_and_workflows / docs/workflow-catalog.md

Available reusable workflows and their purposes.

## CI Workflows

### `ci-node.yml`

Standard CI pipeline for Node.js projects.

**Inputs**:
- `node-version`: Node.js version (default: 20)
- `run-lint`: Whether to run linting (default: true)

### `ci-go.yml`

Standard CI pipeline for Go projects.

**Inputs**:
- `go-version`: Go version (default: 1.22)
- `run-tests`: Whether to run tests (default: true)

## CD Workflows

### `deploy-k8s.yml`

Deploy to Kubernetes using Helm.

**Inputs**:
- `environment`: Target environment (staging/production)
- `chart-path`: Path to Helm chart
- `values-file`: Path to values file

### `deploy-lambda.yml`

Deploy AWS Lambda functions.

**Inputs**:
- `function-name`: Lambda function name
- `runtime`: Lambda runtime (default: nodejs20.x)
