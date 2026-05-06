# Coffee Machine 3.0 — Product Brief (DRAFT)

> Status: Half-baked. Some sections are deliberately fuzzy. Your job in the workshop is not to fix the brief — it is to engineer enough context that Copilot can produce sensible stories *despite* the fuzziness.

## Vision
Coffee Machine 3.0 turns the office espresso ritual into a delightful, fair, and slightly opinionated experience. It knows you. It paces you. It judges you a little. It never runs out of beans on a Monday.

## The problem
Today's office coffee experience is broken in three ways:
1. **The queue is chaos.** People hover. People cut. People take 14 minutes for a flat white.
2. **The machine has no memory.** Brenda orders the same cortado every day at 9:02 and still has to tap through six menus.
3. **Hoarding.** Three people on the 4th floor have stockpiled the oat milk again.

## Users
- **Daily drinkers** — show up, want their usual, in and out.
- **Occasional drinkers** — need help choosing, easily intimidated by the menu.
- **Connoisseurs** — want grind size, temperature, dwell time, and to be heard.
- **Visitors** — no profile, no clue, very thirsty.

## In scope (v1)
- Queue management with calendar-aware pre-brewing
- Per-user "usual" memory
- Anti-hoarding controls for shared supplies
- Mood-aware suggestions (optional, controversial)

## Out of scope
- Payments and billing
- Social feed, ratings, leaderboards
- Integration with the building's HVAC
- Anything involving facial recognition

## Success metrics
- TBD. Something about throughput? Satisfaction? Bean efficiency? Define this with your team during the workshop — vague success metrics are exactly the kind of thing context engineering must pin down.

## Constraints
- Must work when the WiFi is flaky (it will be).
- Must not embarrass anyone (no public mood broadcasts).
- Must finish a brew before the 10:00 standup, or there will be revolt.
- Must support visitors without forcing account creation.

## Open questions (these are gold for context engineering)
- How does it handle visitors with no profile?
- What happens when two daily drinkers both want the last shot of espresso?
- Is "mood detection" creepy or delightful? Where is the line?
- What does "fairness" mean for shared supplies — per person, per team, per floor?
