# Combat foundations
Updated 2026-11-26. Current rules; numerical tuning open.

## Combat vocabulary
Roles: tank, damage dealer, healer, support, controller. Specialties: sustained DPS, burst, DoT, AoE, single-target, sustain, healing, mitigation, shielding, buffs/debuffs, CC, break, counters, execution, mobility, summoning, resource support. Classes can combine specialties. Damage classification separates physical/magical (possible true damage), delivery, source, target pattern, range, crit and element. See [Elements](ELEMENTS.md).

## Current attribute roster (29)
| Category | Attributes |
| --- | --- |
| Fundamental | Health, Energy |
| Offense | Attack (ATK, physical), Magic Attack (MATK), Critical Chance, Critical Damage, Accuracy, Penetration, Break Power |
| Defense | Defense (DEF, physical), Magical Defense, Critical Defense, Critical Resistance, Block Chance, Evasion, Resistance |
| Speed/efficiency | Attack Speed, Movement Speed, Cooldown Reduction, Energy Recovery, Energy Efficiency |
| Sustain/utility | Health Regeneration, Lifesteal, Aggro |
| Status | Effect Potency, Effect Duration |
| Farming | Drop Rate, Experience Gain, Currency Gain |
The consolidated list is covered for conceptual design; exact formulas and some earlier candidate stats' implementation remain open. No general AP, separate penetration stats, generic Damage Reduction, Healing Power or Shielding Power. A descriptive Combat Power rating is optional, not a damage stat.

## Clashing attributes
| Offensive | Defensive |
| --- | --- |
| Accuracy | Evasion and Block Chance |
| Penetration | Defense and Magical Defense |
| Critical Chance | Critical Resistance |
| Critical Damage | Critical Defense |
| Effect Potency | Resistance |
| Break Power | Armor |
Raw stats may exceed 100%; excess counters opposing stats/debuffs, except explicit Crit and Block tiers. Suggested direct percentage-point subtraction for opposing chance stats; exact formulas open. Resistance influences harmful status application/duration. Healing scales with MATK. Shields scale according to creating skill and can increase recipient Block Chance.

## Critical and Block
- Established: base crit bonus +50% (1.5x total), Critical Damage attribute adds percentage points to it. Above 100% effective Critical Chance enables Super Crit; no Ultra Crit for now. Critical Resistance counters chance/tier; Critical Defense counters crit damage.
- Established: ordinary Block leaves 50% damage, above 100% effective Block Chance enables a stronger block leaving 25%.
- Recommended tier resolution for both: 0–100% chance of ordinary success; 100–200% guarantees ordinary success with excess chance of stronger tier; 200% guarantees stronger tier. Excess above 200% counters reductions, not additional tiers. Resolve counters before tier roll.
- Recommended Super Crit damage: 1 + 2 * (0.5 + Critical Damage attribute as decimal), normal crit 1 + (0.5 + attribute). Critical Defense reduces bonus portion without making crit weaker than normal. Exact formulas pending.
- Evasion is the specialty of agile/dexterous builds; Block favors tanks/high-Aggro builds. No class exclusivity or automatic Aggro-to-Block conversion. Suggested resolution: evasion, then block, then relevant mitigation; final order open.

## Armor and Break
Enemy breakable Armor is derived from defense, incrementally stronger on elites/bosses. While intact it increases Resistance, making statuses harder to trigger and shorter. Break Power accelerates armor depletion. Players probably will not have breakable Armor by default; ordinary equipment armor, shields and Defense remain. Recommended separate integrity gauge; armor recovery, break stagger, HP mitigation, exact formulas and player exceptions open.

## Energy and automated combat
All skills including ultimates consume Energy; no universal ultimate gauge. Specific skills may introduce stacks, gauges or charges. Attacks follow weapon attack/fire rate, skill cooldowns and basic-chain recovery. A completed basic combo has brief recovery, often following knockback; class swap can extend the combo and rush the displaced target. Auto alternates class skills or full basic chains; see COMBAT-SWITCHING.md. Stat-based automatic defensive actions; optional active input; full manual mode and detailed choreography deferred. Suggested shared Energy across swaps, free basic attacks and passive plus normalized on-hit recovery. See [Skills](SKILLS-AND-COLLECTION.md) and [Switching](COMBAT-SWITCHING.md).

## Equipment slots
Conceptually covered: primary/secondary weapon, head, chest, hands, legs, feet, necklace, ring; relic deferred. Two global weapon slots shared across both class selections. Armor, accessories and companions are shared and unchanged on class swaps. Exact ring count and shield/off-hand handling open. Itemization in [ITEMIZATION.md](ITEMIZATION.md).

## Open calculation work
Damage/defense formulas, counter resolution, crit bonus mitigation, armor durability/regen, Energy rates, threat, skill coefficients, chance limits and buff/debuff ceilings (see ELEMENTS.md). No extra attribute or mechanic inferred from an example.
