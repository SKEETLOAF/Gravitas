# Elementalist — Prestige I kit (working draft)

Status: assistant proposal for owner review, not implementation or numerical tuning. Mage -> Elementalist -> Warlock is the established working sequence; deliberate elemental sequencing and reaction amplification are the established broad identity. Exact Trait exception, profile, weapons, Core affinity selection, skills and talents below remain proposals. [Mage](MAGE.md), [Elements](../ELEMENTS.md), [Class architecture](../CLASSES.md), [Talents](../TALENTS.md).

## Profile
Magical DPS/controller. Mage retains flexible, efficient spellcasting and neutral damage; Elementalist specializes in meaningful reactions; Warlock retains curses, lingering afflictions and accumulated-effect detonation. Proposed primary Magic Staff, secondary Tome (both inherited compatible families). Health D(2), Energy B(4), ATK F(1), MATK S(6+1 surcharge), DEF D(2), MDEF C(3) = 19. Proficiencies Effect Potency, Effect Duration, Penetration, Energy Recovery. No new universal elemental attribute or universal elemental weakness matrix. Focus on six core elements; Necrotic/cosmic reaction manipulation remains future class territory. Inherit compatible ordinary Mage spells, not Spellweaver or exclusive class passives.

## Trait — Catalysis
- Personally triggering a natural core primer/reactor reaction improves the applicable existing reaction property within a cap (damage, application, Armor pressure, coverage, etc.; define per reaction; no blanket CC extension). Only a paid/direct eligible spell or eligible Core finisher can own a Trace-creating reaction; no proc or secondary reaction.
- If the natural reaction actually consumes some primer, retain one temporary personal Trace of that consumed primer on the primary target (only one outstanding per caster, latest eligible replaces it). A later distinct compatible reactor element on the same target may consume that Trace to perform one reduced-strength reaction, e.g. Fire -> Cold (Thermal Shock) -> Lightning (Overload from Fire Trace). No extra actual primer status; trace is private and not usable by allies. No repeat of the same reactor element, no Trace from a Trace reaction, no free recursive effects.
- Natural compatible reactions take priority over Trace use; if a direct activation triggers a natural reaction against the target, do not also consume Trace for that target on that activation. Newly created Trace cannot be used within its creation action. Existing global status coexistence/consumption and primer-first ordering remain unchanged for all other interactions. Trace uses bounded actual consumed primer amount and its own expiry; no duplication of consumed ally status. Trace bonus does not increase its own creation budget. Reaction damage ownership follows trigger source; party/pet primers may qualify when Elementalist personally triggers natural reaction. No credit if ally triggers Elementalist's primer.
- Two-element builds benefit from the baseline natural reaction bonus; Concentrated Formula selectable passive provides stronger repeated-pair option rather than forcing three elements. No new spendable gauge; readable target/caster indicator of Trace element. Expiry, class switching and caps open; recommended no inactive Trace generation or consumption, timer continues during swap, normal persistent effects finish independently.
- Reaction definitions, exact consumption quantities, precedence among simultaneous valid reactions and ownership are unresolved global dependencies; do not hard-code unapproved universal formulas here. No general reaction cooldown added. Normalize multi-hit/AoE application by skill-defined budget and event attribution.

## Selectable class passives (2)
- Concentrated Formula: improve natural reaction effectiveness in exchange for forgoing Trace creation, allowing strong two-element and repeated-pair builds. Explicitly exclude Trace-specific talents or show incompatibility before purchase; base tree major talents below remain useful without Traces.
- Harmonic Sequence: retains Catalysis Trace and improves the existing primary property of the distinct reactor that consumes it (reduced-strength secondary reaction still capped). No additional Trace, status or reaction count. Intended multi-element alternative; compare actual DPS/utility to Concentrated Formula.

## Legendary Core skills (2; one equipped)
- Primordial Script (guaranteed): neutral magical sequence, finisher applies selected primer (Fire/Water/Earth) once at bounded potency. Default Fire; affinity chosen outside combat in Core configuration, stored with loadout (candidate small option, not a new combat key or skill slot). Same weapon-family moveset and distinct element VFX. No simultaneous primers.
- Conductor's Verse (alternative): neutral magical sequence, finisher applies selected reactor (Resonance/Cold/Lightning) once at bounded potency, useful for closing reactions. Default Cold; same outside-combat affinity proposal. Never automatically changes element to force a reaction. Both have useful normal damage with no reaction.
Affinity selection is proposed, not existing confirmed feature; fallback fixed Fire and Cold Core variants if new configuration is undesirable. Normalize status application and chain frequency; compatible inherited Ember Script remains an ordinary question of Core inheritance, not assumed.

## Ordinary active skills (10; 3 equipped)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Flame Brand | Either | Focused Fire strike followed by a short residual burn-producing field; one bounded Burn application budget rather than refresh per tick. Primer. |
| Normal | Deluge | Either | Broad Water surge applies Soaked over a short area, prioritizing primary target. Primer. |
| Normal | Fault Spike | Either | Erupting Earth spike applies Fracture and strong Armor pressure, useful against intact Armor. Primer. |
| Normal | Rime Shards | Either | Fan of Cold projectiles applying Chill; capped application per target per activation. Reactor. |
| Rare | Resonant Vortex | Either | Resonance field applies Reverberation, nudges susceptible enemies toward center; fallback Armor pressure on resistant foes. Reactor, not Force. |
| Rare | Storm Needle | Either | Concentrated Lightning strike then limited arcs to distinct nearby enemies; Shock, no self-bounce or repeated same-target application. Reactor. |
| Rare | Confluence | Either | Neutral magical sigil around a selected enemy area; next paid elemental skill landing in it gains bounded application effectiveness. One enhancement per activation and capped targets; no element applied by sigil itself. |
| Rare | Elemental Mantle | Either | Temporary personal Resistance buff; first incoming harmful elemental status application during buff is weakened according to normal Resistance rules. Next paid elemental spell gains modest Effect Potency. No cleanse/immunity or implicit element. |
| Legendary | Prismatic Lance | Staff | Powerful directional projectile with a reactor affinity selected outside combat (Cold/Lightning/Resonance; default Lightning); applies only chosen reactor, concentrates impact against primary target and has partial secondary coverage. No automatic reaction. |
| Legendary | Elemental Crucible | Tome | Persistent neutral magical field; first natural core reaction personally triggered in area per paid field activation gains enhanced applicable property and limited coverage; field then collapses in a neutral magical impact with no new status/Trace. Useful baseline collapse even if no reaction occurred by expiry. |
Either means Staff or Tome. All skills follow ordinary Energy, cooldown, Impulse, accuracy, resistance and Armor rules. Exact skill application quantities, durations, tags and timings TBD. Avoid adding a third elemental matrix, silent multi-element damage or guaranteed control.

## Collectible passive skills (5)
- Scorched Earth: Flame Brand trades direct impact for longer residual Fire field and increased bounded Burn application budget; still no per-tick infinite refresh.
- Tidal Imprint: Deluge trades area coverage for concentrated Soaked application on fewer targets. Useful bosses; no guarantee through Resistance.
- Glacial Fracture: Rime Shards trades part of its Chill application for stronger direct Armor pressure when hitting Fracture-afflicted enemies; normal Shatter only if real valid reaction occurs, no duplicate free Shatter.
- Stormfront: Storm Needle trades some primary damage for greater arc reach and distinct-target coverage; bounded total hit/application budget, isolated baseline retained.
- Convergent Formula: Elemental Crucible trades part of neutral collapse damage for stronger first qualifying reaction modifier; no extra reaction or Trace. Staff-only alternatives should remain viable through other passives.

## Example builds and automation
- Thermal Artillery: Primordial Script (Fire) / Rime Shards, Prismatic Lance (Cold), Confluence / Concentrated Formula / Warfare, Flow. Straightforward repeated Thermal Shock without Trace.
- Storm Cycle: Primordial Script (Water) / Resonant Vortex, Storm Needle, Deluge / Harmonic Sequence / Tempo, Warfare. Water -> Resonance (Tempest) -> Lightning (Electro-Charge via Trace if no competing natural reaction). Deluge re-primes. Do not assume outcome if another natural status takes precedence.
- Tectonic Control: Conductor's Verse (Cold) / Fault Spike, Storm Needle, Elemental Crucible / Harmonic Sequence / Warfare, Endurance (candidate Influence if approved). Earth -> Cold Shatter -> Lightning Magnetize via Trace where eligible; Tome for Crucible.
- Presets can order primer then reactor then alternate reactor; auto respects valid target, actual status/Trace, Energy, cooldown, recovery and zone. Simple fixed sequences still useful without conditional optimization. Do not introduce new macro language or force manual aim. Party and pet application can create alternate opportunities; prefer normal valid reactions rather than stalling indefinitely.

## Talent tree — Elemental Dominion (working name)
Innate: MATK and Effect Potency. Independent class forks, base and first expansion use standard P0/P I cost profiles, availability of promoted-class sections unresolved. Each legal route costs 30 TP. No Trace-only mandatory nodes, so both class passive choices remain supported. Effects, prerequisites, exact tags and coefficients draft.

### Base (1–3 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [1] MATK; [1] Energy; [2] Effect Potency |
| Fork 1 L — Primer Mastery | [1] Effect Duration; [1] Primer skill damage; [2] Primer application effectiveness; [3] Deep Imprint: eligible primer skills concentrate more application on their primary target, trading a bounded portion of secondary application; single-target skills instead gain a small primary application bonus |
| Fork 1 R — Reactor Mastery | [1] Penetration; [1] Reactor skill damage; [2] Reaction impact effectiveness; [3] Reactive Geometry: eligible reactor projectiles gain a small impact area when landing on a naturally primed target; no duplicate hit or free status on the original target |
| Shared | [1] Energy Recovery; [2] Catalysis natural reaction effectiveness; [2] Elemental direct skill damage |
| Fork 2 L — Concentration | [1] Penetration; [2] Single-target spell damage; [2] Break Power on applicable reactions; [3] Condensed Reaction: eligible area reaction damage concentrates part of its unused coverage budget against an isolated target; no conversion of unused control duration into damage by default |
| Fork 2 R — Diffusion | [1] Effect Duration; [2] Area skill radius; [2] Secondary target application effectiveness; [3] Diffusion: eligible area primer skills extend a portion of their application to the perimeter of the existing impact area, with reduced potency and strict target limit |
| Conclusion | [1] Energy Efficiency; [2] Effect Potency; [3] Elemental Continuity: after a natural reaction, the next distinct paid elemental skill improves its existing primary property, such as primer application or reactor impact, once per reaction-owning action |

### First expansion (2–6 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [2] MATK; [2] Effect Potency |
| Fork 1 L — Primer Mastery | [3] Primer skill application effectiveness; [5] Elemental Reservoir: eligible persistent primer fields redistribute a bounded part of their remaining application budget to a previously affected enemy that leaves the field, once per field; no duration reset or unlimited application |
| Fork 1 R — Reactor Mastery | [3] Reactor skill effectiveness; [5] Reactive Momentum: the first distinct reactor spell after a natural reaction gains reduced casting recovery within animation floors; no cooldown reset or free cast; usable in two-element builds with distinct same-element reactor skill IDs |
| Shared | [2] Energy Efficiency; [2] Catalysis natural reaction effectiveness |
| Fork 2 L — Concentration | [4] Reaction impact and applicable Armor depletion; [6] Focused Catalyst: eligible area reactions on isolated targets concentrate a greater share of their existing damage budget onto the primary enemy, and eligible non-damaging control reactions gain a bounded Armor-pressure option against resistant bosses; no second reaction or repeated damage event |
| Fork 2 R — Diffusion | [4] Area effect and secondary application effectiveness; [6] Cascade Circuit: a naturally triggered reaction may redirect a reduced portion of the triggering skill's existing elemental application budget to one nearby compatible primed target within its expanded impact area; normal consumption, separate reaction ownership, no Trace creation from this secondary reaction |
| Conclusion | [4] Master of Elements: first qualifying paid elemental skill following a natural reaction gains improved applicable primer/impact property; if a Trace exists, its lifetime is preserved during this skill's ordinary windup, never extended past a fixed grace cap |

## Critical review and dependencies
- References: Last Epoch Runemaster https://support.lastepoch.com/hc/en-us/articles/46363095981723-Runemaster-Skills and https://support.lastepoch.com/hc/en-us/articles/46362196459675-Runemaster-Skill-Tree (order/combinations, skill mods); October 2026 developer report https://forum.lastepoch.com/t/eterra-monthly-october-edition-2026/82143 (centralization warning); Genshin community mechanics https://library.keqingmains.com/evidence/combat-mechanics/elemental-effects/elemental-gauge-theory (consumption and triggers); Guild Wars 2 https://wiki.guildwars2.com/wiki/Combo and https://wiki.guildwars2.com/wiki/Attunement (field/finisher and elemental identities). GGM accessibility, no copying exact mechanics.
- Largest risk: Trace exception complicates reaction ownership, priority and status application. Establish a deterministic global reaction resolver first, then test private Trace behavior against real competing statuses, party/pet primers, multi-target skills, boss CC resistance, target death, class switches and simultaneous triggers. No recursive reactions or status duplication.
- Test repeated-pair vs varied-element builds across solo, auto, co-op, boss, farming, high Resistance and different weapons. Do not let multi-element diversity be obligatory or Concentrated Formula erase the value of Catalysis. Direct neutral Mage builds remain competitive. Preserve Warlock affliction, Spellblade infusion, Sage allied amplification territory.
- Review duplicate primer/reactor functions with Mage skills, distinguish via coverage, field geometry and application properties, not raw power creep. Elemental Mantle and Confluence compete for scarce active slots; prove utility against another damaging spell.
- Expensive talents change application distribution, coverage, recovery or reaction behavior. Validate equivalent 30-TP route utility and no dead nodes. Focused Catalyst vs Condensed Reaction stacking and Cascade Circuit vs universal area mods need explicit budgets. Eight static route-cost checks passed; no gameplay testing or numerical validation.
