---
name: working-with-gurusup-agents
description: "Use when the user wants to talk to an agent, asks what their agents are doing or what is waiting for them, wants to answer an agent's question or approval, decide a setup card, follow or stop a run, or see or undo an agent's changes, OR when you are about to call conversations.send, conversations.answer, actions.decide, inbox.list, pending_work.list, runs.trace, runs.cancel or agents.put_back."
---
# Working with Gurusup agents

Talk to agents, follow their work, and answer the questions and approvals they send the person.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="working-with-gurusup-agents"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If it returns a list of topics instead of the guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Ask for an explicit decision before approving an action that reaches outside Gurusup. Show its `summary`, app, account and visible references; do not narrate raw arguments.
- Only the person controlling a conversation can answer its questions and approvals; being an admin does not change that. Setup cards are decided only by the agent's current owner, and only with a card decision, never from a text reply.
- Answer in the conversation where the item is shown and with its original id. Never look for a copied request or redirect the person to another conversation.
- Pass a `request_id` when sending a message or an answer, and reuse it only to retry the same message after a lost response. Without it a retry sends twice.
- Stopping a run or cancelling cannot undo actions already done.
