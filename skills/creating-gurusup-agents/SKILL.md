---
name: creating-gurusup-agents
description: Use when the user wants to create, change or review a Gurusup agent or routine - for example "create an agent that...", "automate this every morning", "change what my agent does" or "add a skill to my agent".
---

# Creating Gurusup agents

Before creating or changing any agent, call the Gurusup `learn` tool with `topic="agents"` and follow that guide. It is the source of truth and it changes as Gurusup does.

The short version:
1. Process, then skill, then agent. Write the process (steps, sources of truth, actions, what to do alone versus ask first) as a skill, publish it, and assign it to the agent.
2. The agent's goal says what the agent is for: its area, its voice in one line and what it does not do. It never repeats the process.
3. Look for an existing agent for that area before creating a new one, and add the skill to it when it fits.
4. Test the goal with a real example before saving it, and keep routines paused until they are tested.

If `learn` does not offer the agents topic, agents are not available for this organization: tell the user instead of improvising.
