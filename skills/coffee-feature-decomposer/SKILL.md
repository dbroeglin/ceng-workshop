---
name: coffee-feature-decomposer
description: Decomposes a single Coffee Machine 3.0 feature idea into a JIRA-ready Epic with Stories and Tasks. Use when the user proposes a feature and asks for a backlog, ticket breakdown, or "how would we build this?"
---

# Coffee Feature Decomposer

Takes a one-line Coffee Machine 3.0 feature idea and produces a structured backlog: one Epic, 2–5 Stories per Epic, 1–4 Tasks per Story.

> Repo-wide context — the product brief, personas, glossary, scope rules, and JIRA conventions — lives in `.github/copilot-instructions.md`. This skill builds on top of it and does not repeat it.

## When to use
- User proposes a Coffee Machine 3.0 feature idea
- User asks for JIRA tickets, a backlog, an epic, or a feature breakdown
- User says "how would we build [coffee-related thing]"

## When NOT to use
- User asks for code or implementation details
- User asks about a different product

## Inputs to gather first
- The feature one-liner (required)
- Which persona it primarily serves (ask if unclear)
- Any extra constraint not already in the brief

## Output format
> TODO (Challenge 2): replace this with the concrete spec.
>
> Suggested skeleton:
> - **Epic:** title with team prefix, description, success criteria, link to a brief section
> - **Story:** title, "As a [persona] / I want / So that," Given/When/Then acceptance criteria
> - **Task:** engineer-readable, less than one day
> - **JIRA fields:** per the JIRA configuration in `.github/copilot-instructions.md`

Every story names a persona by name and uses at least one glossary term.

## Examples
> TODO (Challenge 2): reference your gold-standard story from `examples/gold-story.md`.

## Anti-patterns to refuse
- Stories without acceptance criteria
- Tasks larger than one day
- Story titles that don't say what's being built (e.g. "Improve UX")

## After generating
- Show the structure for user review before pushing
- Offer to push to JIRA via the MCP server
- Ask which items go to backlog vs. explicitly out-of-scope
