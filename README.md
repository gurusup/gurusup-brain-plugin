# GuruSup Brain plugin

Brings GuruSup Brain, your company's memory, into Claude. It bundles the Brain MCP server (OAuth sign-in with your GuruSup account) and a skill that tells Claude to check Brain first for anything about your company.

## Install (Claude Code)

```
/plugin marketplace add gurusup/gurusup-brain-plugin
/plugin install gurusup-brain@gurusup
```

The first Brain call opens a browser to sign in. If you already added the Brain MCP by hand (`claude mcp remove gurusup`), remove it first so the tools don't show up twice.

## Contents

| Path | What |
|------|------|
| `.claude-plugin/plugin.json` | Plugin manifest |
| `.claude-plugin/marketplace.json` | Marketplace entry, so the repo installs directly |
| `.mcp.json` | Brain MCP server, `https://mcp.brain.gurusup.com/mcp` |
| `skills/using-brain/` | Check Brain first, follow the `init` contract |

Validate after changes: `claude plugin validate .`
