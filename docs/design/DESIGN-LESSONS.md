# Gravitas — design learning notes

Purpose: preserve reusable lessons from critique, comparison, design iteration and eventual playtesting. This is a living synthesis, not a chronological changelog or replacement for canonical specifications. Keep entries concise; distinguish observed owner preferences, design hypotheses and validated results. Consolidate repeated lessons as they evolve. Git history preserves discarded drafts.

## Class and skill design

### Passive skills should change play, not merely inflate numbers
Owner-preferred direction, learned during Warrior design (2026-11-27).
- Individual Class Traits establish a discipline's defining loop. Collectible passive skills supply conditional effects, triggered abilities and skill transformations that create build choices. Talent nodes provide incremental development and deeper specialization; they may also transform mechanics where appropriate.
- A passive can change an active skill's function with a real trade-off (Warrior Warmonger transforms Battle Cry from tanking to aggression). Avoid making every passive mandatory for the same build.
- Starter lineage passives can be simpler; mix accessible stat bonuses with meaningful combat interactions. Preserve useful inherited options across descendants with different playstyles.
- Higher starting skill rarity retains intrinsic power advantages; build synergy can let an evolved lower-origin skill outperform it situationally. Keep rarity meaningful without making all investment obsolete.

### Design around existing combat events
Working design principles from Warrior iteration:
- Use existing Block/Super Block, prevented damage, Armor break, basic-chain completion/extension, Impulse, weapon/class switches, Energy and status effects as hooks. Avoid adding new resource meters by default.
- Distinguish block count from damage actually prevented by Block. Exclude unrelated mitigation; normalize conversions to appropriate player scaling and bound proc output. Avoid recursive counter/shockwave triggers, duplicated damage-conversion exploits and runaway Energy loops.
- Give defensive skills and passives reasonable baseline value in ordinary automation. A counter should still act if no incoming hit arrives during its stance; tank passives should not go dead in single-target bosses; Armor-break builds need deliberate value during Broken windows and appropriate handling of unarmored enemies.
- Differentiate mechanically similar skills rather than piling overlapping triggers on the same mandatory rotation.
- Keep optional active play rewarding without requiring manual parry timing for baseline class functionality.

### Review future kits through these questions
Does the class have a distinct loop? Do passives enable different builds and interact with real combat mechanics? Is an inherited skill useful outside its original class? Does auto-combat handle its conditions reliably? Are there sensible boss, single-target, multi-target and unarmored use cases? Are stronger rarity skills rewarding? What happens at extreme stat values and when effects overlap? These are review prompts, not mandatory new mechanics.

### Lessons from designing the remaining foundation kits
Assistant-derived working design hypotheses, not playtest conclusions (2026-11-27):
- Separate a class's loop from its descendants' specialties: Ranger direct precision vs Hunter prey/traps; Mage spell cadence vs Elementalist reaction manipulation; Assassin burst openings vs Shinobi deception and Blade Dancer sustained combos; Cleric immediate restoration vs Oracle conditional blessings and Sage amplification.
- Two Core skills should change attack rhythm and payoff while reusing weapon-family animation foundations. Don't imply new range, weapon compatibility or elemental tags solely from skill names/VFX.
- Build skill transformations with explicit trade-offs (area versus focus, upfront versus delayed damage, shield size versus Critical Resistance). Let baseline skills operate without required passive combinations.
- Design valid fallback targets and baseline effects for solo/party, armored/unarmored, resistant, short-lived and single-target enemies. A heal needs a valid recipient, an evasive build needs some opportunity even while a tank holds Aggro, and chained attacks cannot self-bounce indefinitely.
- Keep effect ownership explicit: direct hits versus secondary/proc hits, actual damage versus overkill, actual healing versus overheal, cooldown/charge ownership, bounded conversions and per-action normalization. No recursive mark, echo, healing or Energy loops.
- Treat unconfirmed status implementations (e.g., Bleed) as dependencies; do not promote them into established universal rules by drafting a skill.
- All five foundations now have complete candidate pools and example builds. Review intersections before numerical tuning: active/inactive passive scope, duplicate skills, slot levels across presets, cross-class weapon compatibility and lineage inheritance, then talent interactions. No new system or resource required merely to establish identity.

## Reference leads for further verification
Prior design discussions identified Go Go Muffin's Swordbearer skill transformations and retaliation, Sword x Staff's Charms and trigger-dependent effects, Last Epoch's skill-specific trade-offs, Torchlight: Infinite's skill support interactions and Diablo IV's weapon-switch incentives. Use these as research leads, not proof of exact named effects or values; verify current primary/community documentation before relying on specific mechanics. Adapt principles to Gravitas, not exact kits. See REFERENCES.md for the wider reference index.

## Comparative attribute review (2026-11-27)
Research sources: Go Go Muffin community beginner guide, stat breakdown (https://boarhat.gg/games/go-go-muffin/guide/beginner-guide/); Sword x Staff compiled in-game stat descriptions and keywords (https://www.gacha.gg/sword-x-staff/mechanics); Sword x Staff community build guides (https://www.prydwen.gg/sword-x-staff/guides/build-guide-dominator and https://www.prydwen.gg/sword-x-staff/guides/build-guide-duelist).
GGM uses general ATK for damage/healing, DEF, ASPD/Haste, Crit, Determination (chance-based defense bypass or healing amplification), Mastery, Accuracy/Evasion, Block and mitigation stats. SxS uses ATK/DEF/HP/SPD, Resilience against ailments, Crit/Block and counters, Effect Hit/RES, broad damage/heal modifiers and element/target-specific modifiers. Community documentation, not independent gameplay validation.
Design assessment (assistant recommendation, not new canon): retain Gravitas's 29-attribute roster for now. Separate physical/magical scaling, explicit Break Power and Energy economy, Super Crit/Block and action-linked effects differentiate our real-time hybrid combat. Avoid adding universal damage multipliers or per-element permanent character attributes merely because references have them; use targeted skill/equipment/talent effects.
Open balance priorities:
- Specify Accuracy vs Evasion/Block resolution so Accuracy does not cheaply erase both defenses; define crit/block coexistence and mitigation order, overflow and anti-counter limits.
- Specify Effect Potency vs Resistance (application chance, magnitude and/or duration) and Effect Duration's distinct purpose, avoiding double-counted scaling or permanent CC.
- Attack Speed vs Cooldown Reduction vs Energy economy: distinguish animation/channel/recovery and cooldown effects; preserve readable combat and sustainable rates without exponential loops.
- ATK/MATK and DEF/MDEF: test mixed-build stat dilution, shield magical/physical behavior, split damage, hybrid scaling and healing eligibility for criticals/other modifiers. No assumption that heals can crit yet.
- Check low-value rolls and mandatory stat thresholds, especially Break Power on unarmored enemies, Aggro in solo, Resistance against status-free opponents, and farming stats versus combat stats. Give optional content-specific usefulness rather than force every stat equally useful everywhere.
- Validate 18-point grade profiles by simulations and representative encounters, not equal allotment alone; consider actual coefficients, damage mitigation, hit rate, Energy, threat and role value. No numerical changes approved.

## Talent design lessons (working hypotheses)
- A shared tree should support lineage descendants and compatible hybrid/cross-tree builds through mechanical tags, not named class-exclusive Traits. Preserve progression investment as classes evolve.
- Use modest, linear rank effects, including measurable changes to geometry, falloff, damage distribution, effect duration, and resource economy. Collectible passives can make larger skill transformations; avoid duplicating them as full effects from a single rank.
- Cost a starter section explicitly before setting hybrid acquisition budgets. Proposed 50 ranks per section gives 200 preallocated ranks across two parent trees' first two sections; the approximately 30 free TP estimate fits a plausible early unlock but is not a reason to force an unlock level.
- Review gates against earned TP and effective-rank multipliers, distinguish native rank cost from effective rank, and avoid mandatory full-tree completion at each progression step. Defer deeper sections until future class kits and their dependencies are understood.
- Starter node draft coverage: 5 trees, 2 sections each, 24 nodes/tree, 120 total nodes. Not a numerical balance test. See TALENTS.md.

## Talent topology revision
Owner prefers more distinct single-purchase nodes instead of repeatedly leveling each talent 3–5 times, inspired by Go Go Muffin. General and class-specialized pools with two paths per class pool are proposed. Design lesson: distinguish frequent progression choices from repetitive rank spending; preserve build breadth, avoid filler, and re-evaluate class-slot multipliers when node ownership becomes binary. Verified community reference: https://mobi.gg/en/tips/go-go-muffin-build/ (two branches per tree) and https://boarhat.gg/games/go-go-muffin/guide/beginner-guide/ (level-linked talents and resettable allocations). Prior numerical starter layout is not current canon.

## Selectable talent tree revision
Owner prefers a distinct tree for every actual class, several universal trees unlocking/expanding with progression, two class paths and a base bonus for choosing a tree. Aim for approximately three complete base trees with 50 TP by P0 level 60 if unlocked at 10. Proposed 16 paid nodes per tree provides 48 TP spend and two spare. Review selection caps to prevent free entry-bonus hoarding. A previous 40-point investment gate cannot be satisfied inside a single 16-node base tree; reconcile gates, costs and hybrid allocations instead of blindly preserving incompatible rules. Reference verified: Boarhat Ranger guide shows Hawk Arrow plus Forging Foundation and Zealous Burden (https://boarhat.gg/games/go-go-muffin/class/ranger/), CC5 guide documents new elemental talent disks (https://boarhat.gg/games/go-go-muffin/guide/cc5-guide/). Earlier shared multi-rank tree drafts are reference-only; exact bonuses and selection capacity not yet approved.

## Evidence and validation
No implementation/playtest evidence yet. When testing begins, record reproducible observations, relevant build/version, what changed, and the resulting lesson; do not present design hypotheses as measured outcomes.
