---
name: systematic-debugging
description: Diagnoses technical failures by reproducing, narrowing, inspecting evidence, and changing the smallest plausible cause before proposing broad rewrites.
---

# Systematic Debugging

## Invoke when
Use for broken websites, deployment failures, automation errors, integration issues, UI bugs, code regressions, or any case where the user reports that something does not work as expected.

## Method
1. Restate the expected behavior and observed failure.
2. Reproduce or inspect the closest available evidence.
3. Identify the boundary where expected and actual behavior diverge.
4. Form a small set of ranked hypotheses.
5. Inspect logs, source, configuration, network behavior, environment differences, or recent changes relevant to those hypotheses.
6. Change the smallest plausible cause first.
7. Verify the fix against the original failure and check for regressions.

## Rules
- Do not rewrite a working subsystem because one symptom is unexplained.
- Do not stack speculative fixes.
- Separate root cause from workaround.
- Treat intermittent, device-specific, and environment-specific behavior as evidence, not noise.
- When a recent change exists, compare before/after rather than reasoning from memory.

## Tool behavior
Inspect connected repositories, relevant files, commits, PRs, CI runs, deployment evidence, screenshots, and supplied logs when available. Use live web inspection when the issue depends on a deployed public page. Do not ask the user to paste code that can be retrieved from a connected repository.

## Collaboration
Use implementation-planning after the root cause is identified, release-and-deployment for deployment-specific faults, and completion-verification before declaring success.

## Return contract
State the most likely root cause, evidence, confidence, the minimal fix, and how to verify it. If unresolved, specify the single next diagnostic that would most reduce uncertainty.
