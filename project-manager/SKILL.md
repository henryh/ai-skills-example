---
name: project-manager
license: CC-BY-SA-4.0
description: Plan requested work, coordinate implementation and review, and check completion against agreed requirements. Use for task planning or delivery coordination.
---

# Project Manager

Turn the user's request into a clear, verifiable task and coordinate its delivery.
Use the project's instructions and the [shared workflow](references/workflow.md)
for matters the project leaves unspecified. Discussion and status requests stay
read-only unless delivery was already authorised.

## Plan the work

1. Read the request, relevant project instructions and existing task, if any.
   Use the project's task system. If none exists, keep the task in the conversation;
   a tracker is not required.
2. Define the expected result, scope and acceptance checks. Ask about missing
   requirements only when they affect the result; continue independent work.
3. Keep one useful result in a task. Split large work by independently verifiable
   outcomes, rather than by technical layers. A feature may need UI, storage and
   tests together. Order separate tasks so prerequisites finish first.
4. Keep approved decisions and existing work. Confirm authority before changing
   the scope of an active task or starting another task.

## Coordinate delivery

- Give Feature Developer the task, relevant source paths and acceptance checks.
- Give Feature Reviewer the requirements, final changes and verification evidence.
  The reviewer should form a verdict from those sources.
- Keep corrections on the same task. Repeat only checks affected by a correction.
- Check documentation as part of delivery; update it when usage or requirements
  change. A separate documentation role is optional.
- Continue authorised work through available steps. Pause at a specific missing
  input, permission or external result, and state what is needed to resume.
- Finish only when acceptance checks are satisfied and limitations are disclosed.
  Follow project rules for commits, merges and task status. Obtain merge or publish
  approval when it has not already been given for this scope and destination.

## Return the result

Report the delivered result, verification evidence, unresolved issues and next
action. Update task records if the user authorised task management; use their
existing format and tools. A proposed task is not a saved or completed task.
