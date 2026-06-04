# AGENTS.md

This repository is a Codex marketplace repo that mirrors the structure of `WeZZard/skills`.

## Source Of Truth

- Marketplace file: `.agents/plugins/marketplace.json`
- Plugin manifest: `codex/codex-workflow/.codex-plugin/plugin.json`
- Skill behavior: `codex/codex-workflow/skills/*/SKILL.md`
- Standalone instructions: `instruction.md`
- Public overview: `README.md`

## Package Intent

The marketplace teaches Codex to:

- explore before implementing,
- write concrete plans,
- execute work in dependency order,
- audit the result against the plan,
- recover from tool failures by re-aligning,
- stay thorough,
- explain prior messages with evidence when asked.

## Maintenance Rules

- Keep the marketplace entry aligned with `codex/codex-workflow`.
- Keep the plugin Codex-native.
- Do not add metadata for other agent runtimes.
- Do not expand this package to the rest of the source marketplace unless the user asks.
- Keep the body text direct and concrete.

## Quality Bar

Before publishing a change, confirm:

- the marketplace file points at `codex/codex-workflow`,
- every skill file has valid frontmatter,
- the README matches the repo layout,
- `instruction.md` still matches the same workflow,
- the repo still reflects the source repo's `codex-workflow` workflow only.
