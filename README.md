# Claude Code Best Practices

A reference repository for Claude Code configuration concepts, implementation examples, and workflows. It includes best-practice notes, sample project configuration, tutorial material, and demonstrations such as a command-to-agent-to-skill weather flow. It is documentation and example configuration, not a packaged runtime.

## Repository map

| Area | Contents |
|---|---|
| [Best-practice guides](best-practice/) | Settings, skills, commands, subagents, memory, MCP, and CLI flags |
| [Implementation examples](implementation/) | Example configurations for skills, commands, subagents, scheduled tasks, and agent teams |
| [Orchestration workflow](orchestration-workflow/orchestration-workflow.md) | Command → agent → skill example |
| [Development workflows](development-workflows/) | Research and implementation workflow examples |
| [Agent teams](agent-teams/) | Agent-team example assets |
| [Tutorial](tutorial/day0/README.md) | Getting started by operating system |
| [Reports](reports/) | Research and reference notes; check their dates and sources |
| [Tips](tips/) and [videos](videos/) | Dated notes and linked material |

See the [documentation index](docs/README.md) for a fuller map.

## Example configuration

The repository includes project-level Claude configuration, including `.claude/settings.json` and `.mcp.json`. These files are examples and may allow broad file edits, shell commands, and MCP tools. Review every permission, hook, and server command before use. Do not copy the settings wholesale into another project.

The weather workflow and other implementation pages describe examples. Their presence does not prove they were run successfully in your environment. Verify current Claude Code behavior and external service requirements against current official documentation.

## Use safely

1. Read the guide for the feature you plan to configure.
2. Inspect the corresponding implementation files and permission settings.
3. Adapt a minimal configuration for your environment and back up existing settings.
4. Verify commands and behavior locally before enabling hooks, tools, or external servers.

Do not commit credentials, private memory, or personal configuration. Treat network-connected MCP servers and shell hooks as code with external effects.

## Status and verification

This repository is a reference and example collection, not a deployable application. No tests or examples were run as part of this README update. Historical reports and dated tips may no longer match current product behavior; check their source and date before relying on them.

## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)
