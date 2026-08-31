# Solution Architecture

## Purpose
Choose a technical structure that solves the real problem with the fewest unnecessary dependencies and a clear path to operation, maintenance, and change.

## Invoke when
Use before building integrations, websites, automation platforms, data flows, agent systems, deployment stacks, or when comparing architecture options.

## Method
1. Define the user/business outcome and hard constraints.
2. Inventory existing systems, skills, contracts, data, and connectors.
3. Separate must-haves from future possibilities.
4. Compare viable options on complexity, cost, reliability, portability, security/privacy, maintainability, and failure modes.
5. Prefer the smallest architecture that meets current requirements while leaving reversible extension points.
6. Identify system boundaries, sources of truth, interfaces, ownership, and recovery paths.
7. Explicitly state vendor lock-in and recurring-cost implications.

## Tool behavior
Inspect connected repositories, deployment configuration, available connectors/actions, and existing architecture before proposing replacement systems. Use current vendor documentation for capabilities or limits that may change.

## Collaboration
Use solution-exploration when alternatives are not yet narrowed, implementation-planning after architecture selection, ai-workflow-architect for automation-heavy systems, and release-and-deployment for production rollout.

## Output
Return the recommended architecture, alternatives considered, key tradeoffs, component/data-flow description, risks, and the first implementation milestone.
