# Toolcape for Claude

The Toolcape plugin adds the Toolcape connector (`https://toolcape.com/mcp`) to Claude, plus a
skill that teaches Claude how to use it. You sign in once with your work account; Claude then
reaches the services your organization has connected in Toolcape, as you.

## Install

**Claude (web, desktop, Cowork):** Customize → Plugins → **+** → Add marketplace → `toolcape/claude-plugins`,
then install **Toolcape**.

**Claude Code:**

```bash
claude plugin marketplace add https://github.com/toolcape/claude-plugins
claude plugin install toolcape@toolcape
```

**VS Code:** open this link, which opens the Claude Code plugin dialog on Toolcape:

```text
vscode://anthropic.claude-code/install-plugin?plugin=toolcape&marketplace=https%3A%2F%2Fgithub.com%2Ftoolcape%2Fclaude-plugins
```

Then sign in when Claude asks you to connect Toolcape.

**Updates:** Claude Code doesn't update third-party plugins on its own. Turn it on once in `/plugin` →
Marketplaces → toolcape → Enable auto-update, or run `claude plugin marketplace update toolcape`.

## Only the connector?

Add a custom connector in Claude with the URL `https://toolcape.com/mcp`.

## Releasing

Claude only offers an update when the plugin's version goes up. Bump `version` in
`plugins/toolcape/.claude-plugin/plugin.json` in every change you want people to receive.
