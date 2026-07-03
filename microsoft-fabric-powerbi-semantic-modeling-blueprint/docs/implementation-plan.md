# Implementation Plan

## Delivery Stages

1. Define fact grain, dimensions, keys, and metric ownership.
2. Build Gold consumption views and expected results.
3. Create semantic model metadata, relationships, and hierarchies.
4. Implement DAX measures and a dedicated date model.
5. Add RLS roles and identity test cases.
6. Compare Direct Lake, Import, and DirectQuery.
7. Add deployment, certification, monitoring, and support guidance.

## Key Assets

- SQL Gold views.
- TMDL or PBIP-friendly model metadata where practical.
- DAX measure library.
- Metric definitions and business glossary.
- RLS matrix.
- Result fixtures and validation scripts.
- Environment and release checklists.

## Acceptance Criteria

The blueprint becomes Active when measures reconcile to fixtures, RLS behaves as designed, deployment guidance is reproducible, and the demo uses a versioned model.
