# claude-code-best-practice

> An engineering project in the HMZ GitHub portfolio.

<p align="center">
  <a href="https://github.com/hmzainjamil/hmz-claude-code-best-practice">Repository</a> ·
  <a href="https://github.com/hmzainjamil/hmz-claude-code-best-practice/commits/main">Commits</a> ·
  <a href="https://github.com/hmzainjamil/hmz-claude-code-best-practice/issues">Issues</a>
</p>

<p align="center"><img alt="Visibility" src="https://img.shields.io/badge/visibility-public-blue"> <img alt="Lifecycle" src="https://img.shields.io/badge/lifecycle-active-success"> <img alt="Documentation" src="https://img.shields.io/badge/documentation-deep%20editorial-lightgrey"></p>

<!-- HMZ DEEP README v1 -->

## At a glance

| Field | Current state |
|---|---|
| Visibility | public |
| Lifecycle | Active |
| Repository size | 5795 KB |
| Default branch | main |
| Evidence basis | Current repository documentation and source-visible material |

## Why this exists

An engineering project in the HMZ GitHub portfolio.

This README separates documented capabilities from measured evidence and avoids converting roadmap ideas or external assumptions into implementation claims.

## 🧠 CONCEPTS

| Feature | Location | Description |
|---------|----------|-------------|
| <img src="!/tags/a.svg" height="14"> [**Subagents**](https://code.claude.com/docs/en/sub-agents) | `.claude/agents/<name>.md` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-subagents.md) [![Implemented](!/tags/implemented.svg)](implementation/claude-subagents-implementation.md) Autonomous actor in fresh isolated context — custom tools, permissions, model, memory, and persistent identity |
| <img src="!/tags/c.svg" height="14"> [**Commands**](https://code.claude.com/docs/en/slash-commands) | `.claude/commands/<name>.md` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-commands.md) [![Implemented](!/tags/implemented.svg)](implementation/claude-commands-implementation.md) Knowledge injected into existing context — simple user-invoked prompt templates for workflow orchestration |
| <img src="!/tags/s.svg" height="14"> [**Skills**](https://code.claude.com/docs/en/skills) | `.claude/skills/<name>/SKILL.md` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-skills.md) [![Implemented](!/tags/implemented.svg)](implementation/claude-skills-implementation.md) Knowledge injected into existing context — configurable, preloadable, auto-discoverable, with context forking and progressive disclosure · [Official Skills](https://github.com/anthropics/skills/tree/main/skills) |
| [**Workflows**](https://code.claude.com/docs/en/common-workflows) | [`.claude/commands/weather-orchestrator.md`](.claude/commands/weather-orchestrator.md) | [![Orchestration Workflow](!/tags/orchestration-workflow.svg)](orchestration-workflow/orchestration-workflow.md) |
| [**Hooks**](https://code.claude.com/docs/en/hooks) | `.claude/hooks/` | [![Best Practice](!/tags/best-practice.svg)](https://github.com/shanraisshan/claude-code-hooks) [![Implemented](!/tags/implemented.svg)](https://github.com/shanraisshan/claude-code-hooks) User-defined handlers (scripts, HTTP, prompts, agents) that run outside the agentic loop on specific events · [Guide](https://code.claude.com/docs/en/hooks-guide) |
| [**MCP Servers**](https://code.claude.com/docs/en/mcp) | `.claude/settings.json`, `.mcp.json` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-mcp.md) [![Implemented](!/tags/implemented.svg)](.mcp.json) Model Context Protocol connections to external tools, databases, and APIs |
| [**Plugins**](https://code.claude.com/docs/en/plugins) | distributable packages | Bundles of skills, subagents, hooks, MCP servers, and LSP servers · [Marketplaces](https://code.claude.com/docs/en/discover-plugins) · [Create Marketplaces](https://code.claude.com/docs/en/plugin-marketplaces) |
| [**Settings**](https://code.claude.com/docs/en/settings) | `.claude/settings.json` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-settings.md) [![Implemented](!/tags/implemented.svg)](.claude/settings.json) Hierarchical configuration system · [Permissions](https://code.claude.com/docs/en/permissions) · [Model Config](https://code.claude.com/docs/en/model-config) · [Output Styles](https://code.claude.com/docs/en/output-styles) · [Sandboxing](https://code.claude.com/docs/en/sandboxing) · [Keybindings](https://code.claude.com/docs/en/keybindings) · [Fast Mode](https://code.claude.com/docs/en/fast-mode) |
| [**Status Line**](https://code.claude.com/docs/en/statusline) | `.claude/settings.json` | [![Best Practice](!/tags/best-practice.svg)](https://github.com/shanraisshan/claude-code-status-line) [![Implemented](!/tags/implemented.svg)](.claude/settings.json) Customizable status bar showing context usage, model, cost, and session info |
| [**Memory**](https://code.claude.com/docs/en/memory) | `CLAUDE.md`, `.claude/rules/`, `~/.claude/rules/`, `~/.claude/projects/<project>/memory/` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-memory.md) [![Implemented](!/tags/implemented.svg)](CLAUDE.md) Persistent context via CLAUDE.md files and `@path` imports · [Auto Memory](https://code.claude.com/docs/en/memory) · [Rules](https://code.claude.com/docs/en/memory#organize-rules-with-clauderules) |
| [**Checkpointing**](https://code.claude.com/docs/en/checkpointing) | automatic (git-based) | Automatic tracking of file edits with rewind (`Esc Esc` or `/rewind`) and targeted summarization |
| [**CLI Startup Flags**](https://code.claude.com/docs/en/cli-reference) | `claude [flags]` | [![Best Practice](!/tags/best-practice.svg)](best-practice/claude-cli-startup-flags.md) Command-line flags, subcommands, and environment variables for launching Claude Code · [Interactive Mode](https://code.claude.com/docs/en/interactive-mode) |
| **AI Terms** | | [![Best Practice](!/tags/best-practice.svg)](https://github.com/shanraisshan/claude-code-codex-cursor-gemini/blob/main/reports/ai-terms.md) Agentic Engineering · Context Engineering · Vibe Coding |
| [**Best Practices**](https://code.claude.com/docs/en/best-practices) | | Official best practices · [Prompt Engineering](https://github.com/anthropics/prompt-eng-interactive-tutorial) · [Extend Claude Code](https://code.claude.com/docs/en/features-overview) |

## Architecture

No verified architecture section was available in the current README, so no architecture is invented here.

## Getting started

No verified installation procedure was available in the current README. Use the repository root, dependency manifests, and project docs as the source of truth.

## Usage

No verified runtime command was available in the current README. Commands should be taken from the repository's executable entry points and package configuration.

## Configuration

Configuration should be taken from environment examples, package configuration, and runtime entry points. Secrets should never be committed.

## Validation and evidence

No dedicated test or evaluation section was available in the current README. Performance, production readiness, and outcome claims are therefore not asserted here.

## Security

Keep credentials outside the repository, validate untrusted inputs at system boundaries, and grant external tools only the permissions they require.

## Limitations

- This README reports the current documented state and does not convert planned functionality into completed functionality.
- Quantitative claims should be backed by reproducible repository evidence or linked test artifacts.
- External service behavior, provider limits, and current pricing are not inferred from repository documentation.



## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)