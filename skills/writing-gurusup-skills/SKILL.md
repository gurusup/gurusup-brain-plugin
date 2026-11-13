---
name: writing-gurusup-skills
description: "Use when the user wants to save how their team does something as a Gurusup skill, or to create, update, publish, approve or review a company skill, OR when you are about to call skills_publish, skills_update, skills.publish_package, skills.edit, skills.upload_link, skills.change_status or skills.propose_drafts."
---
# Writing Gurusup skills

A company skill holds one process: its steps, its source of truth and when to act alone versus ask first. Skills are shared with the organization and used by assistants and agents.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="writing-gurusup-skills"`. If it returns a list of topics instead of the guide, call `learn` with `topic="skills"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If neither returns a guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- One skill per process. Write the steps, the source of truth, the apps it reads and acts in and the criteria for acting alone versus asking first.
- Review the skill with the person before publication, and publish only the approved skill, with an explicit yes for that skill and audience.
- Before uploading, compare purpose and steps against `skills.available`, not only names; read matching skills in full. Propose updating an equivalent skill instead of creating a duplicate (it may have come through another assistant); explain the changes and ask for an explicit yes for that update and audience.
- Never share assistant memory, conversations or private fragments with the organization without explicit consent. Permission to review history is not permission to upload it.
- Every new skill or version starts pending until an organization admin approves it, including an admin's own.
