# Azure Databricks Unity Catalog Blueprint

> Implement governed Azure Databricks data products with storage controls, environment isolation, least privilege, fine-grained access, audit, and lineage.

## Status

**Planned scaffold**

This folder defines the delivery contract. Runtime-specific examples will be added and validated before Active status.

## Business Scenario

A fictional Contoso Manufacturing platform publishes operations, quality, maintenance, and restricted cost data products across development and production environments.

## Microsoft Services

- Azure Databricks
- Unity Catalog
- ADLS Gen2
- Microsoft Entra ID
- Azure Key Vault
- Azure Monitor
- Optional Microsoft Purview integration points

## What Learners Will Build

1. Metastore, catalog, schema, and domain model.
2. Managed and external asset decision examples.
3. Storage credentials and external locations.
4. Group-based least-privilege grants.
5. Workspace and catalog isolation.
6. Row filters and column masks.
7. Audit, lineage, and periodic access review.

## Planned Structure

- README and governance documentation.
- Architecture source and exported diagram.
- SQL, notebooks, and infrastructure templates.
- Synthetic manufacturing data products.
- Permission and policy tests.
- Demo script and access exercises.

## Release Gate

- [ ] Synthetic manufacturing data products are included.
- [ ] Catalog, schema, storage, and grant scripts are implemented.
- [ ] Allowed and denied permission tests pass.
- [ ] Row filters and column masks are demonstrated safely.
- [ ] Audit, lineage, ownership, cost, and cleanup are documented.
- [ ] Demo shows environment isolation and access behavior.

## Start Contributing

Open the [implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample plan](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. Verify current Azure Databricks runtime, compute, privilege, and feature requirements.
