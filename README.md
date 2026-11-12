# Gurusup plugin

Brings Gurusup, your company's memory, into Claude. It bundles the Gurusup MCP server (OAuth sign-in with your Gurusup account) and a skill that tells Claude to check Gurusup first for anything about your company.

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
| `skills/using-gurusup/` | Check Gurusup first, follow the `init` contract |
| `skills/creating-gurusup-agents/` | Create or change agents: process, then skill, then agent |
| `skills/setting-up-gurusup/` | Getting started and "set it up for me" |
| `skills/connecting-apps-and-sources/` | Connect sources (knowledge) and apps (actions) |
| `skills/writing-gurusup-skills/` | Create or update company skills without duplicates |

Validate after changes: `claude plugin validate .`. Keep `version` in `.claude-plugin/plugin.json` and `plugin.json` in sync.

Full docs: https://gurusup.com/brain/mcp
