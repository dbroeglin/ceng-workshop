# Challenge 2 — Shape and Example (15 min)

**Goal:** lock in the *task-specific* context — the output structure and a gold-standard example. This turns Challenge 1's enriched content into a structured backlog.

## Step 1 — Define the output contract

Open `skills/coffee-feature-decomposer/SKILL.md`. Find the `## Output format` section. Replace the TODO with a concrete spec:

- **Epic:** title, description, success criteria, link to a brief section
- **Story:** title, "As a [persona] / I want / So that," Given/When/Then acceptance criteria
- **Task:** engineer-readable, less than one day, no implementation details

Be specific. Vague contracts produce vague output.

> Notice: you're NOT writing the team prefix, label, issue type, or any JIRA field in here — those live in `.github/copilot-instructions.md` (filled in Challenge 0). The skill just says "per the JIRA configuration in copilot-instructions.md." One source of truth, less drift.

## Step 2 — Write the gold story

Open `examples/gold-story.md`. Write ONE story you're proud of, following the format above. 5 minutes max — perfectionism is the enemy.

This story defines the quality bar for everything Copilot generates next.

## Step 3 — Wire it into the skill

Back in `SKILL.md`, find the `## Examples` section. Replace the TODO with a reference to `examples/gold-story.md` and the instruction:
> "Match the shape and quality of this example."

## Step 4 — Re-run and push to JIRA

Same feature, same prompt. The output should now look noticeably more like your gold story.

When you're happy:
> "Push these tickets to JIRA."

Check JIRA via your team's saved filter. Tickets land with the right prefix, label, and structure.

🎉 You turned a half-baked one-liner into a JIRA-ready backlog using context alone — no code, no clicking through JIRA UI.

---

**Done?** Move to Challenge 3 if there's time left.
