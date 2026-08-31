---
name: implementation-planning
description: Converts an approved solution into a practical sequence of small, testable implementation steps with dependencies, acceptance criteria, rollback points, and ownership.
---

# Implementation Planning

## Invoke when
Use after the desired solution is understood but before or during execution: websites, automations, integrations, migrations, campaign tracking, deployment changes, or operational workflows.

## Plan structure
1. Define the target state and explicit acceptance criteria.
2. Inventory current-state dependencies and constraints.
3. Separate prerequisites from implementation.
4. Sequence the smallest independently testable changes.
5. Identify risky or irreversible steps and define rollback/backup behavior.
6. Put verification immediately after each meaningful change.
7. Defer optional polish until the core path works.

## Tool behavior
Inspect the connected repository, existing configuration, workflow, documentation, or deployment state when available before writing steps. Use exact file paths, branch names, settings, or connector actions when they are known; do not invent them.

## Collaboration
Use solution-exploration before planning when the approach is still undecided; systematic-debugging when the task is actually diagnosis; completion-verification after execution.

## Return contract
Provide an ordered plan with dependencies, expected result per step, verification, and rollback where relevant. Highlight the first safe executable step and any information that truly blocks progress.
