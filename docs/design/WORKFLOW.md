# Design notebook workflow
This is a collaborative exploration framework, not a fixed GDD or implementation backlog.

- Start at the [master tree](MASTER-TREE.md) and the [decision ledger](DIRECTION.md).
- Expand each branch recursively as decisions require: purpose, reference, alternatives, mechanics, dependencies, player experience, risks, innovation, validation and open questions.
- Label owner-confirmed decisions Established; tentative owner or assistant ideas Exploratory; intended later features Future; unanswered choices Undecided. Record discarded/superseded ideas with rationale when applicable.
- Keep examples visibly illustrative. Never convert brainstorming or assistant recommendations into confirmed canon.
- Maintain one canonical location for each decision, cross-link dependent branches, and preserve stable branch IDs.
- When the owner changes a decision, update the ledger and affected branch docs; record date and implications. Preserve unresolved alternatives rather than prematurely narrowing.
- Discussion order is flexible; the master tree has six suggested phases, not a release schedule.
- Keep separate project design from any other Roblox project; no imported assumptions from ORBIT!, OMDB or other concepts.
- Current owner-prioritized discussion: Branch III, four foundational classes, reusable class template, and individual advancement trees before hybrid branches. See [class architecture](CLASSES.md). Return to Branch I and other dependencies as needed.
- No gameplay code or implementation has been approved by this notebook.

- Latest owner priority: explore [shared combat and equipment foundations](COMBAT-FOUNDATIONS.md) before fleshing out individual class kits; return to class architecture afterwards.

- Owner accessibility principle: preserve depth without requiring players to understand every subsystem. Detailed UX/onboarding later. Overall progression direction in [PROGRESSION.md](PROGRESSION.md) approved; detailed implementation and tuning remain open.


## Current discussion priority (2026-11-26)
Owner requests closing previously explored/refinement topics before opening new itemization/economy/class-kit discussions. Owner considers attributes/stat list and equipment slots covered; do not repeat them. Treat numerical formulas, scaling and slot implementation details as later tuning rather than blocking design. Current closure proposals: elemental/status interaction rules, idle/auto-adventure, monetization guardrails, class promotion requirements. Await feedback before marking proposals confirmed.

- Latest refinement: owner clarified reaction order, cosmic stacking, no generic reaction cooldown, CC diminishing returns/recovery, reduced capped offline rewards without equipment, and repeat dungeon farming loop. Remaining conceptual closure: monetization and promotion requirements, plus any unresolved status stacking/consumption decisions if owner wants to settle now. Do not reopen attribute or equipment slot discussions.
