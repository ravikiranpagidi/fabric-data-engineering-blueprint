# Learning Paths

These paths combine active and planned blueprints into role-based sequences. Active folders can be used now. Planned folders describe the intended progression and become links when implementation is released.

## Path 1: Azure Lakehouse Engineer

**Target audience:** Azure data engineers, Databricks engineers, and developers moving from ETL projects to governed lakehouse delivery.

**Skills learned:**

- Metadata-driven ingestion with Azure Data Factory.
- ADLS Gen2 zone and data contract design.
- PySpark and Delta Lake medallion implementation.
- CDC and streaming reliability patterns.
- Unity Catalog permissions, storage governance, and lineage.
- Automated testing, deployment, release approval, and rollback.

**Recommended sequence:**

1. [Azure Lakehouse Starter Kit](../azure-lakehouse-starter-kit/README.md) - Active
2. `azure-streaming-cdc-blueprint` - Planned
3. `azure-databricks-unity-catalog-blueprint` - Planned
4. `azure-data-engineering-cicd-blueprint` - Planned

**Hands-on project:** Build a fictional Retail Operations Lakehouse that ingests daily master data and streams order and inventory changes. Govern plant and finance datasets with Unity Catalog, then promote the solution through Dev, Test, and Prod.

**Outcome:** You can explain and demonstrate how an Azure Lakehouse moves from initial ingestion to governed, automated production delivery.

## Path 2: Microsoft Fabric Analytics Engineer

**Target audience:** Microsoft Fabric learners, analytics engineers, Power BI developers, and Azure data engineers transitioning to Fabric.

**Skills learned:**

- OneLake and Lakehouse organization.
- Fabric pipelines, notebooks, Spark, and Delta tables.
- Eventstream, Eventhouse, KQL, dashboards, and operational alerts.
- Star schema and semantic model design.
- Direct Lake decision-making, DAX, RLS, and governed consumption.
- Conversational analytics source preparation and evaluation.

**Recommended sequence:**

1. [Fabric Data Engineering Blueprint](../fabric-data-engineering-blueprint/README.md) - Active
2. [Fabric Real-Time Intelligence Blueprint](../fabric-real-time-intelligence-blueprint/README.md) - Active
3. `microsoft-fabric-powerbi-semantic-modeling-blueprint` - Planned
4. `fabric-data-agent-copilot-analytics-blueprint` - Planned

**Hands-on project:** Build a fictional Service Operations analytics product with historical cases in a Lakehouse, live SLA events in Eventhouse, a governed Power BI semantic model, and a tested conversational analytics experience.

**Outcome:** You can build and present a Fabric solution that connects batch engineering, real-time operations, semantic modeling, and governed question answering.

## Path 3: Enterprise AI Data Architect

**Target audience:** Data architects, AI engineers, cloud architects, and technical leads designing governed AI-ready platforms.

**Skills learned:**

- Customer data product and identity resolution design.
- Consent, PII, quality, and access controls.
- Enterprise RAG ingestion, retrieval, grounding, and citation patterns.
- Azure AI Search index and retrieval design.
- Evaluation datasets, human feedback, monitoring, and responsible use.
- Governance catalog, lineage, glossary, and ownership workflows.

**Recommended sequence:**

1. [Azure Lakehouse Starter Kit](../azure-lakehouse-starter-kit/README.md) - Active foundation
2. `ai-ready-customer-360-blueprint` - Planned
3. `azure-data-governance-purview-blueprint` - Planned
4. `azure-openai-rag-enterprise-blueprint` - Planned
5. `fabric-data-agent-copilot-analytics-blueprint` - Planned comparison

**Hands-on project:** Build a fictional omnichannel Customer 360 product, catalog its business meaning and lineage, publish an approved knowledge corpus, and evaluate a secured assistant that retrieves only permitted content.

**Outcome:** You can design AI experiences whose answers are grounded in governed data products and evaluated against explicit quality criteria.

## Path 4: Power BI And Semantic Model Engineer

**Target audience:** Power BI developers, BI engineers, analytics engineers, and model owners responsible for trusted metrics.

**Skills learned:**

- Gold-layer dimensional design and table grain.
- Reusable facts, dimensions, measures, and business definitions.
- DAX measure design and validation.
- Direct Lake, Import, and DirectQuery decision criteria.
- RLS test design, model certification, deployment, and ownership.
- Preparing semantic models for reports and conversational analytics.

**Recommended sequence:**

1. [Fabric Data Engineering Blueprint](../fabric-data-engineering-blueprint/README.md) - Active
2. `microsoft-fabric-powerbi-semantic-modeling-blueprint` - Planned
3. `ai-ready-customer-360-blueprint` - Planned
4. `fabric-data-agent-copilot-analytics-blueprint` - Planned
5. `azure-data-engineering-cicd-blueprint` - Planned release track

**Hands-on project:** Create a fictional Commercial Performance model with certified sales, margin, inventory, and customer measures. Test RLS, deploy the model, and validate natural-language business questions against known results.

**Outcome:** You can own the semantic contract between engineered data and business decisions, including testing and lifecycle management.

## Path 5: Data Governance And Platform Lead

**Target audience:** Data architects, platform engineers, governance leads, data stewards, and technical managers.

**Skills learned:**

- Governance operating model and role design.
- Catalog, glossary, classification, lineage, and data product onboarding.
- Fabric and Databricks access boundaries.
- Unity Catalog grants, external locations, row filters, and column masks.
- CI/CD controls, approvals, environment isolation, and release evidence.
- Responsible measurement of platform adoption and community impact.

**Recommended sequence:**

1. [Azure Lakehouse Starter Kit](../azure-lakehouse-starter-kit/README.md) - Active architecture foundation
2. [Fabric Data Engineering Blueprint](../fabric-data-engineering-blueprint/README.md) - Active Fabric foundation
3. `azure-data-governance-purview-blueprint` - Planned
4. `azure-databricks-unity-catalog-blueprint` - Planned
5. `azure-data-engineering-cicd-blueprint` - Planned

**Hands-on project:** Define a fictional multi-domain analytics platform with data owners, stewards, consumers, catalog records, least-privilege access, lineage evidence, deployment approvals, and quarterly access review.

**Outcome:** You can connect governance policy to platform controls, operating processes, and evidence that teams can actually maintain.

## How To Use A Path

For each blueprint in a path:

1. Read the business scenario and architecture decision summary.
2. Run or review the implementation in the documented order.
3. Complete the validation and troubleshooting exercises.
4. Record one design decision and one alternative you rejected.
5. Deliver the demo without reading directly from the README.
6. Extend one dataset, rule, metric, or deployment check.
7. Share corrections or improvements through an issue or pull request.
