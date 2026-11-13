---
name: managing-gurusup-memory
description: "Use when the user asks what Gurusup has learned, whether its memory is up to date or still building, wants to save a fact, exclude content, review conflicting facts or see memory activity, OR when you are about to call memory.start, memory.retry, memory.exclude_content, contradictions.decide, contradictions.ask_contact or add_company_knowledge."
---
# Managing Gurusup memory

Gurusup's memory is what it has learned from the organization's sources, notes and decisions. This skill covers building it, checking it, saving facts into it, resolving conflicting facts and reading its activity.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="managing-gurusup-memory"`. If it returns a list of topics instead of the guide, call `learn` with `topic="memory-build"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If neither returns a guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- Reading progress never starts work. Use `memory.start` or `memory.retry` only when the person asks and `memory.status` says it is allowed (`start_allowed`, `retry_allowed`).
- Never describe documents that are waiting or being prepared as already in memory.
- Save a fact with `add_company_knowledge` only with the person's consent, and always ask who may read it unless they said so: only them, named people, or the organization.
- Decide a conflicting fact only with the person's supported decision. Ask before `contradictions.ask_contact`: it sends the question to a teammate right away, with no preview.
