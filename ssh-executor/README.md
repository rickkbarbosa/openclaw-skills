# ssh-executor

This release continues the packaging cleanup of **ssh-executor** and explicitly declares all runtime requirements used by the bundled helper.

## What changed in 1.0.3

- declares `python3` in skill metadata alongside `ssh` and `bash`
- keeps bundled script references aligned with `scripts/ssh-run.sh`
- keeps the release bundle coherent with `SKILL.md`, `scripts/`, and `references/`

## Recommended upload artifact

For publication, upload the packaged skill artifact:

- `ssh-executor.skill`

The outer `.zip` is for storage, review, and backup. The `.skill` is the actual distributable bundle.

## Included files

- `ssh-executor.skill`
- `ssh-executor.skill.sha256`
- `SKILL.md`
- `scripts/ssh-run.sh`
- `references/safety.md`
- `release.json`
- `README.md`

## Public metadata

- **Slug:** `ssh-executor`
- **Display name:** `ssh-executor`
- **Version:** `1.0.3`
- **Tags:** `ssh, remote-exec, ops, automation, linux`

Short description:

> Run key-based SSH commands with alias support, structured output, tmux-friendly workflows, and confirmation guardrails for dangerous operations.

Changelog:

> Metadata declaration release. Adds explicit `python3` runtime requirement, keeps bundled script references aligned, and preserves a coherent public release bundle.
