# Thread GC

A Codex skill for assessing the health and continuity of fixed-role project tasks and recommending safe handoffs when needed.

## What it does

- Reviews currently used, non-archived tasks within the selected project.
- Uses recent work and concrete continuity issues as evidence; task age or context length alone does not justify replacement.
- Recommends whether to keep, monitor, replace at a safe boundary, or retire a role.
- Provides procedures for authorized replacement, archival, and recovery while preserving user work.

Assessments are read-only. Renaming, creating, messaging, routing changes, and archival require authorization covering those actions. Reading this skill does not start an audit.

## Install

Clone this repository into your Codex skills directory:

```sh
git clone https://github.com/Allwayz/thread-gc.git ~/.codex/skills/thread-gc
```

If your Codex installation uses a custom `CODEX_HOME`, place the repository at `$CODEX_HOME/skills/thread-gc` instead.

## Use

Ask Codex to use `$thread-gc` to assess the fixed-role tasks for a project and recommend any needed handoffs. See [SKILL.md](SKILL.md) for scope, evidence, and lifecycle rules.

## Files

- `SKILL.md` — full skill instructions.
- `agents/openai.yaml` — display metadata and default prompt.
