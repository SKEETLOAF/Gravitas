# Ranger — foundation kit

Status: owner delegated the remaining four foundations for design. This is the assistant's complete working kit proposal, not individually approved or playtested. Canonical architecture: ../CLASSES.md, ../SKILLS-AND-COLLECTION.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../ELEMENTS.md, ../WEAPONS.md and ../DESIGN-LESSONS.md.

## Profile and progression
Prestige 0. Ranged DPS; Bow primary, Dagger secondary. HP D, Energy B, ATK A, MATK D, DEF D, MDEF C (18 allotment). Proficient: Accuracy, Penetration, Critical Damage, Attack Speed.
Standard foundation acquisition, individual Class Mastery, shared lineage progression and Class Trait Ascension; no extra gate or currency proposed. One guaranteed Legendary Core at acquisition; exact starter skill unlock sequence and summon pools open. Skill XP levels slots; individual skills retain star/tier investment; naturally higher rarity is intrinsically stronger at comparable development, subject to build synergy. Ordinary loadout: one Core and three active skills; existing selectable class passive and Trait remain separate from five passive skills. Five passive-skill slots per loadout still provisional. No ultimate.

## Identity
Versatile precision combat: sustain accurate hits on a chosen enemy, exploit the opening with a concentrated attack, then reposition or continue pressure. Ranger is the dependable direct projectile specialist, not Hunter's trap/prey manipulation, Gunslinger's firearm arsenal, or Arcane Archer's magical projectile behavior.

## Class Trait
Deadeye: landed direct Core attacks build Precision against the current target, to a bounded maximum. Next damaging ordinary active against that target consumes accumulated Precision to increase Accuracy and Critical Damage for that activation (crit chance still resolves normally; Accuracy bonus affects eligible hits). Precision is built on confirmed landed hits, not crits, so it remains useful against high Critical Resistance. Change target loses/decays target-specific progress; target death clears it, short grace for unavoidable switches proposed. Trait upgrades increase payoff. Cap progress per Core attack action, not every projectile. No new mandatory meter.

## Selectable class passives (2)
- Sharpshooter: baseline Accuracy bonus; additional Penetration against distant targets, using normalized distance within the attack's usable range; melee/close range retains baseline value.
- Skirmisher: after a skill-driven reposition or weapon/class transition into Ranger, briefly increase Attack Speed and Movement Speed; bounded refresh, not a stacking swap exploit.

## Legendary Core skills (2)
| Skill | Acquisition | Weapon | Behavior |
| --- | --- | --- | --- |
| Trueflight | Guaranteed | Either | Balanced Core chain. Consecutive attacks against the same target increase Accuracy, and finishing hit deals additional physical damage. Bow uses arrows; Dagger uses close strikes. Does not auto-convert dagger to bow range. |
| Crosswind | Alternative | Either | Faster Core sequence with reduced per-hit impact; finisher strikes one additional nearby target with reduced damage or delivers a second smaller hit when alone. Each sequence grants a short Movement Speed bonus. Direct hits only build Trait at normalized rate. |
Core modifiers layer onto universal weapon-family basic animations. No free weapon switching resets, no new attack sequence solely for each class; exact animation variants and timing open.

## Ordinary active skills (10)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Piercing Shot | Bow | Arrow penetrates along a line, dealing reduced damage to subsequent enemies; remains strong against the first target. |
| Normal | Quickdraw | Dagger | Quick advancing slash; bridges a displaced enemy or close target into melee chain. |
| Normal | Steady Aim | Either | Brief Accuracy and Critical Damage buff; can be activated during regular rotation without a rooted manual aiming requirement. |
| Normal | Disengage | Either | Short backward evasive movement and a parting hit; improves Evasion briefly. Uses permitted combat geometry, never overrides encounter-zone selection. |
| Rare | Arrow Rain | Bow | Repeated physical volleys into a selected enemy group; smaller concentrated footprint against isolated foes. |
| Rare | Split Second | Dagger | Two rapid strikes with the second benefiting from a successful first hit, then a short retreat; uses normal hit resolution. |
| Rare | Pinning Shot | Bow | Powerful shot applies Slow to susceptible enemies and bonus Armor depletion against intact Armor; baseline damage against control-resistant targets. |
| Rare | Expose Weakness | Either | Strike applies a short, bounded physical-defense debuff; does not require a crit or armor break, allowing party follow-up. |
| Legendary | Deadshot | Bow | Deliberate high-impact shot with intrinsic Penetration; each completed Core chain since previous use strengthens its shot up to a cap. Does not require maximum Trait stacks to act. |
| Legendary | Close Quarters | Dagger | Rapid close-range sequence followed by a retreating thrown dagger finisher; damage and Evasion payoff scale modestly with direct attacks landed during activation. |
Either means either class-compatible weapon, not unrestricted use of all weapon families. All skill Energy costs, cooldowns, coefficients, effect caps and animation timing open. Ordinary Impulse, recovery, Armor, stat and element rules apply.

## Class-specific passive skills (5)
- **Guiding Wind:** After a missed direct attack, briefly improve Accuracy for the next direct attack, consuming on attempt; misses never generate Precision.
- **Fletched Fury:** Arrow Rain trades wide coverage for a concentrated barrage on one enemy; fewer simultaneous targets, greater focused damage. Retains meaningful baseline effect when only one target exists.
- **Needlepoint:** Piercing Shot loses secondary-target penetration but gains increased first-target Penetration and Armor depletion; alternate build, not a mandatory upgrade.
- **Moving Target:** After a permitted reposition, the next Core attack gains bonus damage and Accuracy; no reward for repeated invalid movement, ordinary idle pursuit or stutter movement.
- **Opening Volley:** First direct attack against a newly Broken enemy triggers an additional physical projectile with a per-target cooldown; cannot trigger itself. Useful even when an ally breaks Armor.

## Shared lineage starter pool (9)
Four Normal active skills:
| Skill | Weapon | Function |
| --- | --- | --- |
| Quick Shot | Either | Fast direct physical attack with normal weapon range. |
| Fan Strike | Either | Short area attack with low Energy cost; Bow spread shot, Dagger arc. |
| Focus | Either | Temporary Accuracy increase; simpler than Steady Aim. |
| Flank | Either | Short permitted approach/reposition followed by a direct attack; no forced move outside combat zone. |

Five starter passive skills:
- **Eagle Eye:** Increases Accuracy.
- **Keen Edge:** Increases Critical Damage.
- **Rapid Recovery:** Completing a Core chain briefly increases Energy Recovery.
- **Pursuit:** First hit after an enemy is displaced deals additional damage; capped per target.
- **Measured Shot:** First damaging active after a complete Core chain gains modest Penetration.

Starter availability and passive/Core inheritance details remain open; compatible learned ordinary actives inherit under established lineage/hybrid rules. All passive names/effects are working design. No passive can duplicate itself through specialization or swapping without an explicit approved stacking rule.

## Example builds and automation
- **Precision:** Trueflight + Steady Aim + Expose Weakness + Deadshot; Sharpshooter. Needlepoint if replacing a skill with Piercing Shot.
- **Volley:** Crosswind + Arrow Rain + Piercing Shot + Pinning Shot; Sharpshooter. Use Fletched Fury only for concentrated encounters.
- **Skirmisher:** Crosswind + Quickdraw + Disengage + Close Quarters; Skirmisher. Moving Target supports real repositioning.
These are loadout ideas, not mandatory optimal builds. Use existing generic macro/auto executor: valid target, approach, Core chain, ordinary skill extension, recovery, cooldown and Energy. Respect combat-zone overrides. Conditional use can improve performance but skill baseline must function in a simple ordered rotation. No new editor or tactical AI required.

## Balance, implementation and synergy review
Distance bonuses must respect dagger range and automated positioning; don't require constant kiting to function. Avoid per-projectile proc inflation, permanent debuff stacking, or macro exploit via rapid switching. Deadshot preparation cannot stall casting indefinitely. No universal hit guarantee or forced critical. Visualize aim/Precision through subtle target cue and shot cadence; no new mandatory UI bar. Bow/dagger variants use existing animation families and separate skill animations. Test single boss, grouped enemies, high Evasion, Armor, target death and forced zone changes.
All temporary effects must specify source, target, active-class eligibility, expiry, cap and event ownership at implementation; persistent applied effects follow existing swap rules. Test common equipment/secondary weapons, inherited ordinary skills and same-class specialization. No raw coefficients, star caps, cooldowns, exact unlock schedule, new statuses or additional resource systems finalized here.
