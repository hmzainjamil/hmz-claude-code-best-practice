# Claude Code hook examples

This directory contains this repository's command-hook configuration, Python sound handler, and sound assets. It is a project-specific example, not the complete Claude Code hook reference.

## Files

- [Project settings](../settings.json) registers command hooks.
- [Handler](scripts/hooks.py) maps hook events to local sound folders.
- [Local toggles](config/hooks-config.json) contains per-event disable switches and a logging setting.
- [Sound assets](sounds/) provide the files used by the handler.

Hooks can execute local commands automatically. Review the project settings and handler before enabling these examples, especially in a repository you do not trust. The committed settings may grant broad tool permissions; review those separately.

For current event names, fields, configuration, and supported hook types, see the [official Claude Code hooks reference](https://code.claude.com/docs/en/hooks). The earlier fixed hook count and event table in this file were version-sensitive and are removed. No compatibility or runtime test is claimed for the local example.
