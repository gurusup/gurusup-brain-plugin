---
name: creating-gurusup-agents
description: "Use when the user wants to create, change, organize or review a Gurusup agent or routine (\"create an agent that...\", \"automate this every morning\", \"change what my agent does\", \"add a skill to my agent\"), OR when you are about to call agents.create, agents.update, agents.delete, agents.test_goal, agents.set_access, jobs.create, jobs.update or sections.move."
---
# Creating Gurusup agents

An agent is a teammate for one area, such as Sales. It runs the processes written in its assigned skills, with the apps and knowledge it is given. Routines make it act on a schedule.

Before acting, read the full guide from Gurusup: call the Gurusup `learn` tool with `topic="creating-gurusup-agents"`. Follow the guide it returns: it is the source of truth and changes as Gurusup does. If it returns a list of topics instead of the guide, this part of Gurusup is not available for this organization: say so instead of improvising.

## Hard rules

- If the person wants to start a conversation before choosing a purpose, create a personal agent with a provisional name and omit `goal` (or send `""`). Do not invent a goal from a greeting or require a skill first. The agent asks what they need and proposes its name and goal in the web conversation; the owner can agree there.
- For a defined process: process, then skill, then agent. Write, review and publish the process as a skill first (`writing-gurusup-skills`), then assign it through `skill_slugs`. The goal says what the agent is for and never copies the process.
- Look for the area's existing specialist before creating a new agent; add the skill to it when it fits.
- Restate the agreed work in one short paragraph and get one confirmation before `agents.create` or `agents.update`.
- Test a new goal with a real example before saving it. Skip the test only when the person explicitly asks. Only the owner can run the test; if someone else edits a shared agent's goal, suggest the owner tests it, and save untested only if the person explicitly chooses to.
- Routines are created paused. Offer to run one once first, and never turn it on without the person saying so.
- Try a process in chat with the agent before creating its routine, and iterate an existing routine with `jobs.update`.
- Use the context the person supplies for this task and authorized Gurusup sources. Get explicit consent before sharing private material with the organization.
