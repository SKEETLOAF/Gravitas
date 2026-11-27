# Mage — foundation kit

Status: owner delegated the remaining four foundations for design. This is the assistant's complete working kit proposal, not individually approved or playtested. Canonical architecture: ../CLASSES.md, ../SKILLS-AND-COLLECTION.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../ELEMENTS.md, ../WEAPONS.md and ../DESIGN-LESSONS.md.

## Profile and progression
Prestige 0. Magical DPS; Magic Staff primary, Tome secondary. HP D, Energy A, ATK F, MATK A, DEF D, MDEF C (18 allotment). Proficient: Effect Potency, Effect Duration, Energy Efficiency, Cooldown Reduction.
Standard foundation acquisition, individual Class Mastery, shared lineage progression and Class Trait Ascension; no extra gate or currency proposed. One guaranteed Legendary Core at acquisition; exact starter skill unlock sequence and summon pools open. Skill XP levels slots; individual skills retain star/tier investment; naturally higher rarity is intrinsically stronger at comparable development, subject to build synergy. Ordinary loadout: one Core and three active skills; existing selectable class passive and Trait remain separate from five passive skills. Five passive-skill slots per loadout still provisional. No ultimate.

## Identity
Flexible spellcasting: weave Core attacks between ordinary spells, conserve Energy, and exploit magical damage and elemental effects. Mage has strong baseline spells and sequencing without requiring reactions. Elementalist later specializes in reaction manipulation, Warlock in accumulated afflictions and detonation, Spellblade in melee infusion, Sage in allied amplification.

## Class Trait
Spellweaver: completing a Core chain primes a bounded empowerment for the next ordinary damaging spell: bonus MATK-based damage and reduced Energy cost. Additional completed chains improve the payoff to a cap; consumed once per activation rather than each hit. Trait upgrades improve efficiency and damage. Support/defensive casts do not consume the damage empowerment. No free recasts or new universal resource; exact stack lifetime and consumption order open.

## Selectable class passives (2)
- Arcane Conduit: baseline Energy Efficiency; additional Energy Recovery after completing a Core chain, refreshed rather than stacked.
- Spellcraft: baseline Effect Potency; stronger bonus for damaging spells against multiple targets or an elite/boss. Avoid duplicating Elementalist's future reaction-specific identity.

## Legendary Core skills (2)
| Skill | Acquisition | Weapon | Behavior |
| --- | --- | --- | --- |
| Arcane Sequence | Guaranteed | Either | Balanced MATK-based magical basic chain. Finisher restores a small amount of Energy and emits a small secondary arcane hit; neutral magic has no implied element or reaction. |
| Ember Script | Alternative | Either | Slower magical Core chain with Fire-tagged finisher applying Burn; finisher grants bounded bonus damage when striking an already burning target. Reuses Staff/Tome sequences with Fire VFX. |
Core modifiers layer onto universal weapon-family basic animations. No free weapon switching resets, no new attack sequence solely for each class; exact animation variants and timing open.

## Ordinary active skills (10)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Firebolt | Either | Direct Fire spell applies Burn; inexpensive single-target pressure. |
| Normal | Frost Lance | Either | Cold projectile applies Chill; bonus Armor pressure if control cannot apply, not a guaranteed Freeze. |
| Normal | Stone Ward | Either | Earth-themed personal shield scaled by MATK or a skill-defined coefficient; when shield expires naturally or is depleted, releases a small Earth impact applying Fracture to nearby enemies once. No free recasts. |
| Normal | Arcane Pulse | Either | Neutral magical area blast with reliable damage and Impulse; no status application. |
| Rare | Chain Lightning | Either | Lightning bolt chains to nearby targets applying Shock; when alone, first hit retains strong baseline damage rather than infinite self-bounces. |
| Rare | Tidal Surge | Either | Water wave applies Soaked and displaces susceptible enemies; against intact Armor, offers bounded Armor damage instead of forced knockback. |
| Rare | Echo Burst | Either | Resonance burst applies Reverberation and creates a delayed second impact at original target area; does not require a reaction. |
| Rare | Arcane Reservoir | Tome | Restores a bounded amount of Energy over a short period and grants temporary Energy Efficiency; costs Energy to cast, cannot repeatedly refund itself or refresh for net exponential gains. |
| Legendary | Meteor | Staff | High-impact Fire/Earth-themed meteor; choose Fire as baseline element (Burn), Earth visuals do not silently apply Fracture. Landing causes large magical area damage, then a short residual Fire field; telegraphed delay. |
| Legendary | Astral Cascade | Either | A neutral magical barrage of successive impacts concentrated on the main enemy with partial area damage; each distinct Core-chain extension since last cast strengthens final impact up to a cap. No cosmic status simply because of name. |
Either means either class-compatible weapon, not unrestricted use of all weapon families. All skill Energy costs, cooldowns, coefficients, effect caps and animation timing open. Ordinary Impulse, recovery, Armor, stat and element rules apply.

## Class-specific passive skills (5)
- **Afterimage Script:** After completing a Core chain, next damaging spell leaves a delayed reduced-power echo; once per completed chain, no recursion, no duplicate status by default.
- **Glacial Geometry:** Frost Lance trades its narrow direct projectile for a wider Cold cone, lower single-target damage but applies Chill to more enemies; allows a crowd-control build without forcing reactions.
- **Overchannel:** Meteor spends additional Energy when enough is available for a stronger impact; otherwise casts baseline Meteor. Extra cost cannot produce free cooldown/energy loops.
- **Mnemonic Ward:** When Stone Ward is depleted by damage, reduce remaining cooldown of one eligible damaging spell by a bounded amount; natural expiration does not trigger refund.
- **Conservation:** Using three distinct ordinary spell IDs without repeating one grants reduced Energy cost to the next spell; clears on trigger, cannot count Core attacks or echoed casts.

## Shared lineage starter pool (9)
Four Normal active skills:
| Skill | Weapon | Function |
| --- | --- | --- |
| Magic Missile | Either | Neutral low-cost magical projectile. |
| Kindle | Either | Small Fire hit applies Burn, lighter than Firebolt. |
| Mend Mana | Either | Small bounded Energy restoration over time, net gain limited by cooldown and cost. |
| Gust | Either | Resonance hit with minor displacement if eligible; simple ranged-control tool. |

Five starter passive skills:
- **Arcane Studies:** Increases MATK.
- **Deep Reserves:** Increases maximum Energy.
- **Efficient Casting:** First ordinary spell after a full Core chain costs slightly less Energy.
- **Lingering Magic:** Damaging elemental skills modestly extend existing statuses applied by that activation; no unlimited duration refresh.
- **Residual Pulse:** First damaging spell against a Broken target releases a small neutral magical impact, bounded per target.

Starter availability and passive/Core inheritance details remain open; compatible learned ordinary actives inherit under established lineage/hybrid rules. All passive names/effects are working design. No passive can duplicate itself through specialization or swapping without an explicit approved stacking rule.

## Example builds and automation
- **Elemental generalist:** Ember Script + Tidal Surge + Frost Lance + Chain Lightning; Spellcraft. Sequence available primer/reactor pairs without requiring every action to react.
- **Arcane artillery:** Arcane Sequence + Meteor + Arcane Pulse + Astral Cascade; Arcane Conduit. Overchannel optional for high-Energy build.
- **Control and endurance:** Arcane Sequence + Stone Ward + Echo Burst + Arcane Reservoir; Arcane Conduit. Mnemonic Ward for defensive cooldown payoff.
These are loadout ideas, not mandatory optimal builds. Use existing generic macro/auto executor: valid target, approach, Core chain, ordinary skill extension, recovery, cooldown and Energy. Respect combat-zone overrides. Conditional use can improve performance but skill baseline must function in a simple ordered rotation. No new editor or tactical AI required.

## Balance, implementation and synergy review
Never silently treat all magic as an element; visual themes do not imply second status. Use existing primer ordering, coexistence, consumption, reaction and CC rules. Energy refund must net out appropriately and not recur via echoes or slot swaps. High CDR/efficiency and simultaneous echoes need guardrails. Staff/Tome compatibility intentionally mostly shared, two distinct weapon specialists plus universal spells. Test bosses immune to control, unarmored mobs, interrupted Meteor, low Energy, co-op reaction attribution and remote VFX budget.
All temporary effects must specify source, target, active-class eligibility, expiry, cap and event ownership at implementation; persistent applied effects follow existing swap rules. Test common equipment/secondary weapons, inherited ordinary skills and same-class specialization. No raw coefficients, star caps, cooldowns, exact unlock schedule, new statuses or additional resource systems finalized here.
