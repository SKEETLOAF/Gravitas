# Shared RPG combat and equipment foundations
2026-11-26 | Exploration framework; not a finalized mechanic specification.

## Owner discussion priority
Establish general RPG mechanics before individual class kits: DPS, tanking, sustain, burst, damage over time, buffs/debuffs, healing, crowd control, status effects, equipment slots and related systems. These are discussion subjects, not all confirmed mechanics. Preserve the established fast-paced automated hack-and-slash direction and optional active intervention, class expansion, weapon compatibility, and future manual controls.

## 1. Combat vocabulary
Roles describe contribution: tank, damage dealer, healer, support, controller.
Specialties describe delivery or approach: sustained DPS, burst, DoT, area effects, single-target, sustain, healing, mitigation, shielding, buffs, debuffs, CC, break, counter, execution, mobility, summoning, resource support. Roles are not exclusive restrictions. Distinguish damage throughput (DPS), delivery pattern (burst/DoT), target pattern (single/area/cleave/chain), and utility (healing/buff/control). Classes may combine specialties; none are assigned here.

## 2. Shared combat rules to explore
- Health, damage, defeat, recovery, revives; posture or stagger as a possible separate system.
- Offensive and defensive attributes, derived statistics, scaling and caps; no fixed stat names or formulas.
- Damage categories (physical/magical/possible true), optional elemental affinities, delivery tags (basic/skill, direct/periodic, melee/ranged, single/area); these are orthogonal and not finalized.
- Critical hits, penetration/resistance, shields, healing, threat/aggro, targeting, defensive actions, movement and interruption.
- Combat resources: shared or class-specific gauges, costs, regeneration, swap behavior.
- Ability tags, targeting, cooldown ownership, status application and action/event ordering; automated and manual use share rules.
- Balance solo and party roles; avoid mandatory manual checks or making support unable to progress alone.

## 3. Status system candidate catalog
Periodic damage: Bleed (physical wound), Burn (fire damage), Poison (lingering damage).
Soft control: Slow (movement), Weaken (offensive power), Vulnerable (damage taken), Sunder (defense).
Hard control: Stun (action interruption/disable), Root (movement restriction), Silence (skill restriction), Freeze (temporary disable), Knockdown/Launch (physical reactions; may be separate action states rather than timed statuses).
Positive effects: Haste, Fortify, Regeneration, Barrier, Empower, Cleanse (instant removal rather than persistent status), Immunity/resistance.
Potential other effects: marks, curses, taunt/threat changes, anti-heal, dispel. None are confirmed. Keep damage types separate from statuses; fire damage need not always burn. Avoid duplicating statuses with indistinguishable purposes.
For each accepted status define application, magnitude, duration, tick frequency, stacking/refresh/overwrite rules, source and scaling, targets, cleanse/dispel, immunity/resistance, boss behavior, swap persistence, indicators and automation response. Decide CC resistance/diminishing returns and boss break rules before tuning permanent lockdown. Cross-class effects may persist after a swap if intentionally designed; no general policy yet.

## 4. Equipment slot architecture (candidate starting layout)
- Weapon loadout: primary and secondary; two total equip slots tentative, exact global/per-class rule and shield/off-hand meaning unresolved. Do not create a third off-hand slot by accident.
- Armor: head, chest, legs, hands, feet as possible distinct slots; compact alternative combines armor pieces.
- Accessories: necklace, ring slots, optional relic or trinket.
- Cosmetic appearance separate from stat-bearing equipment; no pets/relics/multiple accessory layers required yet.
- Gear questions: class-neutral vs restricted pieces, stat requirements, scaling, item level/rarity, affixes, sets, unique effects, sockets, upgrade paths, loadouts, inventory, loot filtering, gear behavior on class swap.
- For a single multiclass character, shared armor/accessories are a recommended starting point; per-class gear sets are an alternative and not decided. Weapon compatibility remains in WEAPONS.md. No slot count or item model is confirmed.

## 5. Next exploration order (recommendation)
1. Combat roles and specialties, including overlap and meaningful distinctions.
2. Core combat rules, damage categories, defensive and recovery systems.
3. Status effects and interaction rules.
4. Character attributes and resource/stat architecture.
5. Equipment slots, item stats and gear progression.
6. Universal class/weapon kit anatomy and promotion progression, then individual foundations.
Order is flexible; retain the existing 24-branch master index. No individual kits, formulas, exact status values, equipment counts or final class assignments established here.

## Elemental and supplemental development
See [ELEMENTS.md](ELEMENTS.md) for the owner's element roster, original reaction direction, refined status and cosmic catalyst proposals, modular VFX approach, and relic/mount/pet decisions. Relics are confirmed as unique upgrades; their equip structure remains open. Mounts and pets are desired; exact mechanics remain open.

## Owner decisions superseding resource/defense exploration
Universal Energy for all skills/ultimates, no generic ultimate gauge; attack/fire rate and cooldown-driven attacks, stat-based chance block/evasion versus counters, Aggro as attribute; detailed choreography deferred. See [SKILLS-AND-COLLECTION.md](SKILLS-AND-COLLECTION.md) for regeneration proposals, skill progression, pet/mount design and open decisions. Relic specifics deferred to a future update.


## Raw stat overflow and critical tiers (2026-11-26)
Owner specifies stats should be able to exceed 100% because debuffs and counter stats exist; Critical Chance above 100% introduces Super Crits and above 200% Ultra Crits. Do not impose a universal raw 100% cap on stats. Separate permanent/passive stat values, temporary modifier caps, counter-stat resolution and effective probability. Recommended critical overflow: after applicable buffs/debuffs/counters, effective crit chance C between 0 and 100 gives C% chance normal critical; 100 to 200 guarantees critical with (C-100)% chance super; 200 to 300 guarantees super with (C-200)% chance ultra; 300 guarantees ultra. One tier resolved per hit; do not multiply separate independent crit rolls. Values beyond 300 remain available as a buffer against reductions; additional reward tiers or overflow conversion not confirmed. Recommended crit tier multipliers scale the bonus portion of Critical Damage (normal 1x bonus, super 2x bonus, ultra 3x bonus) rather than exponentiating full multipliers; exact tier scaling pending. Distinguish percentage-point reductions from multiplicative reductions, and resolve before tier selection. Evasion/block may retain raw overflow against counters without implying guaranteed defense or new tiers; effective chance rules remain open. Skill coefficients remain outside temporary stat buff limits.


## Critical damage baseline clarification (2026-11-26)
Owner confirms non-critical stat overflow is for countering clashing stats and debuffs, not separate overflow reward tiers. Owner expects double base critical damage; recommended default 200% total (100% bonus). Proposed linear bonus scaling yields 2x/3x/4x normal/super/ultra at base, pending confirmation of tier multipliers.


## Additive critical damage (2026-11-26)
Owner sets base critical bonus to +50% (150% total damage), superseding earlier double-damage recommendation. Critical Damage attribute adds directly in percentage points to this base bonus. Recommended retained linear tier scaling: total multiplier = 1 + tier * (0.5 + additive Crit Damage attribute expressed as decimal), tier 0 normal, 1 critical, 2 super, 3 ultra. At zero attribute: 1.5x/2x/2.5x; +50% attribute: 2x/3x/4x. Base and additive attribute confirmed; exact higher-tier formula remains recommendation pending confirmation.
