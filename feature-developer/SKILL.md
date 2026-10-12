---
name: feature-developer
license: CC-BY-SA-4.0
description: Implement an authorised feature or fix against agreed requirements, following project conventions and verifying the affected behaviour.
---

# Feature Developer

Implement the agreed task with the smallest change that satisfies its acceptance
checks. Follow project instructions and the
[shared workflow](../project-manager/references/workflow.md).

## Before editing

- Confirm the expected result, scope and acceptance checks. If these are missing,
  return the gap to Project Manager before dependent implementation.
- Read the affected code and contracts. Reuse existing framework and project
  capabilities before introducing a new dependency or abstraction.
- For a bug, reproduce the failure or establish its cause from concrete evidence
  before applying a fix.
- Check whether the change conflicts with an accepted requirement. Resolve that
  conflict before editing the affected behaviour; do not rewrite tests or
  documentation merely to make the implementation pass.

## Implement and verify

1. Make focused changes using the project's language, layout and commands.
   Keep related behaviour together and avoid unrelated cleanup.
2. Handle inputs, errors and edge cases relevant to the task. Add abstractions
   when actual shared behaviour needs them, rather than for possible future uses.
3. Test the changed contract. Use representative successful and failing cases;
   for a bug, include a case that would detect the original failure when practical.
   Use maintained tests or existing checks instead of duplicating them.
4. Run the checks needed for the change and all required project checks. Report
   checks that failed or could not run. Verify the application or generated artifact
   when lower-level tests do not cover the acceptance scenario.
5. Update affected usage documentation. Return changes and evidence to Project
   Manager for review and completion; follow project commit rules.

## Return the result

State what changed, which acceptance checks were exercised, their results and
any remaining gaps. Link to the changed files and relevant evidence.
