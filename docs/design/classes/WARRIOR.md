# Warrior — foundation kit (working proposal)

Status: full skill-pool proposal for owner review, not finalized mechanics. Established architecture and growth are in ../CLASSES.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../SKILLS-AND-COLLECTION.md and ../WEAPONS.md. Numerical coefficients, Energy costs, cooldowns, animation timings and acquisition beyond the guaranteed Core are open.

## Established profile
Prestige 0; Tank; Sword primary, Shield secondary. Main growth HP A, Energy D, ATK B, MATK F, DEF B, MDEF D (18 allotment). Soft proficiencies Block Chance, Aggro, Break Power, Resistance.

## Proposed identity
Adaptable frontline fighter converting enemy pressure into momentum; balanced offense, defense and Armor breaking. Distinct from Berserker aggression and Knight dedicated protection. Auto-friendly, solo-capable, useful in parties.

## Trait — Fighting Spirit
Successful blocks accumulate a bounded benefit for the next damaging ordinary active skill, increasing damage and Armor depletion. Super Blocks grant additional progress. Super Block is universal. No mandatory extra resource bar. Trait upgrades improve payoff. Stack limits, lifetime, consumption timing, coefficients, swap handling and upgrade milestones open.

## Selectable class passives (separate from passive skills)
- Vanguard: baseline Aggro and Block Chance bonus; amplified when engaging multiple enemies or an elite/boss.
- Undaunted: increased Break Power versus intact Armor; damage bonus versus Broken enemies.

## Legendary Core Skills (2; one equipped)
- Martial Discipline (guaranteed on class acquisition): balanced basic chain with increasing Armor damage and a strong finisher; completing the chain temporarily increases Block Chance.
- Unyielding Advance (alternative): heavier basic chain; successful blocks empower the next basic strike with additional damage and Aggro, partially based on damage prevented by Block.
Both proposed usable with Sword and Shield, using existing weapon-family animation framework; Core mechanics layer onto weapon-specific sequences. Exact weapon compatibility, free basic Energy rules, animation variants and recovery open.

## Ordinary active skills (10; three equipped)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Cleave | Sword | Sweeping multi-target slash |
| Normal | Shield Bash | Shield | Heavy Armor depletion and knockback against eligible targets |
| Normal | Battle Cry | Either | Increase Aggro and personal DEF/MDEF temporarily |
| Normal | Iron Guard | Shield | Temporary Block Chance and Resistance increase |
| Rare | Onslaught | Sword | Advancing multi-hit attack, pursues displaced enemies and extends combos |
| Rare | Rupture | Sword | Concentrated downward Armor-breaking strike |
| Rare | Rally | Either | Temporarily increase nearby allies' ATK and Break Power |
| Rare | Shield Toss | Shield | Ricocheting returning shield projectile, generates Aggro per hit |
| Legendary | Retaliation | Either | Brief defensive stance, then strong counterattack with additional physical damage and Armor depletion from damage prevented by Block during stance; baseline attack if unstruck |
| Legendary | Linebreaker | Either (proposed) | Charge through enemies, multiple strikes ending in area attack; temporary personal shield with baseline value plus bonus based on actual Armor depletion during attack |

Retaliation's damage conversion should use actual Block-attributable prevention, not raw incoming damage or historical blocks; cap relative to own attributes. Linebreaker's Armor conversion must also have bounded scaling. Iron Guard is a timed buff rather than a locked counter stance. All ordinary actives follow Energy, cooldown and Impulse rules. Armor prevents ordinary stagger/knockback while intact. Skill XP upgrades slots, individual stars and tiers belong to the learned skill. Higher starting rarity has intrinsic advantage even after lower rarity reaches Legendary status.

## Warrior-specific passive skills (5)
- Stalwart: successful blocks briefly increase Resistance; repeated blocks refresh rather than stack without limit.
- Reprisal: blocking accumulates a small portion of actual damage prevented as bonus damage on the next ordinary damaging active; bounded by ATK/DEF benchmark. Does not create a new attack or trigger itself. Review overlap with Fighting Spirit and Retaliation; alternative use as shield conversion if excessive.
- Second Wind: breaking enemy Armor restores a small amount of Energy; normalized/capped per activation or short window.
- Hold the Line: below a Health threshold, increased Block Chance and DEF; avoid threshold flicker via hysteresis or short duration.
- Follow Through: striking a Broken target increases subsequent basic attack damage for a short window, with bounded benefit.

## Shared Warrior-lineage starter skills (separate from class-specific pool)
Four Normal ordinary actives, available as lineage starter collection; precise free unlock schedule open.
| Skill | Weapon | Function |
| --- | --- | --- |
| Heavy Strike | Either | Direct powerful single-target physical attack |
| Brace | Either | Brief personal shield, skill-defined scaling |
| Shoulder Charge | Either | Short advancing strike, helps close distance and generate Aggro |
| Sweeping Blow | Either | Low-cost area attack, lower impact than dedicated Cleave; review overlap and replace if too redundant |
Five starter passive skills, shared by Warrior descendants and compatible hybrid users (eligibility proposal):
- Conditioning: increase HP.
- Arms Training: increase ATK.
- Fortitude: increase DEF.
- Combat Instinct: increase Break Power.
- Resolve: increase Resistance.
Exact effects, rank curves, acquisition and class/passive inheritance open.

## Example rotations (proposals)
Tank: Unyielding Advance + Battle Cry + Iron Guard + Retaliation; Vanguard.
Armor breaker: Martial Discipline + Rupture + Shield Bash + Linebreaker; Undaunted.
Frontline support: Martial Discipline + Rally + Battle Cry + Linebreaker; Vanguard.
Actual automatic scheduling must handle range, Energy, cooldown and recovery; favor conditional Retaliation before incoming pressure when practical without demanding manual timing. If conditional macro commands aren't available, Retaliation remains useful as ordinary baseline skill. Core/active/passive proc events should not recursively trigger one another or multiply the same prevented damage without explicit limits. Passive-skill slots per class vs character and trigger scope remain open, so no final passive loadout assumptions.

## Deferred concept — Last Bastion
Ultimates removed from current design by owner. Preserve Last Bastion as future concept only: empowered block/resistance state, independent automatic counters, concluding sweep. No current ultimate slot.

## Review
This is an assistant proposal, not owner-approved kit. User previously provided feedback on Fighting Spirit/Retaliation overlap, Vanguard's boss weakness, Undaunted after Armor break and universal Super Block. Review blocked-damage stacking, starter versus class skill differentiation, shield compatibility, class-specific Core inheritance, passive slot scope, exact numbers and animation budget before locking.