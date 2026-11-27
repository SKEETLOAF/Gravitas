# Cleric — foundation kit

Status: owner delegated the remaining four foundations for design. This is the assistant's complete working kit proposal, not individually approved or playtested. Canonical architecture: ../CLASSES.md, ../SKILLS-AND-COLLECTION.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../ELEMENTS.md, ../WEAPONS.md and ../DESIGN-LESSONS.md.

## Profile and progression
Prestige 0. Support; Tome primary, Shield secondary (working compatibility). HP C, Energy C, ATK F, MATK B, DEF C, MDEF B (18 allotment). Proficient: Energy Recovery, Cooldown Reduction, Effect Duration, Critical Resistance.
Standard foundation acquisition, individual Class Mastery, shared lineage progression and Class Trait Ascension; no extra gate or currency proposed. One guaranteed Legendary Core at acquisition; exact starter skill unlock sequence and summon pools open. Skill XP levels slots; individual skills retain star/tier investment; naturally higher rarity is intrinsically stronger at comparable development, subject to build synergy. Ordinary loadout: one Core and three active skills; existing selectable class passive and Trait remain separate from five passive skills. Five passive-skill slots per loadout still provisional. No ultimate.

## Identity
Adaptable direct restoration, protective support and credible solo magical offense. Cleric responds to immediate ally needs, rather than Oracle's future conditional blessings, Exorcist's enemy suppression, Paladin's frontline protection or Sage's dedicated allied spell amplification. Healing uses MATK; shield scales according to skill; no new Healing Power stat.

## Class Trait
Divine Favor: ordinary healing that restores actual missing Health primes the next damaging ordinary active with extra Light damage, while completing a damaging Core chain primes the next healing ordinary active with increased MATK-based healing. Two bounded nonstacking readiness flags (proposed); no infinite alternation from procs, overheal alone does not generate healing-side empowerment. Solo healing works on self; no damage target required to cast restorative spell. Trait upgrades improve payoff. Light damage/status applies only when explicitly tagged; ordinary restoration does not apply Radiance to enemies.

## Selectable class passives (2)
- Caretaker: baseline Energy Recovery and increased healing on allies (including self) below a Health threshold; avoids wasting all healing throughput on full-Health targets.
- Lightbearer: baseline MATK bonus; completing a Core chain briefly improves next damaging active's Light damage if it has Light tag, otherwise baseline MATK still helps. Bounded refresh/consumption.

## Legendary Core skills (2)
| Skill | Acquisition | Weapon | Behavior |
| --- | --- | --- | --- |
| Luminous Verse | Guaranteed | Either | MATK-based Light basic chain; finisher applies Radiance to enemy using existing Light status rules and restores a small amount of missing Health to self or lowest-health-ratio eligible ally in range (one recipient, self fallback). Shield uses existing strike animation with magical hit VFX. |
| Sacred Refrain | Alternative | Either | MATK-based neutral magical basic chain, with finisher granting a small personal or lowest-health ally shield. More protective but lower direct damage; no automatic Light status. Both cores deal damage and preserve solo play. |
Core modifiers layer onto universal weapon-family basic animations. No free weapon switching resets, no new attack sequence solely for each class; exact animation variants and timing open.

## Ordinary active skills (10)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Heal | Either | Direct MATK-based heal to selected eligible ally, automatic lowest Health ratio if no manual selection; self fallback. |
| Normal | Smite | Either | Direct Light magic attack applies Radiance; straightforward solo damage. |
| Normal | Protect | Shield | Skill-scaled shield on self or selected ally, increasing Block Chance as defined by skill while shield persists; auto prioritizes endangered ally. |
| Normal | Renew | Either | MATK-based regeneration on selected ally or self; bounded duration, same-source refresh. |
| Rare | Healing Circle | Tome | Restores Health to eligible nearby allies over several pulses, including self. Aggregate party healing and repeated pulses bounded. |
| Rare | Purify | Either | Removes eligible harmful status from selected ally or self and heals a modest amount; baseline heal if nothing to cleanse. Does not bypass scripted encounter requirements. |
| Rare | Radiant Spear | Either | Concentrated Light strike with partial area impact and Radiance; stronger damage than Smite at comparable development. |
| Rare | Sanctuary | Either | Temporary protective area centered on selected combat zone or caster, providing Resistance and small periodic healing; no forced movement, self included. |
| Legendary | Merciful Light | Tome | Strong targeted heal then a limited pulse to other injured allies; if alone, useful single-target healing with no extra self-bounces. Prioritizes urgent injuries; bounded overflow handling. |
| Legendary | Judgment | Either | Powerful Light attack followed by healing of nearby injured allies proportional to a bounded portion of actual direct damage dealt (MATK-based minimum). Applies Radiance to enemy. No healing recursion or overheal conversion without explicit passive. |
Either means either class-compatible weapon, not unrestricted use of all weapon families. All skill Energy costs, cooldowns, coefficients, effect caps and animation timing open. Ordinary Impulse, recovery, Armor, stat and element rules apply.

## Class-specific passive skills (5)
- **Overflowing Grace:** A portion of overhealing from direct ordinary healing skills becomes a shield, capped relative to MATK and recipient Health; passive shields cannot create another overheal event.
- **Radiant Communion:** Smite sacrifices some direct damage to heal the lowest-health eligible ally or self on hit; no independent copy of Smite, healing procs cannot re-trigger Communion.
- **Sheltering Word:** Protect additionally grants temporary Critical Resistance but trades away part of shield strength; defensive specialization for crit-heavy encounters.
- **Shared Prayer:** Renew can spread once to another injured ally at reduced potency; if none, first recipient gains a modest duration extension instead. No recursive spread.
- **Grace Under Fire:** When Cleric's direct healing restores substantial missing Health on a low-Health ally, next damaging Core finisher or ordinary damaging active grants a small bounded Energy refund once; internal cooldown, no overheal trigger.

## Shared lineage starter pool (9)
Four Normal active skills:
| Skill | Weapon | Function |
| --- | --- | --- |
| First Aid | Either | Small direct MATK-based heal on ally or self. |
| Light Bolt | Either | Low-cost Light damage, modest Radiance application per status rules. |
| Ward | Either | Small skill-scaled personal shield. |
| Encourage | Either | Brief modest ATK/MATK bonus on self or selected ally; no automatic stacking per party size. |

Five starter passive skills:
- **Devotion:** Increases MATK.
- **Spiritual Reserves:** Increases Energy Recovery.
- **Steady Faith:** After casting a direct heal, briefly gain Critical Resistance.
- **Helping Hand:** First direct heal on a low-Health recipient in a short window gains a modest bonus; self eligible.
- **Bright Response:** After removing an eligible harmful status, next ordinary damaging skill deals modest bonus damage; expires and consumes once.

Starter availability and passive/Core inheritance details remain open; compatible learned ordinary actives inherit under established lineage/hybrid rules. All passive names/effects are working design. No passive can duplicate itself through specialization or swapping without an explicit approved stacking rule.

## Example builds and automation
- **Healer:** Luminous Verse + Heal + Healing Circle + Merciful Light; Caretaker. Overflowing Grace and Helping Hand optional.
- **Protector:** Sacred Refrain + Protect + Purify + Sanctuary; Caretaker. Sheltering Word and Bright Response.
- **Battle Cleric:** Luminous Verse + Smite + Radiant Spear + Judgment; Lightbearer. Radiant Communion and Grace Under Fire support solo or party offense.
These are loadout ideas, not mandatory optimal builds. Use existing generic macro/auto executor: valid target, approach, Core chain, ordinary skill extension, recovery, cooldown and Energy. Respect combat-zone overrides. Conditional use can improve performance but skill baseline must function in a simple ordered rotation. No new editor or tactical AI required.

## Balance, implementation and synergy review
Healing target selection must be deterministic, avoid pets/invalid targets by default, never waste long-CD heal on full-health allies if an injured target is eligible (baseline macro fallback remains simple). Support and solo autos should not stall on unusable targets. Separate actual restoration from overheal, shield creation, Light status and damage conversion. Bounded damage-to-heal scaling, party target caps, no double-counted shared healing, independent cooldown ownership. Test solo boss, group with no incoming damage, low-Health ally, shielded targets, dispel immunity, co-op contribution credit and class swaps. Preserve Light/Dark/Force reactions rather than assuming Radiance heals by itself.
All temporary effects must specify source, target, active-class eligibility, expiry, cap and event ownership at implementation; persistent applied effects follow existing swap rules. Test common equipment/secondary weapons, inherited ordinary skills and same-class specialization. No raw coefficients, star caps, cooldowns, exact unlock schedule, new statuses or additional resource systems finalized here.
