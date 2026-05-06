# Coffee Machine 3.0 — Context Engineering Workshop

A 60-minute hands-on workshop on context engineering with GitHub Copilot. You'll build a `coffee-feature-decomposer` skill that turns a one-line feature idea into a JIRA-ready Epic + Stories + Tasks via the JIRA MCP server.

The skill you build is yours to keep. The structure is portable — swap "coffee" for any domain in your real work.

## Before you start

1. Read [SETUP.md](SETUP.md) and verify your APM, `skill-creator`, and JIRA MCP setup are working.
2. Skim [specs/coffee-machine-3.0-brief.md](specs/coffee-machine-3.0-brief.md) for the product context.
3. Note your **team identifier** (e.g. `T1`) — your facilitator gives this to you. You'll use it on every JIRA ticket.

## How to work through the workshop

Challenges live in `challenges/`. Do them in order:

1. **[challenges/00-mcp-setup.md](challenges/00-mcp-setup.md)** — Verify your JIRA MCP plumbing and learn lesson zero. (5 min)
2. **[challenges/01-who-and-what.md](challenges/01-who-and-what.md)** — Bootstrap your skill, enrich repo context (persona + glossary). (15 min)
3. **[challenges/02-shape-and-example.md](challenges/02-shape-and-example.md)** — Lock in skill output structure, write a gold story, push to JIRA. (15 min)
4. **[challenges/03-stretch-curveballs.md](challenges/03-stretch-curveballs.md)** — Stretch goals for fast finishers. (10 min)

## Files you'll touch

- [specs/personas/brenda.md](specs/personas/brenda.md) — the persona you'll fill in
- [specs/glossary.md](specs/glossary.md) — the vocabulary you'll define
- [examples/gold-story.md](examples/gold-story.md) — the gold-standard story you'll write
- [.github/copilot-instructions.md](.github/copilot-instructions.md) — JIRA configuration block you'll fill in
- [skills/coffee-feature-decomposer/SKILL.md](skills/coffee-feature-decomposer/SKILL.md) — your take-home artifact

## The take-home

A working skill that turns fuzzy feature ideas into structured backlogs. Adapt it to anything you actually work on.

## Links

- https://support.atlassian.com/atlassian-rovo-mcp-server/docs/configuring-authentication-via-api-token/