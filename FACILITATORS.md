# Facilitator Guide — DO NOT SHARE WITH PARTICIPANTS

Everything participants don't need to see: timing, intervention triggers, JIRA conflict mitigation, curveball reveal timing, between-sessions retro.

## Workshop arc

The teaching arc is **same prompt, different context → wildly different output.** Context is the variable participants manipulate. The artifact they walk away with is a working `coffee-feature-decomposer` skill.

## Timing (60 min)

| Time | Phase | Outcome |
|------|-------|---------|
| 0–3' | Frame the game | Brief introduced; teams know their feature one-liner and team ID |
| 3–8' | Challenge 0 — MCP smoke test | Plumbing verified; project key / team prefix lesson lands |
| 8–13' | Naked prompt → JIRA slop | Visible "before" baseline |
| 13–28' | Challenge 1 — Who and What | Persona + glossary added; re-run shows specificity |
| 28–43' | Challenge 2 — Shape and Example | Output contract + gold story; biggest quality jump |
| 43–53' | Challenge 3 — Curveballs (stretch) | Fast finishers stress-test their skill |
| 53–60' | Debrief + take-home | Skill is the souvenir |

If a team isn't ready for Challenge 3 by minute 43, that's fine — Challenge 3 is intentionally optional. Don't shortchange the debrief to fit it in.

## Single JIRA project — conflict mitigation

You have ONE JIRA project for all teams across both sessions. Without conventions, teams trip over each other within minutes. Enforce these from the start:

### Mandatory naming conventions (assign before workshop)
- **Team identifier:** assign each team `T1`, `T2`, `T3`, ... Print on cards. Make it visible.
- **Issue title prefix:** every issue starts with `[T1] ...`. No exceptions.
- **Mandatory label:** every issue carries label `team-T1` (substitute team ID).
- **Component:** if components are configured, assign one per team and require its use.
- **Epic ownership:** each team works under its own root epic (`[T1] Coffee Machine 3.0`). Stories attach only to your own team's epic.

### Behavioral rules
- Never edit or close another team's issue.
- Never move issues to an active sprint — keep everything in the backlog.
- Don't @-mention real people; use placeholder mentions like `@coffee-product-owner`.
- If the project gets cluttered between sessions, bulk-update session 1's tickets with label `archived-session-1` rather than deleting.

### Saved JQL filter per team
Pre-create one filter per team and share the URL — saves people from staring at 80 mixed tickets:
```
project = COFFEE AND labels = "team-T1"
```

### Between sessions
- Bulk-label all session 1 tickets `archived-session-1` (or close them).
- Reuse `T1`, `T2`, ... or rotate to `T4`, `T5`, ... — whichever is less confusing for your group.
- Capture session 1 surprises in the per-challenge notes below.

## Pre-flight checklist
- [ ] JIRA project exists; team-prefix labels and components configured
- [ ] One saved JQL filter per team; URLs ready to hand out
- [ ] JIRA MCP server endpoint + auth tokens prepared per team
- [ ] APM install URL projected and verified
- [ ] `apm.yaml` validated against current APM spec
- [ ] You've run the full flow end-to-end with a stopwatch
- [ ] Backup plan if MCP fails (manual JIRA copy-paste lane)

## Per-challenge facilitator notes

### Challenge 0 — MCP smoke test
- The naive ask SHOULD fail. If it doesn't (because Copilot inferred the project), reframe: "what would happen tomorrow when you have 5 projects and Copilot picks the wrong one?" Same lesson, same impact.
- The discovery list (project key, issue type, etc.) IS the lesson. Write it on the whiteboard. Photograph it. Refer back to it in later challenges.
- Do NOT pre-fill the JIRA configuration block in `.github/copilot-instructions.md`. Let them discover.

### Challenge 1 — Who and What
- skill-creator can over-discuss naming. If a team is stuck for 2+ minutes, intervene with a suggested skill name.
- The reveal moment is when the same prompt produces stories that actually name Brenda. Make sure each team gets that hit.
- Glossary tip: 4–6 terms is plenty. Don't let them perfectionize.

### Challenge 2 — Shape and Example
- The few-shot gold story is the single biggest quality jump in the whole workshop. Time-box the writing to 5 minutes — perfectionism is the enemy.
- If a team writes a mediocre gold story, run it anyway. Comparing mediocre→pattern-match output is itself instructive.

### Challenge 3 — Curveballs (stretch)
- Reveal only at minute 43. Hand each finishing team one curveball.
- Curveball #5 (Visitor Mode) is the best stress test — it forces them to confront the persona they didn't write. Save it for the team that finished first or looks confident.
- If no team gets here, don't apologize. Mention it in debrief as a take-home extension.

## Watch-outs
- **Resist code questions.** Standard redirect: "that's the platform team's job — your job is to write a story so good they can't misinterpret it."
- **Identity drift.** When stories stop naming personas, prompt: "who is this for, by name?"
- **Silent MCP failure.** If a team is suspiciously quiet for 5 minutes, check their tickets are actually landing in JIRA.

## Between-sessions retro (5 min after session 1)
Capture in three buckets:
1. What surprised me? (good or bad)
2. What context-engineering technique landed best?
3. What scaffolding should be different next session?

Fold #3 into the starter scaffold for session 2 — live demo of "context engineering compounds."

## The take-home
The completed `SKILL.md` is the souvenir. The structure is portable — swap "coffee" for any domain (internal platform, customer onboarding, incident response) and the same context-engineering pattern applies.
