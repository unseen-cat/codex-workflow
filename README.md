# Codex Workflow

This repository mirrors the layout of `WeZZard/skills` and packages the `codex-workflow` skill pack as a Codex marketplace repo.

The root is the marketplace. The actual plugin lives under `codex/codex-workflow/`, which keeps the repository structure close to the upstream project while staying Codex-native.

## Quick Start

From a shell with Codex CLI installed:

1. Register this repository as a marketplace from the repo root.

```text
codex plugin marketplace add ./
```

If you are installing from GitHub:

```text
codex plugin marketplace add unseen-cat/codex-workflow
```

2. Install the plugin from the configured marketplace snapshot.

```text
codex plugin add codex-workflow@codex-workflow
```

## Available Plugin

### codex-workflow

Development workflow skills for planning and execution.

| Skill | Description |
| --- | --- |
| `brainstorming` | Explore user intent, constraints, and options before implementation. |
| `write-plan` | Write explicit plans with verification and dependency order. |
| `execute-plan` | Implement a finalized plan without widening scope. |
| `audit-plan` | Compare the plan with the actual result and report mismatches. |
| `recover-from-errors` | Re-align with the plan when tools fail or progress stalls. |
| `be-thorough` | Investigate, verify, and test before concluding. |
| `same-page` | Re-explain a previous message with evidence, confidence, and a diagram. |

## Repo Layout

```text
.agents/plugins/marketplace.json
AGENTS.md
instruction.md
README.md
codex/codex-workflow/.codex-plugin/plugin.json
codex/codex-workflow/skills/brainstorming/SKILL.md
codex/codex-workflow/skills/write-plan/SKILL.md
codex/codex-workflow/skills/execute-plan/SKILL.md
codex/codex-workflow/skills/audit-plan/SKILL.md
codex/codex-workflow/skills/recover-from-errors/SKILL.md
codex/codex-workflow/skills/be-thorough/SKILL.md
codex/codex-workflow/skills/same-page/SKILL.md
```

## Source

This repository is derived from:

```text
WeZZard/skills
```

Only the `codex-workflow` plugin is packaged here. The source repository also contains other plugins, but they are intentionally out of scope for this Codex refactor.
