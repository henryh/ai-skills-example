# Shared workflow

Use these defaults where project instructions leave a matter unspecified.
Explicit project rules replace the corresponding defaults. Honour the user's
scope, decisions and existing authorisation.

## Scope and working state

- A discussion, diagnosis or status request authorises inspection and a response.
  It does not by itself authorise file changes or task creation. A follow-up
  question during authorised delivery does not cancel that delivery.
- Use the project's existing tools, commands and layout. A task can be a tracker
  entry or an agreed description in the conversation. Do not install a tracker
  or create another task store as a prerequisite for a small change.
- Before editing, inspect the relevant working state and preserve user changes.
  For Git delivery, use a task branch unless the project or user specifies another
  route. Commit only changes belonging to the task, following project rules.
- Keep the current task until completion or an explicit change of focus. A blocker
  does not grant permission to start another task or silently reduce acceptance.
- Make routine implementation choices within the known requirements. Ask when an
  unresolved choice changes the expected product behaviour, accepted contract,
  scope or authority. Stop only the dependent work while it is unresolved.

## Delivery

1. **Project Manager:** agree the result, scope and acceptance checks. Identify
   the relevant code and existing project workflow.
2. **Feature Developer:** implement the task, verify changed behaviour and update
   affected documentation. Return the changes and verification evidence.
3. **Feature Reviewer:** inspect requirements and final changes, report defects
   and identify missing verification. Return corrections to the developer on the
   same task, then review the affected result.
4. **Project Manager:** confirm acceptance, report limitations and complete the
   authorised delivery actions. Update the existing task record when applicable.

Roles describe responsibilities; they need not be separate agents. A single
agent can perform these steps, but its review is a self-check. Use another person
or agent when independent review is required by the project. Delegate only when
authorised; if required independent review is unavailable, report that gap.

Keep planning proportional to the change. A small task needs a clear result and
checks; a technical design or additional specialist is needed only when the
project requires it or material uncertainty justifies it.

## Verification

- Check the boundary where the requirement is observed. A passing unit test does
  not establish a browser interaction or deployment that was never exercised.
- Choose checks for the changed contract and concrete risks, plus required project
  gates. Tests should detect incorrect behaviour, not mirror implementation details.
- For a bug fix, check the original failure and relevant neighbouring behaviour.
  A reversible text correction normally needs a focused consistency check.
- Reuse successful evidence while relevant code, configuration, inputs and runtime
  remain unchanged. Repeat affected checks after a relevant change, failure or
  contradictory observation. A handoff or commit alone does not require rerunning.
- Report success only after a command completes successfully. State failed,
  skipped or unavailable checks; unverified acceptance is not a pass.
- Keep commands focused and output concise. On failure, show the relevant
  diagnostics. Remove temporary resources created for verification, preserving
  maintained tests and pre-existing data.

## Completion and handoff

Continue available authorised steps after each handoff. Stop when the task is
complete, the user asks to pause, or progress requires specific missing input,
authority or an external result. Explain the exact boundary at a stop.

A request to implement or finish does not automatically authorise merging,
publishing or sending messages. Use approval already given for the same scope
and destination; do not ask for it again. A failed required check blocks delivery
until resolved or explicitly waived where the project permits a waiver.

Keep a short handoff in the existing task or conversation: goal, accepted
decisions, changed paths, valid evidence, gaps and next action. Reuse instructions
already available. Read only relevant files or sections, bound large outputs and
narrow truncated searches. Load another role when its work begins.
