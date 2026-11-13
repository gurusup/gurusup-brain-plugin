---
name: connecting-gurusup-sources
description: "Use when the user wants Gurusup to learn from a tool (Slack, Notion, Google Drive, Gmail, a CRM...), choose what it reads there, import older history, decide who can read what a source supplies, or disconnect a source, OR when you are about to call sources.connect, sources.history_import, sources.set_access, sources.drive_select, sources.gmail_select, sources.disconnect or sources.webhook_setup."
---
# Connecting Gurusup sources

Sources supply knowledge. Apps separately authorize actions (`connecting-gurusup-apps`). Your assistant's own connectors do not grant Gurusup access: a source is connected only on Gurusup's connection page.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="connecting-gurusup-sources"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If it returns a list of topics instead of the guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Credentials, tokens and API keys are entered only on Gurusup's connection page. Never ask for them in the chat.
- A source learns from the moment it is connected. Connecting never imports older history; that is a separate import the person agrees to.
- Confirm before anything that removes or narrows: turning an app off for the organization disconnects every member's account of that app; switching off areas in Factorial, Sesame or Zernio, or leaving folders out of a Drive selection, removes that content from memory; disconnecting stops learning.
- Confirm who will read a source before changing its access.
- Only report a source as connected when its status is `active` or `connected`.
