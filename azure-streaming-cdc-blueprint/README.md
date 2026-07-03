# Azure Streaming And CDC Blueprint

> Implement resilient change data capture and streaming ingestion into Delta-based analytical layers.

## Status

**Planned scaffold**

This folder defines the implementation contract. Source CDC capabilities, connector support, and runtime requirements will be verified during development.

## Business Scenario

A fictional Contoso Retail Operations team tracks order changes, payment status, product updates, and inventory availability with low-latency analytics.

## Microsoft Services

- Azure SQL CDC concepts
- Azure Event Hubs
- Azure Databricks Auto Loader and Structured Streaming
- Delta Lake
- Azure Monitor
- Optional Microsoft Fabric Real-Time Intelligence comparison

## What Learners Will Build

1. CDC event envelope and schema contract.
2. Event publishing and Event Hubs ingestion.
3. Immutable Bronze stream.
4. Deduplication and current-state Silver merge.
5. Checkpoints, late data, and schema evolution.
6. Dead-letter, replay, and reconciliation.
7. Monitoring, alerting, and serving tables.

## Planned Structure

- README and streaming design documentation.
- Architecture source and exported diagram.
- Event generator and Structured Streaming notebooks.
- Synthetic CDC event samples and schemas.
- Idempotency, replay, and reconciliation tests.
- Demo script and recovery exercise.

## Release Gate

- [ ] Synthetic CDC publisher and event contracts are included.
- [ ] Bronze and Silver streaming paths are implemented.
- [ ] Duplicate, late, malformed, and replay scenarios pass.
- [ ] Checkpoint, recovery, monitoring, and reconciliation are documented.
- [ ] Security, cost, cleanup, and operational ownership are covered.
- [ ] Demo proves inserts, updates, failure recovery, and current state.

## Start Contributing

Open the [implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample plan](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. Verify current source CDC, Event Hubs, Databricks runtime, and connector requirements.
