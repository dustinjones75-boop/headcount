# Completion Verification

## Purpose
Verify that requested work is actually complete and works in the user's real path, not merely that code was changed or a task reported success.

## Invoke when
Use after bug fixes, deployments, automations, website changes, tracking changes, integrations, migrations, or other implementation work where “done” requires evidence.

## Verification ladder
1. Confirm the requested acceptance criteria.
2. Check the changed artifact or configuration exists where expected.
3. Verify build/tests/status checks when available.
4. Test the exact user path that previously failed.
5. Check adjacent regressions likely to be affected by the change.
6. Verify production or final destination, not only local/preview state, when the request concerns production.
7. Distinguish verified facts from items that could not be tested.

Never declare success based solely on a successful commit, automation run, build, or deployment if the user's end-to-end outcome has not been observed.

## Tool behavior
Use repository diffs, CI status, deployment output, connected automation run evidence, live pages, or other available artifacts. If a required check cannot be performed with available tools, state exactly what remains unverified.

## Output
Return: verified, partially verified, or not verified; evidence for that status; any remaining risks; and the next check if needed.
