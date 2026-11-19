---
name: using-gurusup
description: "Use for company questions that Gurusup can answer from connected sources, when calling ask_company_memory, search_company_memory or retrieve_company_memory, or to find the skill for a request. If Agents access is off, use it to stop current work, pause existing routines or disconnect agent accounts."
---
# Using Gurusup

Gurusup holds the company's memory, unified across its connected sources. Answer company questions from what Gurusup returns, and use the other Gurusup skills to set it up and operate it.

Call the Gurusup `init` tool first and follow the contract it returns. To find the Gurusup guide for a task, call `learn` without a topic and read the one that covers it.

## Hard rules

- Call `init` once per task or session before the first read, and follow the contract it returns.
- Answer only from the evidence Gurusup returns. If it returns no evidence or too little, say so instead of guessing.
- Never invent a subject, a contact or a fact. Company memory is not a contact directory.
- Before any change in the organization, read the Gurusup skill that covers it (`learn` lists them) and confirm with the person.
