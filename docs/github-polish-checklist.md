# GitHub Polish Checklist

## Recommended Repository Topics

Use a focused set of discoverable topics:

```text
microsoft-fabric
azure-data-engineering
power-bi
azure-databricks
delta-lake
azure-openai
azure-ai-search
microsoft-purview
data-governance
lakehouse
pyspark
kql
data-quality
cicd
learning-resources
```

GitHub currently permits a limited number of repository topics, so review the list as the active portfolio changes.

## Badges

Root README badges should communicate project state, not decorate the page:

- License.
- Active blueprints count.
- CI validation status.
- Microsoft Fabric.
- Azure Data and AI.
- Community learning repository.

Topic README badges should be limited to primary services, language or artifact type, validation status, and license.

## Release Naming

Use quarterly or blueprint-specific releases:

- `2026 Q3 Learning Paths And Repository Standards`
- `Fabric Real-Time Intelligence Blueprint v1.0`
- `Azure Lakehouse Starter Kit v1.1`
- `Semantic Modeling Blueprint v1.0`

Each release should list completed assets, validation performed, known limitations, documentation links, and contributor acknowledgments based on actual commits.

## Issue Labels

| Label | Use |
| --- | --- |
| `area:fabric` | Fabric platform content |
| `area:azure-data` | Azure data platform content |
| `area:power-bi` | Power BI and semantic model content |
| `area:ai` | Azure AI and agent content |
| `area:governance` | Purview, Unity Catalog, security, ownership |
| `type:bug` | Broken or incorrect implementation |
| `type:docs` | Documentation change |
| `type:example` | New or improved sample |
| `type:diagram` | Architecture visual work |
| `type:test` | Validation and test work |
| `type:roadmap` | Portfolio planning |
| `level:beginner` | Suitable for new contributors |
| `level:advanced` | Requires deeper platform knowledge |
| `status:needs-triage` | Awaiting maintainer review |
| `status:blocked` | External prerequisite prevents progress |

## Good First Issue Ideas

- Validate links in one topic folder.
- Add expected output to one notebook or SQL script.
- Add one synthetic data quality defect and test.
- Improve alt text and labels for an architecture diagram.
- Add a troubleshooting entry based on a reproducible error.
- Add a glossary term with an official documentation reference.
- Convert one manual validation step into a script.
- Add a role-based exercise to a demo guide.

## Discussion Categories

- Announcements.
- Help With A Blueprint.
- Architecture Decisions.
- Ideas And Roadmap.
- Show What You Built.
- Articles, Talks, And Study Groups.
- Contributor Introductions.

## Screenshot Placeholders

Every active blueprint may include:

- Architecture overview.
- Successful pipeline or job run.
- Quality validation result.
- Governed query or access behavior.
- Final dashboard or application output.

Screenshots must not show tenant names, email addresses, tokens, resource IDs, customer data, or confidential browser tabs.

## Demo GIF Ideas

- Raw file to Gold table in under 30 seconds.
- Eventstream to KQL dashboard update.
- RLS role change and report result.
- Pull request quality gate to deployment approval.
- RAG question with retrieved citations and evaluation result.
- Unity Catalog denied access followed by approved group access.

Keep GIFs short, captioned, compressed, and supplementary to written steps.

## Architecture Image Naming

Use:

`<topic>-<view>-v<major>.png`

Examples:

- `fabric-banking-end-to-end-v1.png`
- `azure-lakehouse-medallion-v1.png`
- `azure-rag-runtime-flow-v1.png`

Keep the editable source beside the export.

## Branching Strategy

Use short-lived branches from `main`:

- `feature/<topic-or-capability>`
- `docs/<topic-or-page>`
- `fix/<issue-or-component>`
- `test/<validation-area>`
- `release/<version>` only when release preparation needs isolation

Branch names, commit messages, pull requests, review comments, and contributor records should describe the work and the people involved. Do not include tool or assistant identity as an author, contributor, branch prefix, or promotional label.

## Contribution Rules

- One coherent purpose per pull request.
- Link the issue or roadmap item.
- Explain learner and implementation value.
- Add or update tests for behavior changes.
- Update architecture and docs when interfaces change.
- Use synthetic data only.
- Remove secrets and environment-specific identifiers.
- Cite official documentation for current product behavior.
- Label preview dependencies and known limitations.
- Preserve unrelated contributor work.

## Folder Naming

- Use lowercase kebab case.
- End implementation collections with `-blueprint` or `-starter-kit` consistently.
- Use service names only when they define the implementation scope.
- Avoid version numbers in folder names.
- Avoid acronyms that are not widely understood.
- Do not create an empty planned folder.

## Final Repository Review

- [ ] Root README has a clear status legend.
- [ ] Every active catalog link resolves.
- [ ] Planned topics are not presented as working implementations.
- [ ] CI covers all executable active folders.
- [ ] Issue and PR templates request validation evidence.
- [ ] Wiki and root README use the same catalog names.
- [ ] Releases summarize real implementation changes.
- [ ] Contributor attribution matches Git history.
- [ ] Screenshots and samples are safe for public use.
