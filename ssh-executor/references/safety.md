# SSH Executor Safety Notes

## Default posture

- Prefer SSH aliases and existing `~/.ssh/config` entries.
- Prefer private keys over passwords.
- Prefer read-only inspection before any mutation.
- Keep timeouts short unless the user clearly expects a long-running command.
- Let ssh config resolve host, user, port, and identity file when an alias already exists.

## Host-key policy

- Existing ssh config policy wins if you do not pass `--host-key-checking`.
- `yes`: best for known sensitive hosts with preloaded host keys.
- `accept-new`: acceptable for first contact on low-risk hosts when the user asked to connect.
- `no`: avoid unless the user explicitly understands the risk.

## Commands that need confirmation

Ask before running commands that:
- modify files or permissions
- restart or stop services
- install, remove, or upgrade packages
- reboot or shut down the host
- use `sudo`
- delete data or rotate logs
- change container, database, firewall, or network state

The script returns a guardrail error for dangerous commands unless `--confirm-dangerous` is present.

## Reporting pattern

After execution, report:
1. target host
2. whether connection succeeded
3. exit code
4. resolved SSH metadata when useful
5. short summary of stdout/stderr
6. next safe step
