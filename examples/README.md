# Shareable examples

Drop-in snippets you can copy without installing the whole Starter.

| File | What it is |
|------|------------|
| [`anti-scope-creep-always-apply.mdc`](./anti-scope-creep-always-apply.mdc) | Tiny `alwaysApply` core + the three-part filter for what earns that slot |
| [`re-read-after-compaction-always-apply.mdc`](./re-read-after-compaction-always-apply.mdc) | Post-compaction recovery: re-read AGENTS.md, do not invent a second stack |
| [`no-second-stack-always-apply.mdc`](./no-second-stack-always-apply.mdc) | Do not invent a parallel framework/dependency mid-task |
| [`verify-dont-invent-always-apply.mdc`](./verify-dont-invent-always-apply.mdc) | Never invent APIs/URLs/env keys; ask before destructive deletes |

## Install one rule

1. Copy the `.mdc` into your repo at `.cursor/rules/`
2. Keep it short — if it grows past a screen, demote stack-specific bits to `globs`

Full free Starter (core always-on rules + 1 PR Skill): repo root / [landing](https://kangtai-cn.github.io/agent-memory-pack/?ref=examples-readme)
