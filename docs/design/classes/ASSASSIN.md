# Assassin — foundation kit

Status: owner delegated the remaining four foundations for design. This is the assistant's complete working kit proposal, not individually approved or playtested. Canonical architecture: ../CLASSES.md, ../SKILLS-AND-COLLECTION.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../ELEMENTS.md, ../WEAPONS.md and ../DESIGN-LESSONS.md.

## Profile and progression
Prestige 0. Melee DPS; Dagger primary, Sword secondary. HP C, Energy B, ATK A, MATK F, DEF D, MDEF C (18 allotment). Proficient: Evasion, Critical Chance, Effect Duration, Attack Speed.
Standard foundation acquisition, individual Class Mastery, shared lineage progression and Class Trait Ascension; no extra gate or currency proposed. One guaranteed Legendary Core at acquisition; exact starter skill unlock sequence and summon pools open. Skill XP levels slots; individual skills retain star/tier investment; naturally higher rarity is intrinsically stronger at comparable development, subject to build synergy. Ordinary loadout: one Core and three active skills; existing selectable class passive and Trait remain separate from five passive skills. Five passive-skill slots per loadout still provisional. No ultimate.

## Identity
Exploit short combat openings: evade or identify a vulnerable target, deliver precise burst, then re-enter the ordinary chain. Assassin specializes in concentrated direct damage rather than Shinobi's deceptive tools/afterimages, Blade Dancer's long sustained combos, or Trickster's unusual projectile trajectories. No mandatory stealth meter or positional backstab requirement in semi-idle play.

## Class Trait
Exploit: successful evasion while Assassin is active or hitting an already staggered/Broken enemy with a direct Core attack primes a bounded bonus Critical Chance and damage for the next damaging ordinary active. Normalize to once per eligible event/action with short internal gate; target vulnerability alone cannot trigger infinite stacking. Evasion grants stronger progress if desired. Trait upgrades improve payoff; ordinary critical rules and Super Crit remain unchanged. No guaranteed crits from this Trait.

## Selectable class passives (2)
- Predator: baseline Critical Chance; bonus direct single-target damage against an enemy below a Health threshold. No automatic kill/execution bypass.
- Elusive: baseline Evasion; a successful evasion briefly increases Movement Speed and Attack Speed, with bounded refresh. No reward for attacks that never targeted the Assassin.

## Legendary Core skills (2)
| Skill | Acquisition | Weapon | Behavior |
| --- | --- | --- | --- |
| Surgical Strike | Guaranteed | Either | Quick precise basic chain, with finishing hit gaining increased Critical Chance. Finisher prioritizes current target, no automatic teleport behind target. |
| Razor's Rhythm | Alternative | Either | Faster light sequence, finishing hit applies Bleed (ordinary physical DoT candidate) with weaker direct impact; follow-up Core hits on a bleeding target grant a small Energy recovery once per chain. If Bleed is not implemented, substitute direct finisher damage pending status review. |
Core modifiers layer onto universal weapon-family basic animations. No free weapon switching resets, no new attack sequence solely for each class; exact animation variants and timing open.

## Ordinary active skills (10)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Lunge | Either | Fast approach and thrust; follows displaced target within allowed range. |
| Normal | Cutthroat | Dagger | Quick single-target physical stab with bonus Critical Chance; no instant kill. |
| Normal | Evasive Step | Either | Short permitted sidestep with Evasion bonus and follow-up strike. Does not override encounter zones or guarantee avoidance. |
| Normal | Hamstring | Either | Low-cost cut applies Slow against susceptible targets; baseline damage against resistant foes. |
| Rare | Twin Fang | Dagger | Two targeted thrusts; if first crits, second gains bonus damage (still rolls its own critical result). |
| Rare | Crescent Slash | Sword | Broad arc with strong physical damage, useful when surrounded; no forced spin or infinite CC. |
| Rare | Rend | Either | Heavy cut applies Bleed and deals additional direct damage against staggered/Broken enemies; non-Bleed baseline retained. |
| Rare | Feint | Either | Attack followed by brief Evasion increase; if evading during the window, next Core strike gains increased damage. No free extra attack while inactive. |
| Legendary | Deathmark | Either | Precise strike marks one target; subsequent direct attacks by this Assassin contribute a capped amount of actual damage to a delayed physical burst. Baseline strike; if the target dies before detonation, discard the remaining stored damage (no corpse detonation or transfer). No recursive stored damage. Mark is skill-specific, not universal Hunter resource. |
| Legendary | Severance | Either | Powerful single-target sequence ending in high-impact strike; additional damage if target is already Broken or below a Health threshold, with a useful base attack outside either condition. |
Either means either class-compatible weapon, not unrestricted use of all weapon families. All skill Energy costs, cooldowns, coefficients, effect caps and animation timing open. Ordinary Impulse, recovery, Armor, stat and element rules apply.

## Class-specific passive skills (5)
- **Read the Opening:** Successful evasion grants a brief buff making next damaging ordinary active gain Penetration; separate from Exploit's crit/damage effect, expires and consumes once.
- **Bloodletting:** Rend trades some upfront damage for increased Bleed duration and potency; if Bleed unavailable defer rather than silently add an element.
- **Vanishing Step:** Evasive Step trades its immediate follow-up damage for a stronger Evasion window; first successful evasion during that window automatically triggers a reduced counterstrike (one per activation). Not stealth or afterimage.
- **Critical Tempo:** After a direct critical hit, next Core attack has increased Attack Speed; no stacking per multihit or proc damage. Normalize at high crit rates.
- **Finishing Touch:** Deathmark detonates earlier after a limited number of direct Core attacks, with reduced maximum stored damage but increased immediate payoff on short encounters; no extra activation.

## Shared lineage starter pool (9)
Four Normal active skills:
| Skill | Weapon | Function |
| --- | --- | --- |
| Quick Cut | Either | Low-cost single-target melee damage. |
| Sidestep | Either | Short permitted evasive movement with brief Evasion bonus; no attack. |
| Crosscut | Either | Two short-range cuts with modest damage. |
| Puncture | Either | Concentrated attack with modest Penetration. |

Five starter passive skills:
- **Agility:** Increases Evasion.
- **Killing Instinct:** Increases Critical Chance.
- **Opener:** First direct hit against a fresh target gains modest damage; per-target gate.
- **Light Footwork:** After a successful evasion, briefly gain Movement Speed.
- **Clean Finish:** Defeating an enemy with a direct active restores a bounded amount of Energy; elite/boss encounter has a modest reward on first Armor break instead, no double reward.

Starter availability and passive/Core inheritance details remain open; compatible learned ordinary actives inherit under established lineage/hybrid rules. All passive names/effects are working design. No passive can duplicate itself through specialization or swapping without an explicit approved stacking rule.

## Example builds and automation
- **Executioner:** Surgical Strike + Cutthroat + Twin Fang + Deathmark; Predator. Critical Tempo and Finishing Touch optional.
- **Counterstriker:** Surgical Strike + Evasive Step + Feint + Severance; Elusive. Vanishing Step and Read the Opening reinforce evasion.
- **Bleed pressure:** Razor's Rhythm + Rend + Hamstring + Lunge; Predator. Bloodletting if Bleed confirmed.
These are loadout ideas, not mandatory optimal builds. Use existing generic macro/auto executor: valid target, approach, Core chain, ordinary skill extension, recovery, cooldown and Energy. Respect combat-zone overrides. Conditional use can improve performance but skill baseline must function in a simple ordered rotation. No new editor or tactical AI required.

## Balance, implementation and synergy review
Avoid pretending attacks are dodged when no incoming attack actually targets player. No positional assumptions behind enemies, no forced movement across arena constraints. Deathmark stores only eligible direct dealt damage, not procs, reflected, DoT, other players or its own burst; clear stored damage on target death and prevent double reward. Preserve crit/crit resistance tiers and Armor control immunity. Bleed is an existing candidate, not yet finalized; exact mechanics pending. Test boss threat on tank, no-evasion scenario, unarmored enemies, short-lived mobs, capped crit, target death and inherited skills.
All temporary effects must specify source, target, active-class eligibility, expiry, cap and event ownership at implementation; persistent applied effects follow existing swap rules. Test common equipment/secondary weapons, inherited ordinary skills and same-class specialization. No raw coefficients, star caps, cooldowns, exact unlock schedule, new statuses or additional resource systems finalized here.

## Legendary weapon compatibility (owner direction)
Both Legendary Core choices and both native Legendary ordinary actives work with either class-compatible weapon. Use appropriate weapon or spell choreography without changing the skill's essential role, cooldown identity or creating a hidden equipment requirement. Skill range follows its authored behavior and valid combat geometry. Separate dedicated weapon skills remain weapon-specific; lower starting rarity ordinary skills retain existing restrictions pending further direction. No change to normal class/skill acquisition or inheritance eligibility. Numerical and animation parity still require testing.
