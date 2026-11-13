---
name: connecting-gurusup-apps
description: "Use when the user wants Gurusup or one of its agents to act in an app (send, create or update in Slack, Gmail, a CRM...), needs an app that is not in the catalog, wants to control which actions need approval, or wants an agent to use a website through the browser (browser use), OR when you are about to call apps.connect, apps.add_remote, apps.set_policy, agents.set_apps, websites.setup or websites.assign."
---
# Connecting Gurusup apps

Apps let agents act: send, create or update things in other tools. Browser use covers websites without an app. They are separate from sources, which only supply knowledge. Each account has its actions set to run automatically, need approval, or be blocked.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="connecting-gurusup-apps"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If it returns a list of topics instead of the guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Credentials are entered only on Gurusup's connection page. Never ask for tokens or secrets in the chat.
- Only confirm a connection once it is active, using `account_name` and `scope`. When only the app name is known, do not claim to know the email or account.
- Keep the work in Gurusup. Never propose running it outside Gurusup to reach a missing app.
- Preserve approval policies unless the person asks to change them.
- Confirm before turning an app or an account off, disconnecting, or removing browser use from an agent: agents lose that access.
