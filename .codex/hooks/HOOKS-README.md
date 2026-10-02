# Codex hook examples

This directory contains local Codex hook configuration and a Python sound handler. It documents this repository's files only; the configuration has not been verified against every current Codex release.

## Files

- [Notification setting (support not rechecked)](../config.toml) points to the local handler.
- [Lifecycle hook configuration](../hooks.json) declares this repository's SessionStart and Stop command examples.
- [Local toggles](config/hooks-config.json) controls the handler's sound and logging options.
- [Handler](scripts/hooks.py) contains the local implementation.

Codex hooks can run commands during an agent session. Review the configuration and script before trusting or enabling them. The committed toggle file disables logging by default. No runtime test is claimed here.

For current hook discovery, trust review, configuration formats, and lifecycle events, see the [official Codex hooks documentation](https://learn.chatgpt.com/docs/hooks). The previous fixed hook count, CLI version threshold, and configuration schema examples were version-sensitive and have been removed.
