# Gurusup plugin

Brings Gurusup, your company's memory, into Claude. It bundles the Gurusup MCP server (OAuth sign-in with your Gurusup account) and Gurusup's skills, which tell Claude when to use Gurusup and which guide to read before acting.

## Install (Claude Code)

```
/plugin marketplace add gurusup/gurusup-brain-plugin
/plugin install gurusup-brain@gurusup
```

The first Gurusup call opens a browser to sign in. If you already added the Gurusup MCP by hand, remove it first (`claude mcp remove gurusup`) so the tools don't show up twice.

## What it sends and where

The plugin runs no local code. Claude calls the Gurusup MCP server, run by Gurusup, sending the questions and search terms it needs to answer you. You sign in with your Gurusup account through OAuth, and the server only returns what that account is allowed to see. You need a Gurusup account to use it. Privacy policy: https://gurusup.com/privacy#brain

## Contents

| Path | What |
|------|------|
| `.claude-plugin/plugin.json` | Plugin manifest |
| `.claude-plugin/marketplace.json` | Marketplace entry, so the repo installs directly |
| `.mcp.json` | Gurusup MCP server for Claude, `https://mcp.brain.gurusup.com/mcp` |
| `plugin.json`, `mcp.json` | Same plugin in the [Agent Plugins](https://agent-plugins.org) format, for ChatGPT and other clients |
| `skills/asking-teammates-with-gurusup/` | Asking teammates with Gurusup |
| `skills/choosing-gurusup-source-scope/` | Choosing what Gurusup learns from a source |
| `skills/connecting-gurusup-apps/` | Connecting Gurusup apps |
| `skills/connecting-gurusup-sources/` | Connecting Gurusup sources |
| `skills/creating-gurusup-agents/` | Creating Gurusup agents |
| `skills/managing-gurusup-memory/` | Managing Gurusup memory |
| `skills/managing-gurusup-organization/` | Managing your Gurusup organization |
| `skills/setting-up-gurusup/` | Setting up Gurusup |
| `skills/using-gurusup/` | Using Gurusup |
| `skills/working-with-gurusup-agents/` | Working with Gurusup agents |
| `skills/writing-gurusup-skills/` | Writing Gurusup skills |

The skills are generated from the skills the Gurusup MCP serves (`learn`): each one keeps the same name and trigger, its hard rules, and points to the full guide. Don't edit them by hand; changes arrive as an automatic sync PR, which never bumps the version. Releases bump `version` in their own PR.

Validate after changes: `claude plugin validate .`. Keep `version` in `.claude-plugin/plugin.json` and `plugin.json` in sync.

Full docs: https://gurusup.com/brain/mcp
