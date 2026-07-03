# GitHub Wiki Plan

## Wiki Role

The root README is the repository landing page. Topic READMEs explain how to use an implementation. The Wiki should serve as the cross-topic learning portal, decision handbook, and navigation layer.

The Wiki should not duplicate every topic document. It should connect concepts, paths, patterns, and troubleshooting information across blueprints.

## Page Plan

### Home

**Purpose:** Orient new visitors and show active blueprints, planned topics, and recommended learning paths.

**Key sections:** Repository promise, status legend, active catalog, path selector, architecture overview, quick start, contributor entry points, disclaimer.

**Content:** Link directly to active implementations. Keep planned topics in a roadmap table. Show one cross-platform Mermaid diagram.

### How To Use This Repo

**Purpose:** Explain how to study, run, validate, demonstrate, and extend a blueprint.

**Key sections:** Choose a path, prerequisites, read versus run modes, validation, demo practice, extension exercises, issue and contribution flow.

**Content:** Provide a repeatable seven-step method and distinguish conceptual review from cloud deployment.

### Learning Paths

**Purpose:** Route learners by role and outcome.

**Key sections:** Azure Lakehouse Engineer, Fabric Analytics Engineer, Enterprise AI Data Architect, Power BI Semantic Model Engineer, Governance and Platform Lead.

**Content:** Target audience, sequence, skills, hands-on capstone, outcome, active and planned status.

### Architecture Gallery

**Purpose:** Compare active reference architectures visually.

**Key sections:** Active diagrams, pattern comparison, diagram source links, presentation use, contribution standard.

**Content:** One PNG and short decision summary per active blueprint. Link to Excalidraw source and topic README.

### Azure Lakehouse

**Purpose:** Connect ADF, ADLS Gen2, Databricks, Delta Lake, CDC, Unity Catalog, and CI/CD topics.

**Key sections:** Batch foundation, medallion model, streaming extension, governance, delivery, performance and cost, decision table.

**Content:** Start with the active Azure Lakehouse Starter Kit and link planned extensions as roadmap items.

### Microsoft Fabric

**Purpose:** Connect Fabric engineering, Real-Time Intelligence, semantic modeling, and data agent learning.

**Key sections:** OneLake and engineering, operational analytics, semantic layer, conversational analytics, lifecycle, governance.

**Content:** Link active Fabric blueprints and label planned semantic and data agent topics.

### Azure OpenAI And RAG

**Purpose:** Explain the planned enterprise RAG blueprint and its quality and governance model.

**Key sections:** Scenario, ingestion, retrieval, grounding, identity, evaluation, feedback, monitoring, responsible use, roadmap.

**Content:** Keep this page at planning level until working code exists. Link current official Azure AI Search and Azure OpenAI documentation.

### Power BI Semantic Modeling

**Purpose:** Provide cross-topic guidance for facts, dimensions, measures, security, Direct Lake, certification, and deployment.

**Key sections:** Model contract, storage mode decision, DAX, RLS, testing, lifecycle, AI-readiness.

**Content:** Reuse examples from active Gold models and link the planned dedicated blueprint.

### Governance And Purview

**Purpose:** Explain data ownership, catalog, classification, glossary, lineage, access review, and evidence.

**Key sections:** Operating model, roles, data product onboarding, metadata, access workflow, audit evidence, implementation roadmap.

**Content:** Separate catalog metadata from access enforcement. Use fictional governance records.

### Unity Catalog

**Purpose:** Explain the planned Azure Databricks governance implementation.

**Key sections:** Object model, storage credentials, external locations, managed and external assets, grants, workspace binding, row filters, column masks, audit and lineage.

**Content:** Link the active Azure Lakehouse setup and current official Azure Databricks documentation.

### CI/CD

**Purpose:** Define repository-wide delivery patterns for ADF, Databricks, Fabric, SQL, and Power BI assets.

**Key sections:** Version control boundary, validation, packaging, environments, approvals, promotion, smoke tests, rollback, release evidence.

**Content:** Link working CI examples from active topics and the planned dedicated blueprint.

### Real-Time Intelligence

**Purpose:** Guide learners through operational events, KQL, dashboards, alerts, and historical extension.

**Key sections:** Event contracts, Eventstream, Eventhouse, KQL, dashboard, Activator, Lakehouse history, lifecycle, troubleshooting.

**Content:** Link directly to the active Smart Logistics blueprint.

### Customer 360

**Purpose:** Explain the planned reusable data product linking BI, segmentation, ML, and AI context.

**Key sections:** Identity resolution, survivorship, consent, quality, dimensional model, features, semantic layer, context projection.

**Content:** Compare the current retail and retail banking examples, then define the planned cross-platform implementation.

### Troubleshooting

**Purpose:** Give visitors one triage entry point before topic-specific troubleshooting.

**Key sections:** Setup, identity, storage, schema, pipelines, Spark, SQL, KQL, Power BI, AI retrieval, CI/CD, issue reporting.

**Content:** Use symptom, likely cause, evidence to collect, and next action. Link to exact topic troubleshooting pages.

### Roadmap

**Purpose:** Show sequencing, release criteria, and ways to contribute without implying unfinished work is active.

**Key sections:** Current active releases, next 90 days, planned portfolio, release gates, contribution opportunities, decision log.

**Content:** Update at each release. Archive completed quarterly roadmap entries into changelog or releases.

## Navigation Structure

```text
Start Here
  Home
  How To Use This Repo
  Learning Paths
  Architecture Gallery

Platforms And Patterns
  Azure Lakehouse
  Microsoft Fabric
  Real-Time Intelligence
  Power BI Semantic Modeling
  Azure OpenAI And RAG
  Customer 360

Enterprise Readiness
  Governance And Purview
  Unity Catalog
  CI/CD
  Troubleshooting

Community
  Contributor Guide
  Roadmap
  FAQ
  Glossary
```

## Wiki Maintenance Rules

- Add a page only when it improves cross-topic navigation or explanation.
- Link detailed implementation guidance instead of copying it.
- Include active or planned status on feature-specific pages.
- Review product links and preview labels quarterly.
- Add previous, home, and next navigation to long pages.
- Keep the sidebar below 35 primary links by grouping related pages.
