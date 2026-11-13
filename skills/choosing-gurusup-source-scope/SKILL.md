---
name: choosing-gurusup-source-scope
description: "Use when an organization admin wants to choose or change which Linear teams or which Attio companies, deals and people Gurusup keeps learning from, OR when you are about to call sources.scope_get or sources.scope_set."
---
# Choosing what Gurusup learns from a source

Scope narrows what Gurusup keeps learning from a connected Linear or Attio source. Other apps choose what they read in their own way (`connecting-gurusup-sources`).

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="choosing-gurusup-source-scope"`. If it returns a list of topics instead of the guide, call `learn` with `topic="source-scope"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If neither returns a guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Only organization admins choose scope. A member asks an admin.
- Always preview with `sources.scope_set` and `dry_run: true`, show what starts and what stops updating, and save with `dry_run: false` only after the person confirms.
- Use the real unit names returned by `sources.scope_get`; never type values the source did not offer.
