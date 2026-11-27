# Shared lineage talent trees

Status: starter tree structure and node designs are assistant proposals for owner review. Existing approved principles remain canonical in CLASSES.md and PROGRESSION.md until this draft is approved. No exact stat coefficients or playtest results.

## Established rules
- Five shared native lineage trees; descendants retain access. All five eventually accessible. Ordinary native rank costs 1 TP, other tree ranks 2 TP after 40 invested native TP. Hybrid parents immediately accessible at 1 TP/rank; non-parent ranks 3 TP after 40 combined invested parent TP.
- One TP per eligible lineage level gained after talent unlock, preserved across prestige; no point on resetting to level 1. Independent track budgets; hybrids have tier-equivalent one-time starting allotment plus normal level earning.
- Attribute, Conditional and Transformative nodes, 3–5 investable ranks, modest linear effective-rank increments. No ordinary skill acquisition through talents. Primary effective ranks 100%, secondary 50% (minimum 1 for invested node), specialization 150% of single primary allocation; overlapping nodes add effective ranks. No arbitrary investment-cap clamp on effective ranks; explicit effect safety caps separate.
- Class Trait, selectable class passives and collectible passive skills retain separate identities. No changes to skill eligibility, skill-slot levels, stars or tiers.

## Proposed structure
One tree per lineage, with three thematic paths continuing through prestige sections. Sections 1 (Foundation) and 2 (Prestige I) each have 12 nodes and 50 investment ranks: paths A and B each 5/5/4/3 ranks (17 TP), path C 5/4/4/3 (16 TP). Every tree totals 24 nodes and 100 native ranks across the two drafted sections; five trees total 120 nodes and 500 ranks.
Proposed lightweight gates: first two nodes of each path open once section is available; third requires 5 invested ranks in the same path/section, fourth requires 10. Gates count paid ranks, not effective/bonus ranks. Prior section need not be maxed to unlock next. Section access by permanent progression milestones; exact destination-tree unlock rules for cross-tree allocations, hybrid deeper-section access and respec enforcement remain open. Recommend shared early-section gates based on the allocating track's tier so cross-tree builds remain practical; owner review required.
Cost is 50 TP per section only at native/parent rates; ordinary non-native section 100 TP, hybrid non-parent section 150 TP. No mandatory new capstone mechanic or class-exclusive tree.
Later P II and P III sections: reserve for actual promotion-kit design. Size and rank budgets open. Keep enough total choices to maintain meaningful trade-offs rather than assuming every tree can be maxed each prestige. The first two sections are not the entire tree.

## Five starter tree designs
| Tree | Paths | Detailed node file |
| --- | --- | --- |
| Warrior | Fortitude / Martial Mastery / Battle Instinct | [Warrior](talents/WARRIOR.md) |
| Ranger | Marksmanship / Barrage / Mobility | [Ranger](talents/RANGER.md) |
| Mage | Arcane Mastery / Elemental Control / Spellcraft | [Mage](talents/MAGE.md) |
| Assassin | Precision / Evasion / Exploitation | [Assassin](talents/ASSASSIN.md) |
| Cleric | Restoration / Protection / Benediction | [Cleric](talents/CLERIC.md) |

## Hybrid starting budget illustration
Owner wants hybrids to start with P III-equivalent TP, possibly the first two sections of both parent trees maxed and around 30 unspent TP, accounting deferred until tree costs known. With this proposed layout, preallocation costs 2 parents x 2 sections x 50 ranks = 200 TP. Example talent unlock at P0 level 8, award only subsequent level gains: P0 60-8=52; P I 80-1=79; P II 100-1=99. Cumulative earned on entering P III = 230; leaves 30 TP after 200 preallocated. If unlock at level 5 instead, budget 233 and free 33. Unlock timing/award convention and exact starter grant remain open; do not force level 8 to meet an estimate. A hybrid starts level 1, cap 120, gains 119 more TP across normal level-ups if all eligible. At the example 230 starting allotment, maximum 349 TP. This is independent from actual parent balances and does not require taking their points.
Recommendation for review: grant one tier-equivalent budget, provide a default allocation maxing both parents' first two sections; let the remaining TP be freely allocated. Preallocated ranks should count toward 40 combined parent-tree gate; don't create a second free rank grant. Respec permanence/locking of starter ranks and gate behavior not approved. If actual section costs or unlock level change, recompute before finalizing.

## Numerical and implementation review
- Node IDs stable within draft, each effect has a measurable rank increment and explicit eligibility, scope, units and cap to be specified later. A Transformative node should modify an existing behavior fractionally, not grant a whole new action at rank 1. Same-rank stat nodes across sections are intentional incremental growth, not new attributes.
- Use skill tags and existing events, not specific class Trait requirements. Distinguish direct action, secondary/proc, actual damage, actual healing, armor and status application. No recursive triggers. Geometry and target caps, legal encounter zones, cooldown and Energy loop safeguards.
- Review whether conditional stat nodes remain useful in solo, boss, party and multi-target encounters; test potential duplication with collectible passive skills and cross-tree rank-1 breadth incentives. No assumption of tested balance.
- Exact numerical increments, unlocking milestones, respec, bonus rank ordering, node dependencies and future sections are open.
