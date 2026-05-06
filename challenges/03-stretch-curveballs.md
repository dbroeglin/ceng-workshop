# Challenge 3 — Curveballs (stretch goal)

If you're here, you've finished the core workshop. Time to stress-test your skill.

Pick ONE curveball below. Run it through your `coffee-feature-decomposer`. Push to JIRA. Compare with your earlier output.

The test: does your context hold up when the feature is harder than the one it was tuned for?

---

## 1. Anti-Hoarding Mode
The machine detects when one team consumes more than 40% of the oat milk and gently nudges them toward fairness.
**Stresses:** privacy boundaries, fairness rules, the "creepy line."

## 2. Mood-Aware Brewing
The machine reads the user's calendar and, before a difficult meeting, suggests something stronger. Strictly opt-in.
**Stresses:** consent flows, opt-in/out defaults, sensitivity.

## 3. Coffee Karma
Pay it forward: queue jumpers lose karma, polite users gain it. Karma unlocks perks (bean-of-the-month, priority pre-brew).
**Stresses:** gamification rules, abuse prevention, glossary discipline.

## 4. Vacation Handover
Brenda is OOO for two weeks. Her usual auto-pauses; her loyalty beans don't expire; her 9:02 slot opens up to others.
**Stresses:** temporal logic, calendar integration, edge cases.

## 5. Visitor Mode
A guest taps the machine. No profile. Get them caffeinated in under 15 seconds without making them feel dumb.
**Stresses:** the persona you didn't write, graceful degradation, default behaviors.

## 6. The Monday Bean Crisis
On Mondays, demand spikes 2.4x baseline. Pre-brewing logic must absorb the spike without wasting beans Tue–Fri.
**Stresses:** trade-offs, success metrics that fight each other, cross-feature interactions.

---

After running it, ask yourself: where did the context fall short? What would you add — to the repo, to the skill — to handle this kind of feature better?

That's the take-home insight: **context engineering is never "done."** It evolves with the kinds of inputs you throw at it.
