# Challenge 0 — Hello, JIRA (5 min)

**Goal:** prove the MCP plumbing works AND learn lesson zero of context engineering before the main game starts.

## Step 1 — Try the naive ask

Ask Copilot:
> "Create a JIRA ticket titled 'Hello from team [your-team-id]'."

Observe what happens. It will probably fail, ask follow-up questions, or land somewhere unexpected.

## Step 2 — What did Copilot need to know?

Discuss in your team. Write down everything Copilot needed but wasn't told:
- ?
- ?
- ?

> Hint: project key, issue type, assignee, labels, your team prefix...

This list IS context engineering, in miniature.

## Step 3 — Add JIRA configuration to your context

Open `.github/copilot-instructions.md`. Find the `## JIRA configuration` block. Fill it in with the values your facilitator gave you:

- Instance URL
- Project key
- **Your team identifier** (`T1`, `T2`, ...)
- **Issue title prefix** — always start titles with `[T1]` (substitute your team ID)
- Default issue type: `Task`
- **Required labels** — must include `team-T1` (substitute your team ID)
- Default assignee: `unassigned`

> ⚠️ The team identifier, prefix, and label are NOT optional. The whole workshop shares ONE JIRA project — without these, your tickets collide with other teams' tickets and nobody can find anything.

## Step 4 — Re-run

Same prompt as Step 1. Your ticket should now land in the right place with the right metadata, prefix, and label.

## Step 5 — Clean up

Close the test ticket so it doesn't pollute your backlog.

---

**Done?** Move to Challenge 1.
