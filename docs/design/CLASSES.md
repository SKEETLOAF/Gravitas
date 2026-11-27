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

## Proposed common class anatomy
- Class Trait: inherent identity mechanic, not summoned or occupying passive slots. Recommended active-class-only eligibility; explicitly persistent effects may survive swaps. No passive stacking across all learned classes. Candidate identities, not approved kits: Warrior blocking/retaliation under enemy pressure; Ranger ranged precision; Mage spell sequencing and elemental interactions; Rogue evasion and rapid attacks; Cleric healing/protection/support.
- Basic attacks depend on active class and weapon. Shared weapon animation/action templates may have class-specific variations.
- Proposed per-class loadout: four equippable active skills, one ultimate, two selectable passive skills, plus inherent Class Trait and basic attacks. Start with functional base kit; alternate skills through existing acquisition routes. Show only active class abilities on main HUD. Counts are reviewable, not confirmed.
- Active skills/ultimates use shared Energy system; individual cooldowns persist across swaps. Ultimate is a skill category, not a separate resource.
- Proposed passives are selectable build modifiers, distinct from inherent Class Trait and mastery talents. Prefer active-class eligibility unless a skill explicitly grants persistent effects. Acquisition and upgrade rules open; avoid adding new currency families.
- Class-specific branching talents and saved talent loadouts are owner-approved. Mastery-linked earned points, compact trees and respec are recommended; exact points, tree size, unlock thresholds, preset limits and editing rules open.
- Each weapon has one weapon skill (confirmed). Class skills may require a compatible family; weapon skill presentation and whether it occupies a separate slot are open. Basic attacks remain weapon/class dependent.
- Two class selections and two shared weapons; shared gear/companions remain unchanged, class skills independently selected. Duplicate class selection grants scaling specialization instead of a second kit, with possible cooldown reduction. Class swap cooldown 0.5 seconds. Canonical rules in [COMBAT-SWITCHING.md](COMBAT-SWITCHING.md).

## Reusable class design template (proposal)
Use the same template for foundations, advanced, hybrid and special classes. Fill only established details; mark others TBD. Do not impose universal skill counts, resources or unique mechanics until the foundations are tested.

1. **Identity:** name, category, parent(s), fantasy, role(s), distinctive playstyle, status.
2. **Acquisition and progression:** prerequisites, unlock path, mastery, branch eligibility, progression retention, alternative paths.
3. **Class benefit:** defining mechanical advantage, activation condition, scope (active-only, equipped, mastery reward, or temporary retained effect), trade-offs and intended value solo/co-op. Do not assume permanent stacking.
4. **Weapons:** primary type, compatible alternatives, shared compatibility, weapon-specific interactions, proficiencies.
5. **Combat foundation:** attack chains, movement, offense, defense, range, resource/gauge if needed, signature loop.
6. **Kit:** inherent passive, active abilities, optional ultimate, weapon techniques versus class techniques, skill modifiers, cooldown ownership. Number and structure TBD.
7. **Automation:** default behavior, target and skill priorities, swap conditions, ability timing, active intervention opportunities, future manual compatibility.
8. **Synergies:** same-class kit, weapon overlaps, non-overlapping functional combos, swap-in/out effects, cross-class resources/buffs/cooldowns.
9. **Growth:** talents, mastery milestones, advanced branches, new techniques, horizontal options; later hybrid prerequisites.
10. **Balance and experience:** strengths, weaknesses, solo viability, team contribution, farm/boss performance, comparisons, guardrails. Explicitly identify what makes this class distinct from parents, siblings and hybrids, and what reason remains to use its parent after unlocking it.
11. **Presentation and implementation:** silhouettes, animation, VFX/audio, UI indicators, required assets, dependencies, test cases.
12. **Decision record:** established, exploratory, future, undecided, discarded; next questions.

## Open class architecture
- Inherent benefit activation: active-only, equipped, mastery reward or intentionally retained effect; no automatic stacking of every learned discipline.
- Review proposed loadout counts, passive/talent acquisition, class/weapon ability ownership, swapping and cooldowns. See [COMBAT-SWITCHING.md](COMBAT-SWITCHING.md).
- Distinct benefits and viability of earlier classes after promotions, skill inheritance, class-specific mechanics, automation and active options.
- Exact foundation and promotion kits, hybrid roster, special acquisition rules. No actual class skills or named promotion roster established.
