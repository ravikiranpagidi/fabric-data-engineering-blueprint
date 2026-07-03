# Architecture Gallery Plan

## Purpose

The architecture gallery should help a learner compare complete Microsoft Data and AI patterns at a glance, then open the source diagram and implementation folder for detail.

## Root Gallery Structure

The root gallery should contain one tile per active blueprint with:

- Blueprint name and status.
- Fictional business scenario.
- One PNG overview.
- Link to Excalidraw source.
- Link to the topic README.
- Primary Microsoft services.
- One sentence describing the design decision the diagram teaches.

Planned blueprints should appear in a separate roadmap table without empty image placeholders.

## Diagram Asset Standard

Each topic should include:

```text
diagrams/
|-- README.md
|-- architecture-overview.excalidraw
|-- architecture-overview.png
|-- architecture-detail.excalidraw       optional
|-- architecture-detail.png              optional
|-- architecture-overview.drawio         optional
`-- architecture-presentation.pptx       optional
```

Use Mermaid in README files for accessible, version-friendly flow diagrams. Use Excalidraw and PNG when the diagram needs service icons, trust boundaries, zones, or presentation polish.

## Visual Standards

- Use official Microsoft architecture icons in exported presentation diagrams when license and source requirements permit.
- Keep icon source and retrieval date in `diagrams/README.md`.
- Use left-to-right flow for primary data or request paths.
- Put governance, identity, monitoring, and CI/CD on supporting lanes.
- Separate trust boundaries and environments visibly.
- Label arrows with protocols, data format, or control action where useful.
- Avoid decorative gradients, 3D effects, and unreadable icon clouds.
- Use no more than seven major nodes in the overview diagram.
- Provide a more detailed second diagram instead of overcrowding the overview.
- Export PNG at a readable width of at least 1600 pixels.

## File Naming Convention

`<topic>-<view>-v<major>.{excalidraw,png,drawio,pptx}`

Example: `azure-rag-request-flow-v1.png`

## Active Blueprint Gallery Entries

| Blueprint | Diagram Title | Key Flow |
| --- | --- | --- |
| Fabric Data Engineering | Retail Banking Lakehouse From Source To Dashboard | CSV sources to pipeline, Lakehouse Files, Bronze, Silver, Gold, SQL endpoint, semantic model, dashboard |
| Fabric Real-Time Intelligence | Smart Logistics Operational Event Flow | Producers to Eventstream, Eventhouse, KQL, dashboard, Activator, Lakehouse history |
| Azure Lakehouse Starter Kit | Retail Customer Analytics Azure Lakehouse | Sources to ADF, ADLS Gen2, Databricks medallion, Unity Catalog, SQL and Power BI |

## Planned Topic Diagram Briefs

### Azure OpenAI RAG Enterprise

**Diagram title:** Governed Enterprise RAG Request And Feedback Flow

**Nodes:** Approved document sources, ingestion function, content storage, Azure AI Search, Azure OpenAI, secured API, user application, Entra ID, Key Vault, Application Insights, evaluation and feedback store.

**Arrow flow:** Documents move through parsing and indexing to search. User identity reaches the API. The API retrieves permitted chunks, sends grounded context to the model, returns citations, and records telemetry and feedback. Evaluation reads test questions and compares expected evidence.

**Layout:** Ingestion lane across the top, runtime request lane across the center, governance and operations lane across the bottom.

**Excalidraw notes:** Use separate trust boundaries for content preparation and runtime. Make retrieval and generation visually distinct. Show feedback returning to evaluation, not directly retraining a model.

### Fabric Power BI Semantic Modeling

**Diagram title:** Fabric Gold Data To Governed Power BI Semantic Model

**Nodes:** Lakehouse or Warehouse Gold tables, SQL analytics endpoint, semantic model, DAX measures, RLS roles, certified reports, Excel or downstream consumers, Git, deployment pipeline stages.

**Arrow flow:** Gold tables feed the semantic model using the selected storage mode. Measures and security govern report queries. Git tracks metadata. Deployment stages promote the model and reports.

**Layout:** Data and model flow left to right, lifecycle flow below, security band across model and consumers.

**Excalidraw notes:** Show Direct Lake, Import, and DirectQuery as decision branches rather than simultaneous defaults.

### Azure Data Governance Purview

**Diagram title:** Governed Data Product Discovery And Access Workflow

**Nodes:** Data sources, ingestion and transformation, Microsoft Purview catalog and map capabilities, glossary, classifications, owners and stewards, access workflow, consumers, evidence and issue register.

**Arrow flow:** Technical metadata and lineage enter the catalog. Owners add business context. Consumers discover a product, review classification, request access, and receive governed access through the platform owner. Issues return to owners and stewards.

**Layout:** Data estate on the left, governance services in the center, people and workflows on the right.

**Excalidraw notes:** Distinguish metadata flow from data flow using line styles. Do not imply that cataloging automatically grants data access.

### Azure Databricks Unity Catalog

**Diagram title:** Unity Catalog Isolation And Fine-Grained Access Model

**Nodes:** Entra groups, Dev and Prod workspaces, Unity Catalog metastore, catalogs, schemas, managed storage, storage credential, external location, tables and volumes, row filters, column masks, audit and lineage.

**Arrow flow:** Groups receive privileges on catalogs and schemas. Workspaces bind to allowed catalogs. External locations reference credentials and storage. Policies apply at query time. Audit and lineage capture governed use.

**Layout:** Identity on the left, workspace and metastore in the center, storage and data objects on the right, audit below.

**Excalidraw notes:** Clearly show the difference between cloud storage permissions and Unity Catalog privileges.

### Fabric Data Agent And Copilot Analytics

**Diagram title:** Governed Conversational Analytics With Fabric Data Agent

**Nodes:** Business user, Fabric data agent, instructions and example questions, Lakehouse, Warehouse, semantic model, KQL database, permission enforcement, query execution, diagnostics, evaluation set, feedback.

**Arrow flow:** User question reaches the agent. The agent selects an approved source, applies user permissions, generates a read query, executes it, returns a concise answer, and records diagnostics. Evaluation compares answers with expected business results.

**Layout:** Request flow left to right, data sources below the agent, governance and evaluation above and below.

**Excalidraw notes:** Label the data sources as selected governed sources. Show read-only behavior and user-context permissions. Mark feature status when the diagram is published.

### Azure Data Engineering CI/CD

**Diagram title:** Multi-Platform Data Engineering Promotion Flow

**Nodes:** Developer branch, pull request, validation checks, artifact package, Dev environment, integration tests, approval, Test, release approval, Prod, smoke tests, monitoring, rollback reference.

**Arrow flow:** Code moves through validation and immutable packaging. The same artifact is parameterized per environment. Failed checks return to the branch. Failed production smoke tests invoke rollback or corrective release.

**Layout:** Main promotion pipeline left to right with quality gates above and evidence stores below.

**Excalidraw notes:** Use different border styles for automated and human gates. Show ADF, Databricks, Fabric, SQL, and Power BI as deployable asset groups within an artifact boundary.

### AI-Ready Customer 360

**Diagram title:** Consent-Aware Customer 360 Data Product For BI And AI

**Nodes:** Commerce, service, loyalty, consent, campaign and web sources, identity resolution, survivorship, Customer 360 Gold model, quality score, consent policy, semantic model, feature table, approved AI context projection.

**Arrow flow:** Source identities are standardized and matched. Survivorship produces a golden profile. Quality and consent controls govern downstream projections. BI, ML, and AI consume separate contracts.

**Layout:** Sources on the left, identity and profile pipeline in the center, governed consumption branches on the right.

**Excalidraw notes:** Do not show one unrestricted customer record feeding every consumer. Make consent and purpose-specific projections visible.

### Azure Streaming CDC

**Diagram title:** Resilient Order And Inventory CDC Into Delta Lake

**Nodes:** Azure SQL change source, CDC publisher, Event Hubs, schema contract, Structured Streaming, Bronze append table, Silver current-state merge, checkpoint store, dead-letter path, replay, monitoring, Power BI or operational consumer.

**Arrow flow:** Changes enter Event Hubs with event identity and ordering metadata. Streaming writes immutable Bronze, deduplicates and merges Silver, records checkpoints, routes poison events, and supports replay. Monitoring measures lag and reconciliation.

**Layout:** Happy path across the center, recovery path below, contracts and monitoring above.

**Excalidraw notes:** Label at-least-once delivery assumptions where used. Show idempotency and reconciliation explicitly.

## Presentation Slides

Optional PowerPoint architecture slides should be editable and contain:

1. Business problem.
2. Architecture overview.
3. Primary data or request flow.
4. Security and governance controls.
5. Deployment and operations.
6. Demo sequence.
7. Decisions and alternatives.
