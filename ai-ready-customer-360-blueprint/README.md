# AI-Ready Customer 360 Blueprint

> Build a consent-aware customer data product for trusted BI, segmentation, feature engineering, and approved AI context.

## Status

**Planned scaffold**

This folder defines a cross-platform implementation contract. The first active track will select either Microsoft Fabric or the Azure Lakehouse foundation and document the decision.

## Business Scenario

A fictional Adventure Works omnichannel retailer needs a consistent customer view across commerce, service, loyalty, marketing consent, campaigns, and digital behavior.

## Microsoft Services

- Microsoft Fabric or Azure Lakehouse implementation track
- Power BI
- Azure Databricks or Azure Machine Learning feature capabilities where appropriate
- Azure AI Search for approved context projection
- Microsoft Purview integration points
- Microsoft Entra ID

## What Learners Will Build

1. Source identity standardization.
2. Deterministic and reviewable matching rules.
3. Survivorship and source evidence.
4. Consent-aware golden customer profile.
5. Interaction facts, quality score, and segments.
6. Semantic model and feature table.
7. Purpose-specific AI context projection.

## Planned Structure

- README and data product documentation.
- Architecture source and exported diagram.
- PySpark, SQL, DAX, and data quality assets.
- Synthetic profile and interaction samples.
- Matching, consent, and reconciliation tests.
- Demo script and extension exercises.

## Release Gate

- [ ] Synthetic multi-source customer data is included.
- [ ] Matching and survivorship rules retain source evidence.
- [ ] Consent and purpose restrictions are tested.
- [ ] Gold, semantic, feature, and AI context contracts are separate.
- [ ] PII, quality, security, and deletion considerations are documented.
- [ ] Demo shows identity resolution, consent, analytics, and approved context.

## Start Contributing

Read the [implementation plan](docs/implementation-plan.md), [diagram brief](diagrams/README.md), [sample plan](samples/README.md), [test plan](tests/README.md), and [demo outline](demo/README.md).

## Disclaimer

This is a community learning scaffold and not official Microsoft documentation. It uses fictional identities and must not be treated as legal advice for privacy, consent, or data retention.
