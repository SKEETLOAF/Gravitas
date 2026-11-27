# Talent trees

Status: owner revises talent architecture (2026-11-27): a distinct talent tree for every individual class, single-purchase nodes, two paths within each class tree, multiple selectable universal trees with additional content opening at later promotions/Character Level, a base selection bonus for each tree, and an initial TP budget allowing roughly three complete base trees. Exact layout, bonus effects and selection limits below are proposals, not approved numbers.

## Point economy
- Keep independent earned lineage TP budgets, retained across sequential class changes; hybrids own separate tier-equivalent starting budget plus normal earning. One TP per eligible level gained; no point for resetting to level 1. Working example: initial unlock at level 10, 60 cap, 50 TP from gains 11–60 (unlock grants no extra point). Owner's desired approximate three base trees fits 16 paid nodes each, 48 TP total and 2 remaining. No multipurchase ranks.
- Proposed 16 native-cost nodes per base tree: two paths of eight nodes; tree selection bonus granted separately on equipping the tree. Nodes are individually bought once; branch prerequisites and cross-links open. Base costs 1 TP per universal or native tree node proposed; previous cross-tree costs 2/3 TP and native investment gate 40 are pending reconciliation with smaller individual class trees.
- Recommended starting capacity of three selected trees per class talent preset, with entry bonus only for selected trees, not every unlocked catalog entry. This is a proposal to prevent free bonus hoarding, not an owner-confirmed slot cap. Node investment and selection retain preset-specific allocation; no in-combat swapping. Whether selected tree slots grow later remains open. If more than three trees may be selected, require meaningful entry investment or other bonus limit.
- No new talent currency. Existing 100% primary/50% secondary/150% specialized talent contributions need numerical effect-strength interpretation for binary nodes. Overlapping effects, qualitative transforms, root bonuses and external bonus order remain open.

## Class trees
Each actual class gets its own tree upon acquisition, not just an extra section in one of five lineage trees. Examples: Warrior (Fortitude/Martial Mastery), Berserker (Frenzy/Reckless Might), Knight (Guardian/Counteroffensive), Ranger (Precision/Skirmishing), Hunter (Predator/Trapping), Gunslinger (Firepower/Gunplay); names are illustrative. Applies to every foundation, promotion, hybrid and special class. Each tree's entry bonus reinforces class identity without replacing its Trait or collectible passives. Base selection does not itself grant a class or skill.
- Prior class-tree purchases and earned TP remain retained across prestige. Recommend acquired ancestral trees remain available to descendants at native cost; actual eligibility for other learned class trees, hybrid parents/ancestor trees, and the previous 40 native-TP gate need review. A 40-TP requirement in one 16-node foundation tree is impossible without later expansions, so do not implement the old gate as written. Cross-class access and costs are unresolved, not abolished.
- Earlier five shared lineage starter node files in talents/ are superseded layout references. Extract suitable effects for individual class and universal trees; do not implement earlier three-path, multi-rank, 50-TP-per-section proposals. New distinct tree designs not finalized.

## Universal tree catalog
Proposal: several reusable standalone two-path trees, offered to all eligible classes. Each has a distinct entry bonus and base node budget. Initial candidates:
| Tree | Entry bonus direction | Paths |
| --- | --- | --- |
| Foundation | HP and defenses | Vitality / Resilience |
| Warfare | ATK/MATK appropriate to eligible damage | Core offense / Active offense |
| Tempo | Attack Speed or cooldown efficiency | Attack cadence / Skill cadence |
| Flow | Energy economy | Recovery / Efficiency |
| Endurance | Recovery and sustain | Health recovery / Mitigation |
| Opportunity | Accuracy and critical performance | Precision / Exploitation |
Exact starting catalog/count, names, bonus values and branch nodes proposed, not approved. Later promotions/Character Level open additional universal trees and/or expansion nodes in existing trees; unlock access permanently rather than requiring repeated shared system unlocks. Which progression milestone, new trees versus expansions, availability to lagging class tracks and future selection capacity open. General-purpose effects do not require a specific class Trait.

## Hybrid budget and migration
Earlier 200 preallocated + 30 free TP illustration was for a rejected large shared-tree layout and must not be carried over. At example talent unlock level 10, cumulative ordinary entering P III budget = (60-10)+(80-1)+(100-1)=228 TP, before any separate grant. Hybrid owns that tier-equivalent budget under existing working rule; its own class tree plus compatible parent trees and universal trees are proposed available choices. Exact starter allocation, selection capacity, access/costs, and whether parent-tree starters are prefilled require fresh design. Do not assume all 228 points can be spent on the same three unexpanded base trees.

## Reference and design lessons
Go Go Muffin community guides show class tree plus general tree combinations, two paths, and later additional talent disks: https://boarhat.gg/games/go-go-muffin/class/ranger/ ; https://mobi.gg/en/tips/go-go-muffin-build/ ; https://boarhat.gg/games/go-go-muffin/guide/cc5-guide/ . Adapt selection bonuses per owner direction; exact GGM root bonus values not independently verified. Keep the three existing Attribute/Conditional/Transformative categories, tagged compatibility, modest incremental effects, no recursive procs, no skill acquisition via talent nodes. No implementation or balancing validation yet.
