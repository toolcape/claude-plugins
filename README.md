# Toolcape for Claude

The Toolcape plugin adds the Toolcape connector (`https://toolcape.com/mcp`) to Claude, plus a
skill that teaches Claude how to use it. You sign in once with your work account; Claude then
reaches the services your organization has connected in Toolcape, as you.

## Install

**Claude (web, desktop, Cowork):** Customize → Plugins → **+** → Add marketplace → `toolcape/claude-plugins`,
then install **Toolcape**.

**Claude Code:**

```bash
claude plugin marketplace add toolcape/claude-plugins
claude plugin install toolcape@toolcape
```

**VS Code:** open this link, which opens the Claude Code plugin dialog on Toolcape:

```text
vscode://anthropic.claude-code/install-plugin?plugin=toolcape&marketplace=toolcape/claude-plugins
```

Then sign in when Claude asks you to connect Toolcape.

## Only the connector?

Add a custom connector in Claude with the URL `https://toolcape.com/mcp`.
