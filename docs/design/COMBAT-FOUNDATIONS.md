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
Grouping for class growth (no new attributes): six main attributes (Health, Energy, ATK, MATK, DEF, Magical Defense) and 23 soft attributes (all remaining listed attributes). Main attributes use a foundational 18-point Scaling Allotment with +1 per prestige (18/19/20 for P0/I/II; future sequential P III 21; hybrid/special budgets open) and F/D/C/B/A/S grades representing weights 1/2/3/4/5/6. A is the ordinary maximum; exceptional S focus has a one-point surcharge (weight 6, budget cost 7). Soft attributes have modest natural growth, with roughly comparable proficient growth across classes and substantially slower non-proficient growth. Approved normalized growth reference weights: 20 proficient or 5 non-proficient natural growth units against 75 external progression units. Natural rates are alternative per-attribute contributions, not additive; weights are balancing targets rather than literal realized percentages or caps. Exact normalization and curves remain open. Inherent main and soft growth contributions are 100% primary plus 50% distinct secondary regardless of overlapping affinities, or 150% primary when specializing; shared external contributions are not multiplied. Proficiencies are affinities, not restrictions; see CLASSES.md. Actual per-attribute growth curves and balancing remain open; see PROGRESSION.md. The consolidated list is covered for conceptual design; exact formulas and some earlier candidate stats' implementation remain open. No general AP, separate penetration stats, generic Damage Reduction, Healing Power or Shielding Power. A descriptive Combat Power rating is optional, not a damage stat.

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
Enemy breakable Armor is derived from defense, incrementally stronger on elites/bosses. While intact it increases Resistance, making statuses harder to trigger and shorter, and prevents ordinary stagger/knockback from combo hits and Impulse. Impulse can occur without interrupting the armored enemy. Break Power accelerates armor depletion. Players probably will not have breakable Armor by default; ordinary equipment armor, shields and Defense remain. Recommended separate integrity gauge; armor recovery, break stagger, HP mitigation, exact formulas and player exceptions open.

## Energy and automated combat
All skills including ultimates consume Energy; no universal ultimate gauge. Specific skills may introduce stacks, gauges or charges. Attacks follow weapon attack/fire rate, skill cooldowns and basic-chain recovery. A completed basic combo has brief recovery, often following knockback; class swap can extend the combo and rush the displaced target. Eligible skills (including support) create skill-specific Impulse hit-stun pulses that bridge attacks and skills, reset/extend basic chains, and knock back susceptible targets after a completed string. Auto-combat mixes skill extensions, basic strings and class swaps via easy-to-author presets and player-created macros; see [Combat flow](COMBAT-SWITCHING.md) for canonical rules. Impulse damage, timing and detailed cancel logic open. Stat-based automatic defensive actions; optional active input; full manual mode and detailed choreography deferred. Boss and raid encounter design must provide meaningful player intervention (owner-confirmed): select designated combat zones to reposition and evade attacks in semi-idle combat, brief clash QTEs, clickable/tappable exposed weak points for combat advantages, environmental hazards and co-op mechanics. Standalone precision-timing QTEs are excluded. Evolution trials must remain auto-clearable with sufficient strength. Direct free movement is reserved for the future action-RPG alternative, not required for semi-idle encounter control. Ordinary automated pursuit, movement and combo transitions remain intact. Recommend temporary zone-selection/input overrides that suspend conflicting automation and resume smoothly, readable telegraphs, device-accessible prompts, and bounded bonuses. Exact clash resolution, manual advantage, auto fallback, raid requirements, and timing remain open; weak-point damage/Armor depletion/attack interruption are candidate outcomes, not confirmed effects; specific hazard and co-op mechanics remain open. Suggested shared Energy across swaps, free basic attacks and passive plus normalized on-hit recovery. See [Skills](SKILLS-AND-COLLECTION.md) and [Switching](COMBAT-SWITCHING.md).

## Equipment slots
Conceptually covered: primary/secondary weapon, head, chest, hands, legs, feet, necklace, ring; relic deferred. Two global weapon slots shared across both class selections; primary weapon contributes 100% attributes, secondary 50%, independent of active weapon. Starting multiplier approved, subject to balance testing. Armor, accessories and companions are shared and unchanged on class swaps. Exact ring count and shield/off-hand handling open. Itemization in [ITEMIZATION.md](ITEMIZATION.md).

## Open calculation work
Damage/defense formulas, counter resolution, crit bonus mitigation, armor durability/regen, Energy rates, threat, skill coefficients, chance limits and buff/debuff ceilings (see ELEMENTS.md). No extra attribute or mechanic inferred from an example.
