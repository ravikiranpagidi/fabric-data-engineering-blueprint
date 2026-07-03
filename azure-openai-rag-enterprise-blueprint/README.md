# Azure OpenAI Enterprise RAG Blueprint

> Build a governed retrieval-augmented generation solution with secured access, citations, evaluation, monitoring, and human feedback.

## Status

**Planned scaffold**

This folder defines the implementation contract for a future active blueprint. It does not yet represent a deployable production solution.

## Business Scenario

A fictional Contoso Service organization needs a knowledge assistant that answers support questions using approved product manuals, service bulletins, and troubleshooting procedures.

## Microsoft Services

- Azure OpenAI
- Azure AI Search
- Blob Storage or ADLS Gen2
- Azure Functions
- API Management
- Microsoft Entra ID
- Azure Key Vault
- Application Insights and Azure Monitor

## What Learners Will Build

1. Document ingestion and content normalization.
2. Chunking and metadata enrichment.
3. Search index and hybrid retrieval.
4. Grounded response API with citations.
5. User and content access enforcement.
6. Evaluation dataset and quality scoring.
7. Human feedback and operational telemetry.

## Planned Structure

- README and implementation documentation.
- Architecture source and exported diagram.
- Source application and infrastructure templates.
- Synthetic document corpus.
- Retrieval, security, and evaluation tests.
- Demo script and extension exercises.

## Release Gate

- [ ] Synthetic knowledge corpus is included.
- [ ] Ingestion, indexing, retrieval, and API code are implemented.
- [ ] Retrieval and answer evaluation tests pass.
- [ ] Identity, content safety, prompt injection, and data handling risks are documented.
- [ ] Cost, monitoring, cleanup, and troubleshooting guidance are complete.
- [ ] Demo shows citations, denied content behavior, evaluation, and telemetry.

## Start Contributing

Review [the implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample contract](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. Verify current service names, model availability, regional support, pricing, and security requirements before implementation.
