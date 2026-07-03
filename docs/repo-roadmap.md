# 90-Day Repository Roadmap

## Roadmap Goal

Over 90 days, turn the current three-blueprint collection into a consistent Microsoft Data and AI implementation playbook, then release the first two expansion topics with working assets.

The roadmap favors depth and release quality over opening all planned folders at once.

## Delivery Principles

- Active means implemented, documented, validated, and demonstrable.
- Planned topics stay in strategy documents until their release gate is met.
- Reuse fictional business domains and shared contracts where that improves comparison.
- Verify current product prerequisites and preview status at implementation time.
- Make every release usable in both read-only study mode and hands-on deployment mode where practical.
- Add validation before adding promotional assets.

## Days 1 To 30: Repository Foundation

### Week 1: Positioning And Navigation

- Replace the root README with the implementation-playbook positioning.
- Publish active and planned status definitions.
- Add the role-based learning paths.
- Add the service coverage map.
- Update the public Wiki Home and sidebar.
- Add the repository expansion plan to the Wiki.

**Exit evidence:** A new visitor can identify what is active, choose a path, and understand the repository standard within five minutes.

### Week 2: Blueprint Standards

- Adopt the topic README template.
- Define architecture naming and source-file standards.
- Add production readiness, demo, and validation checklists.
- Update contribution guidance with blueprint release gates.
- Review active topic READMEs against the new template.

**Exit evidence:** A maintainer can review a proposed topic using one documented checklist.

### Week 3: Validation And GitHub Operations

- Inventory executable assets in all active blueprints.
- Add or refine root CI jobs for documentation links, JSON parsing, Python syntax, sample data, and topic-specific tests.
- Standardize issue labels and good first issue descriptions.
- Review issue and pull request templates.
- Define release notes structure.

**Exit evidence:** Pull requests receive deterministic checks and contributors know what evidence to provide.

### Week 4: Active Blueprint Quality Pass

- Audit setup commands and expected outputs.
- Review official documentation links and preview labels.
- Add missing cleanup and cost-safety steps.
- Check diagrams for readable labels and source exports.
- Record known limitations and next implementation issues.

**Exit evidence:** The three active blueprints meet the same baseline and have scoped improvement issues.

## Days 31 To 60: First Expansion Release

### Primary Release: Power BI Semantic Modeling Blueprint

This topic should be first because it completes the path from engineered Gold data to trusted business metrics and can reuse current Fabric sample domains.

### Week 5: Scenario And Model Contract

- Define the fictional Commercial Performance scenario.
- Specify fact grain, dimensions, relationships, and metric definitions.
- Create synthetic sales, return, target, and inventory samples.
- Write architecture decision records for storage mode, model shape, and security.

### Week 6: Implementation

- Build SQL consumption views.
- Add TMDL or PBIP-friendly semantic model assets where practical.
- Implement DAX measures, hierarchies, and a date model.
- Add RLS roles and test identities.

### Week 7: Validation And Lifecycle

- Add measure fixtures and result checks.
- Add RLS test matrix.
- Document Direct Lake, Import, and DirectQuery decisions.
- Add Git and deployment pipeline guidance.
- Add performance and cost notes.

### Week 8: Demo And Release

- Produce Excalidraw source and PNG architecture.
- Write demo script and exercises.
- Publish Wiki page and architecture gallery entry.
- Create release notes and one article draft.
- Open good first issues for extensions.

**Day 60 exit evidence:** The semantic modeling folder is Active and includes implementation assets, tests, documentation, diagrams, and a repeatable demo.

## Days 61 To 90: Governance Foundation And Second Expansion

### Primary Release: Azure Databricks Unity Catalog Blueprint

This topic should follow because it extends the active Azure Lakehouse starter kit and provides concrete governance controls before more advanced AI and streaming expansion.

### Week 9: Governance Model

- Define the fictional Manufacturing Data Products scenario.
- Specify Entra groups, workspaces, catalogs, schemas, and data domains.
- Decide managed versus external asset examples.
- Define allowed and denied access tests.

### Week 10: Implementation Assets

- Add catalog, schema, storage credential, and external location templates.
- Add group grant scripts.
- Add row filter and column mask examples.
- Add workspace binding and environment isolation guidance.
- Add audit and lineage queries.

### Week 11: Validation And Operations

- Add permission test matrix.
- Add safe setup and cleanup instructions.
- Document ownership, break-glass access, and quarterly review.
- Add cost, monitoring, and troubleshooting guidance.
- Verify runtime and compute prerequisites against current official documentation.

### Week 12: Demo, Community Review, And Next Quarter

- Produce architecture source and PNG.
- Run an end-to-end allowed and denied access demo.
- Publish Wiki page and release notes.
- Draft the Unity Catalog article and short demo video.
- Hold a roadmap discussion for the next blueprint.
- Review repository impact using verifiable signals.

**Day 90 exit evidence:** The Unity Catalog folder is Active, the portfolio has five completed blueprints, and the next quarter is prioritized using learner and contributor feedback.

## Backlog After Day 90

Recommended order:

1. `azure-data-engineering-cicd-blueprint`
2. `azure-streaming-cdc-blueprint`
3. `ai-ready-customer-360-blueprint`
4. `azure-data-governance-purview-blueprint`
5. `azure-openai-rag-enterprise-blueprint`
6. `fabric-data-agent-copilot-analytics-blueprint`

This order builds delivery, streaming, data product, and governance foundations before the AI-focused releases.

## Success Measures

| Area | 90-Day Measure |
| --- | --- |
| Navigation | All active and planned topics have accurate status and working links |
| Quality | Active executable folders run their validation checks in CI |
| Consistency | Active READMEs follow the shared blueprint contract or have tracked gaps |
| Releases | Two new blueprints meet the full release gate |
| Community | At least ten scoped contribution issues exist across docs, tests, diagrams, and examples |
| Learning | Each active blueprint has a demo script and at least one extension exercise |
| Evidence | Releases, feedback, fixes, articles, and sessions link to stable repository versions |

## Risks And Controls

| Risk | Control |
| --- | --- |
| Too many unfinished topics | Do not create planned folders before release work begins |
| Product changes invalidate guidance | Review official links and preview status before each release |
| Cloud costs block learners | Provide read-only paths, safe defaults, cleanup steps, and cost drivers |
| Examples drift across platforms | Use shared domain contracts only when they clarify comparison |
| Documentation outpaces code | Require working assets and validation before Active status |
| Community work becomes hard to review | Use scoped issues, templates, release gates, and focused pull requests |
