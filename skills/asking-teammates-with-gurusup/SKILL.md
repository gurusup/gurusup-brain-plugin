---
name: asking-teammates-with-gurusup
description: "Use when a company fact is still missing after searching memory and a teammate should be asked, when the user asks who can be asked about a topic, wants to follow up a question sent to a teammate, or manages who can be contacted, OR when you are about to call request_human_info, human_info.confirm, human_info.retry, contacts.create or contacts.update."
---
# Asking teammates with Gurusup

Contacts describe who knows which topics and how Gurusup can reach them. When company memory cannot answer a necessary fact, Gurusup can ask the right teammate on the person's behalf.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="asking-teammates-with-gurusup"`. If it returns a list of topics instead of the guide, call `learn` with `topic="organization"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If neither returns a guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Ask a teammate only for a necessary company fact that is still unsupported after asking memory and a focused search. Never for an unclear request, optional details, an access limit or a service error.
- Always preview first with `dispatch=false`, and send only after the person confirms the contact and the question.
- Company memory is not a contact directory. Never pick a contact from evidence; name one only when the person explicitly asks to contact that person.
- Carry the same `activity_id` from the memory question through the preview and the send. Never drop or replace it.
- `human_info.retry` and `contradictions.ask_contact` send right away; ask the person first.
