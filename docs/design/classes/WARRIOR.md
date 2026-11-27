# Warrior — foundation kit (working proposal)

Status: design draft, not owner-approved skill mechanics. Established architecture and growth are in ../CLASSES.md, ../COMBAT-FOUNDATIONS.md, ../COMBAT-SWITCHING.md and ../WEAPONS.md. No numerical coefficients, cooldowns, Energy costs or animations finalized.

## Established profile
Prestige 0; Tank; Sword primary, Shield secondary. Main growth HP A, Energy D, ATK B, MATK F, DEF B, MDEF D (18 allotment). Soft proficiencies Block Chance, Aggro, Break Power, Resistance.

## Proposed identity
Adaptable frontline combat: balance offense, defense and Armor breaking; turn enemy pressure into offensive opportunities. Distinct from Berserker aggression and Knight dedicated protection. Auto-friendly, solo-capable, useful in parties.

## Trait — Fighting Spirit (proposal)
Successful blocks accumulate a bounded benefit for the next damaging skill, increasing damage and Armor depletion. Super Blocks grant additional progress; Super Block is a universal existing mechanic, not a Warrior-only ability. No mandatory new resource bar. Trait upgrades improve payoff. Stack limits, lifetime, consumption timing, coefficients, swap handling and upgrade milestones open.

## Selectable passives (revised proposals)
- Vanguard: baseline Aggro and Block Chance bonus; amplified when engaging multiple enemies or an elite/boss. Avoid dead passive in single-target encounters.
- Undaunted: increased Break Power versus intact Armor; damage bonus versus Broken enemies. Avoid dead passive during break windows.

## Ordinary active skill pool (eight candidates)
| Skill | Weapon | Function |
| --- | --- | --- |
| Cleave | Sword | Sweeping multi-target slash |
| Shield Bash | Shield | High Armor depletion and stagger against eligible targets |
| Onslaught | Sword | Advancing sequence of heavy strikes |
| Battle Cry | Either | Draw enemy Aggro and bolster personal defenses |
| Retaliation | Either | Brief guard stance; counterattack strengthened by damage absorbed during that stance; standard attack still occurs if not struck. No separate historical blocked-damage accumulation. |
| Iron Guard | Shield | Temporary defensive stance with increased Block Chance |
| Rupture | Sword | Downward Armor-breaking strike |
| Rally | Either | Temporary offensive enhancement for nearby allies |

Starter versus summonable allocation, distinct Iron Guard vs Retaliation roles, compatible weapon rules, numerical effects and animation timings remain open. Ordinary skills use shared Energy, cooldown and Impulse rules.

## Ultimate — Last Bastion (revised proposal)
Empowered state: increased Block Chance and Resistance, normal combat continues, successful blocks trigger automatic counters subject to an internal cooldown. Automatic counters do not consume Fighting Spirit. Concluding sweep consumes remaining Fighting Spirit for its offensive bonus. Normal offensive skills may consume it during the state; precise effect and consumption ordering open. Universal Energy cost, no separate ultimate gauge.

## Review notes
Owner supplied design feedback identifying Fighting Spirit/Retaliation overlap, Vanguard's single-target weakness, Undaunted's post-break drop-off, universal Super Block clarification and Last Bastion consumption clarity. Revisions above are assistant proposals addressing feedback, pending owner approval. Exact numbers, starting skill selection, class automation behavior and talent interactions to design next.
