# Architecture Review

`architecture-review` is a read-only Agent Skill that independently reviews a concrete implementation plan, system design, or technical approach before implementation. It evaluates requirement fit, architectural boundaries, data model, workflows, transactions, concurrency, failure handling, permissions, compatibility, scalability, maintainability, and governance compliance.

It does not implement, change source code, modify architecture files, create migrations, or turn early ideation into an architecture review.

## Workflow boundary

```text
Idea / unclear problem → multiple-pov
Defined requirements → full-plan
Concrete plan / architecture → architecture-review
Implementation → practical-test / root-cause when needed
Completion → final-check
```

## Install from this repository

Give your coding agent this repository URL and ask it to install the global `architecture-review` skill from `skills/architecture-review`.

For Codex, use:

```text
$skill-installer https://github.com/MahanManouchehri/architecture-review/tree/main/skills/architecture-review
```

Or paste this prompt into ChatGPT, Codex, or Claude Code:

```text
Install the global Agent Skill at https://github.com/MahanManouchehri/architecture-review/tree/main/skills/architecture-review as `architecture-review`. Preserve the included SKILL.md and make it available across my projects using your platform's supported user-level skill location.
```

## Contents

- `skills/architecture-review/` — the portable Agent Skill.
- `plugin.json` — portable plugin metadata.
- `.codex-plugin/plugin.json` — Codex compatibility metadata.

## License

MIT. See [LICENSE](LICENSE).
