# Challenge 1 — Who and What (15 min)

**Goal:** see what happens when *repo-wide context* is rich vs. empty — without touching your skill at all.

## Step 1 — Bootstrap the skill

A scaffold is already on disk at `skills/coffee-feature-decomposer/SKILL.md`. You'll use `skill-creator` to *refine* it, not generate it from nothing.

Ask Copilot:
> "Use skill-creator to review and refine the existing skill at skills/coffee-feature-decomposer/SKILL.md. It decomposes a Coffee Machine 3.0 feature one-liner into a JIRA-ready Epic + Stories + Tasks. Help me sharpen the frontmatter (name, description) and triggers. No code."

Skim the suggestions, accept the ones that read better. **Don't touch the `Output format` or `Examples` TODOs yet** — that's Challenge 2.

## Step 2 — First run (the "before")

Pick one feature from `specs/coffee-machine-3.0-brief.md` — for example, "queue management with calendar-aware pre-brewing." Ask Copilot:
> "Use the coffee-feature-decomposer skill to break down [your feature]."

Read the output. It's probably generic — "user" instead of a real person, inconsistent vocabulary. Keep this output around for comparison.

## Step 3 — Fill in Brenda

Open `specs/personas/brenda.md`. Fill in every section. Be specific:
- ❌ "Brenda likes coffee."
- ✅ "Brenda has a 9:02 cortado that gets her through the EMEA standup. If it's late, she gets passive-aggressive in chat."

5 minutes max.

## Step 4 — Build the glossary

Open `specs/glossary.md`. Define every term. Add 1–2 of your own. Crisp definitions, no synonyms.

## Step 5 — Re-run (no skill changes)

Same skill, same prompt, same feature. Compare with Step 2.

What changed? Likely:
- "User" became "Brenda" — by name, with her quirks
- Vocabulary tightened — your glossary terms appear verbatim
- Stories got specific where they were generic before

You didn't touch the skill — only the repo context. `.github/copilot-instructions.md` already grounds in `specs/personas/` and `specs/glossary.md`, so filling those files flowed straight through to the skill's output.

**The lesson:** repo context flows into every skill invocation. Enrich it once, every skill benefits.

---

**Done?** Move to Challenge 2.
