---
name: execute-plan
description: Use when a finalized plan is ready to implement.
---

# Executing Plans

Use this skill once the plan is final and you are ready to write code.

The main job is to stay aligned with the plan while moving as fast as the dependency graph allows.

## Rules

- Read the current plan first.
- Build the dependency order before editing.
- Run independent tasks in parallel when possible.
- Use a separate worker or subagent for multi-file work, command interpretation, or research.
- Keep single small edits inline.
- Stop immediately on blockers, missing prerequisites, or failing verification.
- If a task needs human judgment, pause and ask instead of guessing.
- Do not widen scope while implementing.
- Match the plan exactly and leave unrelated code alone.

## Execution flow

1. Load the plan.
2. Sort tasks by dependency.
3. Implement the lowest-level tasks first.
4. Verify each step before moving on.
5. Keep the plan updated if the execution reveals a real change in scope.

## What to avoid

- Do not guess around missing inputs.
- Do not silently skip verification.
- Do not merge unrelated fixes into the same pass.
- Do not continue after a blocker without resolving the blocker first.
