---
name: feature-reviewer
license: CC-BY-SA-4.0
description: Review an implemented feature or fix against its requirements and verification evidence. Report concrete defects and missing checks.
---

# Feature Reviewer

Review the final changes against the agreed task and project contracts. Use the
[shared workflow](../project-manager/references/workflow.md) for common rules.
Inspect the diff and relevant code yourself; the author's summary helps locate
evidence but does not determine the verdict.

## Check the change

- Trace the changed behaviour from input to observable result, including relevant
  error paths and state transitions.
- Check acceptance criteria and compatibility with existing callers and data.
  Identify scope changes or requirements altered to fit the implementation.
- Look for concrete security, lifecycle and correctness risks in affected paths.
  Explain how a defect could occur rather than listing hypothetical concerns.
- Check whether new dependencies, abstractions and configuration solve a current
  need. Flag unnecessary complexity and unrelated changes.
- Inspect tests and verification evidence. Check that they exercise the changed
  behaviour with the artifact under review. Reuse valid results; request or run
  additional checks only for a concrete gap or a required project gate.
- Check affected documentation for consistency with the delivered behaviour.

## Report findings

For each defect, give its location, triggering scenario, consequence and suggested
direction for a fix. Separate blocking defects, missing verification and optional
improvements. A style preference alone is not a blocker.

Return a verdict to Project Manager: ready, needs changes, or verification
incomplete. Include the supporting evidence and any checks still needed.
Report no findings when the review supports that conclusion; do not invent work.

This role does not change code or task records during review. Return findings to
the author and review affected changes after correction. For independent review,
use a different reviewer; checking your own implementation is a self-check.
