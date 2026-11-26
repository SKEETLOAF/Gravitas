# Class architecture and design template
Updated 2026-11-26. Owner decisions distinguished from exploratory design. No class kits are implemented.

## Owner direction
- Begin with four foundational classes. Warrior and Mage are locked. Rogue and Cleric are the owner's tentative third and fourth picks, with Cleric as a support-oriented discipline.
- Foundational classes branch into advanced disciplines; Warrior -> Berserker is the owner's example.
- Class expansion is established: unlocking a descendant adds a distinct, independently developable and equippable discipline; no parent is replaced or consumed. Players can progress every accessible class, including sibling branches, and return to previous styles with their progression retained. Class lineage represents a common concept and unlock ancestry, not a mandatory power hierarchy. Every foundational, advanced, hybrid or special class must have a distinct combat identity and benefit, even relative to its parents or descendants. Combos, synergies and future hybrid unlock paths may originate from any class or branch, not only foundations; exact combinations, unlock requirements and equipment compatibility are still design work. This does not promise that every pair yields a bespoke hybrid.
- Hybrid classes unlock through sufficient progression of multiple classes; Warrior + Cleric -> Paladin is the owner's example. Defer hybrid roster design until the main branches and class template are established.
- Every class should offer its own benefit. Exact benefit structure and whether it persists on swap are open.
- Special classes may exist independently of the core trees, unlocked via game passes, limited events/battle passes, or dungeons. These sources are possibilities, not finalized distribution or monetization rules.
- Classes have linked weapons. Secondary alternative weapons may bridge classes (Warrior sword primary, gauntlets secondary; illustrative Monk gauntlets primary). No shared weapon is required for class combination as a recommended principle, not a confirmed rule. Three classes and two weapons are tentative caps; scope of weapon cap remains open.

## Initial candidate families (not roster commitments)
Three contrasting branches per foundation are suggested for discussion; number, names, progression gates and later tiers remain open.

| Foundation | Candidate advancement | Distinct combat identity | Illustrative benefit |
| --- | --- | --- | --- |
| Warrior | Berserker | Relentless aggression and momentum | Offensive payoff for sustained pressure |
| Warrior | Knight | Guarding, interception and retaliation | Damage mitigation and counter opportunities |
| Warrior | Duelist | Disciplined single-target melee | Precision counters and exploiting openings |
| Mage | Elementalist | Elemental combinations and area attacks | Group damage and elemental reactions |
| Mage | Arcanist | Spell sequencing and controlled arcane power | Resource/skill efficiency and burst |
| Mage | Summoner | Conjured creatures or constructs as extensions of one character | Sustained pressure and battlefield control |
| Rogue | Assassin | Fast strikes against vulnerable targets | Burst and critical opportunities |
| Rogue | Ranger | Ranged weapon combat, positioning and pursuit | Sustained ranged pressure |
| Rogue | Trickster | Deception, traps and disruption | Control and tactical openings |
| Cleric | Priest | Healing and protective divine magic | Sustain and party recovery |
| Cleric | Inquisitor | Offensive holy techniques and judgment | Divine damage and enemy suppression |
| Cleric | Oracle | Blessings, wards and predictive support | Buff/debuff utility and mitigation |

Candidate foundations: Warrior physical pressure/stagger/resilience (sword primary example); Mage spell damage/area control (staff candidate); Rogue precision/mobility (daggers candidate); Cleric recovery/protection (primary weapon undecided). Every foundation should be solo-capable as a recommended principle given single-character gameplay; support need not mean low offense.

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

## Open benefit architecture
Class benefits might be active identity traits, equipped-class passives, mastery unlocks, or effects intentionally retained across switching. Avoid automatically stacking all permanent bonuses from every learned class. Examples: Warrior posture pressure, Mage spell interactions, Rogue vulnerability exploitation, Cleric sustain. These are candidates, not confirmed stats or formulas.

## Advancement questions
Resolved: class expansion, independent disciplines, retained progression and all accessible sibling branches. Open: whether descendants inherit any techniques or benefits, how prior mastery affects unlocking or initial development, exact branch requirements, and which combinations produce a hybrid. Do not assume inherited kits or automatic stat stacking. Avoid defining arbitrary levels and hybrid prerequisites before the core class structure is established.
 
## Special class guardrails (recommendations)
Independent unlock paths should support discovery and distinctive gameplay. If paid or limited access is adopted, avoid making a paid class the only solution to campaign/co-op progression or strictly stronger than earnable alternatives. Decide exclusivity, reruns, acquisition, power parity, and hybrid eligibility separately. No paid class or pricing is confirmed.

## Discussion sequence
1. Establish the four foundations and their individual benefit system.
2. Agree on the common class template, combat kit and weapon relationships.
3. Explore advanced branches family by family, beginning with Warrior.
4. Decide advancement progression and inheritance.
5. Explore hybrids and independent special classes afterwards.

## Alternative architecture under consideration (2026-11-26): promotion lineages
Owner is considering replacing the four foundational branching trees with five core role lineages and sequential, earned class promotions inspired by Go Go Muffin's Class Change system. Roles: Tank, Ranger/ranged DPS, Mage, Melee DPS, Support. Exact class names and whether the five-role model supersedes the four-family model remain pending. Suggested example lineages (not canon): Warrior -> Knight -> Vanguard -> Warlord; Ranger -> Hunter -> Marksman -> Deadeye; Mage -> Sorcerer -> Arcanist -> Archmage; Rogue -> Assassin -> Shadow -> Phantom; Cleric -> Priest -> Oracle -> Saint. Promotions could require mastery and/or milestone objectives or trials, with no fixed levels established. Unusual classes could be independent special unlocks; whether hybrid classes become special unlocks or are removed remains open. Recommend retaining previously established class expansion, multi-class learning and loadout swapping, including access to earlier promoted styles, unless owner explicitly changes those rules. Important open distinction: promotion unlocks an independently equippable style, or advances one class with configurable earlier styles; effect on swap slots and cooldown ownership is unresolved. Prior branching design remains available for comparison, not silently superseded.

Reference: Go Go Muffin uses successive Class Changes with new skills and talents; see https://www.pocketgamer.com/go-go-muffin/best-builds/?page=2 and https://twinfinite.net/guides/go-go-muffin-class-guide/ . These inform promotion structure only, not wholesale adoption.

## Foundational weapon mapping (2026-11-26)
See [WEAPONS.md](WEAPONS.md) for the owner-planned roster and current primary/secondary assignments: Warrior Sword/Shield, Ranger Bow/Dagger, Mage Magic Staff/Tome (owner specified), Rogue Dagger/Sword, Cleric Tome/Shield (Tome owner specified, Shield retained as recommendation). This mapping supersedes earlier weapon examples for the proposed five-role foundations; it does not confirm promotion names or the five-lineage architecture itself.
