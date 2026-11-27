# Class architecture and design template
Updated 2026-11-26. Overall class expansion established; exact lineage structure and kits open.

## Established direction
- One character can learn, independently develop and equip multiple distinct disciplines. Promotions unlock new disciplines without replacing prior classes or losing mastery. Sibling branches can remain accessible. Every class must have a distinct benefit, even relative to its ancestors.
- Classes have linked primary/secondary weapons; see [WEAPONS.md](WEAPONS.md). Shared weapons encourage synergy without requiring every compatible class pair to share a weapon (recommended).
- Hybrid classes may unlock through multiple developed disciplines, including advanced branches. Warrior + Cleric -> Paladin is an illustrative owner example, not a roster commitment. Warrior -> Berserker is an illustrative advancement.
- Independent special classes may be obtained via dungeons, events, battle passes or game passes; sources remain candidates. Earnable equivalent power and ordinary progression without payment remain guardrails.
- Character/class progression and promotion requirements are established in [PROGRESSION.md](PROGRESSION.md). Energy and shared combat rules are in [COMBAT-FOUNDATIONS.md](COMBAT-FOUNDATIONS.md).

## Working foundation model
Five proposed role lineages, inspired by Go Go Muffin. This is the current design basis, not final promotion structure.
| Foundation | Role | Primary | Secondary |
| --- | --- | --- | --- |
| Warrior | Tank | Sword | Shield |
| Ranger | Ranged DPS | Bow | Dagger |
| Mage | Magical DPS | Magic Staff | Tome |
| Rogue | Melee DPS | Dagger | Sword |
| Cleric | Support | Tome | Shield (recommended) |
Exact weapon confirmation status in WEAPONS.md. Whether promotions are sequential or branch, promotion counts/names, inheritance and special/hybrid acquisition remain open. All classes should be solo-capable (recommended); roles are specialties, not restrictions.

## Common class anatomy
- Class Trait: exactly one inherent passive trait per class, unlocked and upgraded through Class Mastery and shared Ascension items. Not summoned or equipped in a selectable passive slot. Same-class specialization does not duplicate the trait. Exact mastery thresholds, level caps, costs, effects and activation across class swaps remain open; active-class-only eligibility is recommended. Candidate identities (not approved kits): Warrior retaliation, Ranger precision, Mage spell sequencing, Rogue exploiting openings, Cleric divine favor.
- Basic attacks depend on active class and weapon. Shared weapon animation/action templates may have class-specific variations.
- Confirmed per-class loadout: four equipped active skills, one ultimate, one passive selected from two available class passives, plus basic attacks. Once class swapping is unlocked, selecting the same class twice grants both passives without duplicating the active or ultimate kit. Functional base kit and alternate skill acquisition retained. Class Trait is an established separate passive progression track.
- Active skills/ultimates use shared Energy system; individual cooldowns persist across swaps. Ultimate is a skill category, not a separate resource.
- Selectable class passives are distinct from inherent Class Traits and mastery talents. Each class offers two, normally equips one; same-class specialization unlocks both. Whether equipped passives remain active during other-class use, acquisition and upgrade rules remain open.
- Branching talents and saved talent loadouts are owner-approved. Owner approved five base trees shared across foundational lineages, with Go Go Muffin and Diablo-style inspiration.
- Each weapon has one weapon skill (confirmed). Class skills may require a compatible family; weapon skill presentation and whether it occupies a separate slot are open. Basic attacks remain weapon/class dependent.
- Two class selections and two shared weapons; shared gear/companions remain unchanged, class skills independently selected. Duplicate class selection grants scaling specialization instead of a second kit, with possible cooldown reduction. Class swap cooldown 0.5 seconds. Canonical rules in [COMBAT-SWITCHING.md](COMBAT-SWITCHING.md).

## Shared lineage talents (approved direction)
One reusable tree for each of five foundational lineages (Warrior, Ranger, Mage, Rogue, Cleric). All descendants access their lineage's tree, while Class Traits, two selectable passives and individual skill kits provide class-specific identity. Each talent node has 3–5 upgradeable ranks (owner-approved); exact rank count and scaling depend on the node. Recommended one point per rank, with prerequisite ranks or branch-investment gates where useful rather than mandatory maxing of all preceding nodes. Three approved node categories: Attribute (increase existing attributes), Conditional (trigger benefits under combat conditions), and Transformative (modify compatible skill/mechanic behavior). Use reusable mechanical tags (Block, Break, healing, DoT, Energy, etc.) so nodes apply across promotions rather than requiring separate trees. Skill acquisition remains separate from talents through the established base-kit/progression/summon system. Do not add talent-exclusive skills by default. Exceptional unlocks, if ever needed, require separate review. Transformative modifiers may change elements, targeting, area or skill behavior; avoid duplicating ordinary Skill XP/star development. Trees may expand with future promotions, using permanent lineage milestones to unlock later sections; an unlocked descendant must not force a new tree or reset. Promotion-exclusive effects should generally live in its trait/skills/passives, not duplicate talent branches.
- Point economy proposal for review: Character Level grants a universal talent-point capacity reusable independently in each saved allocation (not a consumable pool split between classes). Class Mastery and permanent lineage promotion milestones unlock deeper nodes/sections. Occasional promotion point awards are optional, not the primary source; avoid duplicate point farming through descendants. Alternative mastery-derived capacity remains open. No separate lineage XP grind. Exact rates, caps and gates undecided.
- Saved allocations/presets can be selected for different builds or individual classes within the same tree; reuse unlocked points/nodes without paying again. Respec and preset capacity open; no in-combat talent editing recommended.
- Swap-effect proposal: each equipped class selects an eligible saved talent allocation with the full earned capacity. Only the active class's allocation applies: Attribute nodes recalculate active stats, Conditional nodes can trigger while active, and Transformative nodes modify eligible actions from that allocation. Explicitly persistent effects already applied retain intended durations; no new outgoing talent triggers while inactive by default. Same-lineage classes can select different presets without stacking allocations; same-class specialization uses one allocation. Preserve shared Health/Energy without free replenishment, cooldowns and ongoing effects; exact max-stat transition handling open. Hybrid access, scope exceptions and activation policy still need owner approval.
- Future hybrid/special classes: recommend access to existing eligible lineage trees rather than creating new trees by default. Hybrid may select one parent tree initially, or mix compatible branches under one bounded budget if desired later; exact eligibility open. No additional independent hybrid talent grind assumed.
- Illustrative branches only: Warrior protection/retaliation/break; Ranger precision/sustained attacks/mobility; Mage elemental interactions/spell power/Energy efficiency; Rogue criticals/evasion/rapid attacks; Cleric restoration/shielding/enhancement.
- Reference distinction: Go Go Muffin separates skill acquisition (including Class Change summon pools) from level-linked, resettable talents that grant stats and modify current skills. Diablo IV's April 2026 rework emphasizes branching active skill modifications, including changes to element, area and range; passive nodes were removed from its skill tree. Use GGM's separation and consider Diablo's transformative upgrades, not its whole skill acquisition model. Verified references in REFERENCES.md.

## Reusable class design template (proposal)
Use the same template for foundations, advanced, hybrid and special classes. Fill only established details; mark others TBD. Use the confirmed loadout capacities and universal Energy; unique mechanics are class-specific.

1. **Identity:** name, category, parent(s), fantasy, role(s), distinctive playstyle, status.
2. **Acquisition and progression:** prerequisites, unlock path, mastery, branch eligibility, progression retention, alternative paths.
3. **Class Trait:** one inherent upgradeable passive; define mastery and Ascension item requirements, level effects, activation scope, trade-offs and intended solo/co-op value. Do not assume permanent stacking.
4. **Weapons:** primary type, compatible alternatives, shared compatibility, weapon-specific interactions, proficiencies.
5. **Combat foundation:** attack chains, movement, offense, defense, range, resource/gauge if needed, signature loop.
6. **Kit:** inherent passive, active abilities, optional ultimate, weapon techniques versus class techniques, skill modifiers, cooldown ownership. Use confirmed four active / one ultimate / one of two passives; both passives when specializing.
7. **Automation:** easy-to-author default macro/preset, reusable actions and class-specific sequence options, Impulse and swap opportunities, future manual compatibility.
8. **Synergies:** same-class kit, weapon overlaps, non-overlapping functional combos, swap-in/out effects, cross-class resources/buffs/cooldowns.
9. **Growth:** shared lineage talent synergies, mastery milestones, advanced branches, new techniques, horizontal options; later hybrid prerequisites. Do not design a separate tree by default.
10. **Balance and experience:** strengths, weaknesses, solo viability, team contribution, farm/boss performance, comparisons, guardrails. Explicitly identify what makes this class distinct from parents, siblings and hybrids, and what reason remains to use its parent after unlocking it.
11. **Presentation and implementation:** silhouettes, animation, VFX/audio, UI indicators, required assets, dependencies, test cases.
12. **Decision record:** established, exploratory, future, undecided, discarded; next questions.

## Open class architecture
The shared architecture is ready for initial kit design. Before tuning, resolve whether selected passives persist across class swaps, how weapon skills are accessed and whether both weapons contribute stats, and how talent and trait effects apply. Suggested defaults for review: both equipped classes' selected passives remain eligible (subject to their own triggers), only the active class's trait and selected lineage talent effects are eligible unless explicitly persistent, each equipped weapon skill has a dedicated slot and requires its own weapon to execute, shared gear stats persist. Weapon attribute contribution is not yet decided. No final class kit or promotion roster approved.
- Trait level thresholds, ascension costs, upgrade effects and activation scope; no automatic stacking of all learned disciplines.
- Passive activation/acquisition and talent details, class/weapon ability ownership, detailed swap execution and cooldowns. See [COMBAT-SWITCHING.md](COMBAT-SWITCHING.md).
- Distinct benefits and viability of earlier classes after promotions, skill inheritance, class-specific mechanics, automation and active options.
- Exact foundation and promotion kits, hybrid roster, special acquisition rules. No actual class skills or named promotion roster established.
