# Code Review

## Purpose
Review code changes for correctness, regressions, maintainability, security-sensitive mistakes, and mismatch with the stated goal.

## Invoke when
Use for pull requests, diffs, commits, refactors, bug fixes, or implementation reviews.

## Method
1. Read the stated objective and acceptance criteria.
2. Inspect the actual diff and the surrounding code it depends on.
3. Identify correctness bugs first, then regressions, edge cases, tests, maintainability, and style.
4. Distinguish blocking findings from optional improvements.
5. Verify claims against repository evidence rather than guessing from filenames.

## Tool behavior
When GitHub is connected, inspect the PR or commit, changed files, relevant implementation files, and CI/test evidence before reviewing.

## Output
Return findings ordered by severity, with file/behavior evidence, the consequence, and the smallest safe fix. If no material issue is found, say so plainly and note any residual test gap.