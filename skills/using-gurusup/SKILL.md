---
name: using-gurusup
description: "Use for questions about the user's company (customers, projects, people, decisions, meetings, policies, sales, support, roadmap or company history) that Gurusup can answer from the company's connected sources, OR when you are about to call ask_company_memory, search_company_memory or retrieve_company_memory, OR when you are not sure which Gurusup skill covers a request. Lists every Gurusup skill."
---
# Using Gurusup

Gurusup holds the company's memory, unified across its connected sources. Answer company questions from what Gurusup returns, and use the other Gurusup skills to set it up and operate it.

Before acting, read the full skill from Gurusup: call the Gurusup `learn` tool with `topic="using-gurusup"` and follow it. It is the source of truth and changes as Gurusup does. If `learn` does not offer it, it is not available for this organization: say so instead of improvising.

## Hard rules

- Call `init` once per task or session before the first read, and follow the contract it returns.
- Answer only from the evidence Gurusup returns. If it returns no evidence or too little, say so instead of guessing.
- Never invent a subject, a contact or a fact. Company memory is not a contact directory.
- Before any change in the organization, read the Gurusup skill that covers it (`learn` lists them) and confirm with the person.
