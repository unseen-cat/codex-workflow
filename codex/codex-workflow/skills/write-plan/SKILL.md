---
name: write-plan
description: Use when creating or updating the current plan before implementation.
---

# Write / Update Plan

Use this skill to turn a request into a concrete plan before code changes begin.

The plan should answer four things: what will change, what is still uncertain, how success will be verified, and where human judgment is needed.

## What to capture

- Exact files to touch.
- The problem, hypothesis, or requested behavior.
- The verification method.
- Any human review that must happen before dependent work.
- The dependency order between tasks.

## Rules

- Start by saying you are using the write-plan skill.
- Keep the plan focused on the current task.
- Do not invent missing context; gather it or mark it as a hypothesis.
- For bug fixes, include a reproducer or regression check before the fix.
- For refactors, state what behavior must remain unchanged.
- For multi-file or boundary work, spell out the tests at the right level.
- Keep tasks one concrete change each, and order them by dependency.
- Update the live plan instead of rewriting history.
- If a piece cannot be known yet, label it clearly and add a verification task before dependent work.

## Good plan shape

- Goal
- Why this change is needed
- Tasks in dependency order
- Verification
- Risks and open questions

## What not to do

- Do not write vague tasks like "clean things up."
- Do not hide uncertainty.
- Do not skip verification because the change feels small.
- Do not bundle unrelated changes into one task.
