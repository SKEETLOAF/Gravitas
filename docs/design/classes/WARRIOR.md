# Warrior — foundation kit (working proposal)

Status: owner favors the full kit and revised passive direction; passive working roster accepted, exact mechanics and numbers not finalized. Established architecture and growth are in ../CLASSES.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md, ../SKILLS-AND-COLLECTION.md and ../WEAPONS.md. Numerical coefficients, Energy costs, cooldowns, animation timings and acquisition beyond the guaranteed Core are open.

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

## Warrior-specific passive skills (5; owner-approved working direction)
- Reprisal: blocks can trigger an automatic counterstrike, partially scaling with damage prevented; internal cooldown.
- Warmonger: transforms Battle Cry, replacing defensive/Aggro benefits with ATK and Attack Speed; offensive Impulses during the empowered state deal physical damage.
- Tempered Resolve: converts a portion of damage prevented through blocking into a personal shield; increases Resistance while shielded.
- Relentless Assault: basic-chain extensions via active skills reduce Energy cost of the next active; consecutive extensions strengthen the benefit up to a cap.
- Shatterpoint: Armor break releases a damaging shockwave with Armor depletion against nearby enemies and a temporary physical damage vulnerability on the original Broken target.

Review event recursion, proc frequency, blocked-damage conversion budgets, source attribution, vulnerability stacking, status-duration floors and basic-chain-extension resource loops. No guaranteed recursive Shatterpoint chain reaction. Exact values, rarity, trigger scope and inheritance open.

## Shared Warrior-lineage starter skills (separate from class-specific pool)
Four Normal ordinary actives, available as lineage starter collection; precise free unlock schedule open.
| Skill | Weapon | Function |
| --- | --- | --- |
| Heavy Strike | Either | Direct powerful single-target physical attack |
| Brace | Either | Brief personal shield, skill-defined scaling |
| Shoulder Charge | Either | Short advancing strike, helps close distance and generate Aggro |
| Sweeping Blow | Either | Low-cost area attack, lower impact than dedicated Cleave; review overlap and replace if too redundant |
Five starter passive skills (owner-approved working direction), shared by Warrior descendants and compatible hybrid users (eligibility proposal):
- Conditioning: increases maximum HP.
- Arms Training: increases ATK.
- Combat Rhythm: completing a basic attack chain restores Energy.
- Steadfast: successful blocks shorten remaining harmful status durations.
- Opportunist: bonus damage against staggered or Broken targets.

Exact effects, rank curves, acquisition and class/passive inheritance open.

## Design lessons
The owner prefers the revised passive pool over primarily stat-oriented or redundant conditional passives. See [design learning notes](../DESIGN-LESSONS.md) for reusable principles and research leads. Previous candidates remain in Git history rather than in the current kit.

## Example rotations (proposals)
Tank: Unyielding Advance + Battle Cry + Iron Guard + Retaliation; Vanguard.
Armor breaker: Martial Discipline + Rupture + Shield Bash + Linebreaker; Undaunted.
Frontline support: Martial Discipline + Rally + Battle Cry + Linebreaker; Vanguard.
Actual automatic scheduling must handle range, Energy, cooldown and recovery; favor conditional Retaliation before incoming pressure when practical without demanding manual timing. If conditional macro commands aren't available, Retaliation remains useful as ordinary baseline skill. Core/active/passive proc events should not recursively trigger one another or multiply the same prevented damage without explicit limits. Passive-skill slots per class vs character and trigger scope remain open, so no final passive loadout assumptions.

## Deferred concept — Last Bastion
Ultimates removed from current design by owner. Preserve Last Bastion as future concept only: empowered block/resistance state, independent automatic counters, concluding sweep. No current ultimate slot.

## Review
This is the working kit with owner-preferred revised passives, not a numerically finalized kit. User previously provided feedback on Fighting Spirit/Retaliation overlap, Vanguard's boss weakness, Undaunted after Armor break and universal Super Block. Review blocked-damage stacking, starter versus class skill differentiation, shield compatibility, class-specific Core inheritance, passive slot scope, exact numbers and animation budget before locking.