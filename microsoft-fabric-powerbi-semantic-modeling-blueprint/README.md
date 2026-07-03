# Microsoft Fabric Power BI Semantic Modeling Blueprint

> Design a governed Power BI semantic layer over Microsoft Fabric Gold data.

## Status

**Planned scaffold**

The implementation contract is defined here. Model assets, fixtures, and deployment examples will be added before Active status.

## Business Scenario

A fictional Adventure Works Commercial Performance team needs consistent sales, margin, customer, return, inventory, and target metrics.

## Microsoft Services

- Microsoft Fabric Lakehouse and Warehouse
- SQL analytics endpoint
- Power BI semantic models
- Direct Lake
- Power BI Project and model metadata formats where appropriate
- Fabric Git integration and deployment pipelines
- Microsoft Purview integration points

## What Learners Will Build

1. Conformed star schema and table grain.
2. Date and role-playing dimensions.
3. Relationships, hierarchies, and business naming.
4. Explicit DAX measures and validation fixtures.
5. Direct Lake, Import, and DirectQuery decision guide.
6. Row-level security and test matrix.
7. Model certification and Dev/Test/Prod promotion.

## Planned Structure

- README and model design documentation.
- Architecture source and exported diagram.
- Semantic model metadata and DAX assets.
- SQL Gold views and sample data.
- Measure, relationship, and RLS tests.
- Demo script and lifecycle exercises.

## Release Gate

- [ ] Synthetic sales model and Gold contracts are included.
- [ ] Semantic model metadata and DAX assets are versionable.
- [ ] Measure fixtures and RLS tests pass.
- [ ] Storage mode and performance decisions are documented.
- [ ] Security, governance, deployment, and ownership are covered.
- [ ] Demo validates metrics, RLS, and promotion.

## Start Contributing

Open the [implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample plan](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. Verify current Fabric capacity, feature status, licensing, and deployment support.
