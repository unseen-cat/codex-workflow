---
name: audit-plan
description: Use after implementation to compare the final result against the plan and report mismatches.
---

# Audit Plan Execution

Use this skill after the implementation pass finishes.

The audit should answer one question: did every planned task happen, and is there evidence for it?

## What to verify

- File existence for items that should have been created.
- File content for items that should have been changed.
- Deletions for items that should have been removed.
- Command output for any verification step that was part of the plan.

## Reporting rules

- Report each task as `Done`, `Partial`, or `Missing`.
- Attach concrete evidence to every verdict.
- Separate confirmed issues from open questions.
- Do not fix the code while auditing; only report what you found.

## Audit shape

| Task | Status | Evidence |
| --- | --- | --- |
| task name | Done / Partial / Missing | file path, line, or command output |

## What to avoid

- Do not rely on memory.
- Do not mark a task done without checking the actual file system or command result.
- Do not hide partial completion.
- Do not turn the audit into a new implementation pass.
