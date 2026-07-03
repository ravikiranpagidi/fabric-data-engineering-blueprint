# Diagram Brief

**Title:** Resilient Order And Inventory CDC Into Delta Lake

**Nodes:** Azure SQL change source, CDC publisher, Event Hubs, schema contract, Structured Streaming, Bronze, Silver merge, checkpoints, dead-letter path, replay, monitoring, consumer.

**Flow:** Changes enter Event Hubs with identity and ordering metadata. Streaming writes Bronze, deduplicates and merges Silver, records checkpoints, routes bad events, and supports replay.

**Layout:** Happy path center, recovery path below, contracts and monitoring above.

Planned assets:

- streaming-cdc-delta-flow-v1.excalidraw
- streaming-cdc-delta-flow-v1.png
