# ai-marketplace

Central marketplace for Copilot instructions, agents, skills and plugins.

## Structure

| Path | Purpose |
|------|---------|
| `plugins/` | Installable plugins bundling skills/agents |
| `skills/` | Standalone skills (`<name>/SKILL.md`) |
| `agents/` | Standalone agents (`<name>.agent.md`) |
| `instructions/` | Reusable instruction files |
| `.github/plugin/marketplace.json` | Marketplace manifest (Copilot) |
| `.claude-plugin/marketplace.json` | Same manifest for Claude-format consumers |
| `.github/copilot-instructions.md`, `AGENTS.md` | Instructions for this repo |

## Registering the marketplace

- **Copilot CLI**: `copilot plugin marketplace add zss-rzwart/ai-marketplace`, then `copilot plugin install example-plugin@ai-marketplace`.
- **VS Code / Visual Studio**: add `zss-rzwart/ai-marketplace` as a plugin marketplace (e.g. VS Code setting `chat.plugins.marketplaces`).
- **OpenCode**: copy or symlink `skills/` and `agents/` entries into `.opencode/skills` and `.opencode/agents` (or `~/.config/opencode/`).

## Adding content

Copy `plugins/example-plugin`, rename it, and register it in both marketplace manifests.
