---
name: connecting-apps-and-sources
description: Use when the user wants Gurusup to learn from a tool (connect a source such as Slack, Notion, Drive or a CRM), choose what Gurusup learns from it, or let Gurusup act in an app (connect an app account for actions).
---

# Connecting apps and sources

Sources give Gurusup knowledge; apps let it take actions. They are connected separately.

- To connect a source or check what Gurusup learns from it: call the Gurusup `learn` tool with `topic="knowledge"`, and with `topic="source-scope"` to choose what it learns.
- To connect an app for actions: call `learn` with `topic="apps"`.

Connections always finish on Gurusup's own connection page. Never ask the user for passwords, API keys or tokens in the chat.
