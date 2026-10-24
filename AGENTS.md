# Repository layout

- `plugins/<name>/` – installable plugins (`plugin.json`, `skills/`, `agents/`). Each must be listed in both marketplace manifests.
- `skills/<name>/SKILL.md` – standalone skills (front matter `name`, `description`).
- `agents/<name>.agent.md` – standalone agent definitions.
- `instructions/*.instructions.md` – reusable instruction files.
- `.github/plugin/marketplace.json` – marketplace manifest (Copilot CLI, VS Code, Visual Studio).
- `.claude-plugin/marketplace.json` – identical copy (Claude Code-compatible tools, OpenCode plugins).

Keep the two marketplace manifests identical. Plugin skills/agents are copies of the standalone ones.
