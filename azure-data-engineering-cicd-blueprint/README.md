# Azure Data Engineering CI/CD Blueprint

> Deliver repeatable validation and Dev/Test/Prod promotion for Microsoft data engineering assets.

## Status

**Planned scaffold**

This folder defines the cross-platform delivery contract. Deployment examples will be added incrementally and tested against supported platform capabilities.

## Business Scenario

A fictional Fabrikam Analytics Platform team manages coordinated releases across Azure Data Factory, Azure Databricks, Microsoft Fabric, SQL, and Power BI.

## Microsoft Services

- GitHub Actions
- Azure DevOps
- Azure Data Factory
- Azure Databricks
- Microsoft Fabric Git integration and deployment pipelines
- Power BI deployment capabilities
- Azure Key Vault
- Azure CLI

## What Learners Will Build

1. Branch and environment strategy.
2. Pull request validation.
3. Artifact packaging and environment parameters.
4. Dev, Test, and Prod promotion.
5. Automated and human approval gates.
6. Smoke tests and release evidence.
7. Rollback and corrective release process.

## Planned Structure

- README and lifecycle documentation.
- Architecture source and exported diagram.
- GitHub Actions and Azure DevOps YAML.
- Deployment and parameter scripts.
- Synthetic pipeline assets.
- Validation, smoke, and rollback tests.
- Demo script and release exercise.

## Release Gate

- [ ] At least two platform deployment examples are implemented.
- [ ] Validation runs before deployment.
- [ ] The same artifact is promoted with environment parameters.
- [ ] Secrets and service connections are documented safely.
- [ ] Smoke tests, approvals, rollback, and release evidence are included.
- [ ] Platform limitations and manual steps are explicit.

## Start Contributing

Review the [implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample plan](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. Verify current deployment support for each artifact type before implementation.
