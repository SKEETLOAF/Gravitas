# Hunter — Prestige I kit (working draft)

Status: assistant proposal for owner review, not implementation or numerical tuning. Ranger -> Hunter -> Gunslinger is the established sequence; tactical prey manipulation, traps and area control are the approved broad identity. This specific kit, Trait, profile, weapons and talents are unconfirmed. [Ranger](RANGER.md), [Class architecture](../CLASSES.md), [Talents](../TALENTS.md).

## Profile
Tactical physical DPS/controller. Ranger specializes in reliable direct precision; Hunter prepares and exploits prey, controls groups and provides Armor pressure; Gunslinger retains firearm territory. Proposed Bow primary, Polearm secondary (hunting spear); both weapon families in existing roster. Dagger-specific ancestor skills are not implicitly converted. Inherit compatible learned ordinary actives, not Deadeye or exclusive class passives. Health C(3), Energy B(4), ATK A(5), MATK F(1), DEF C(3), MDEF C(3) = 19 allotment. Proficiencies Penetration, Break Power, Effect Potency, Effect Duration. No new universal stat, pet or companion requirement.

## Trait — The Hunt
- First direct landed attack when no valid Quarry exists designates that enemy. One Quarry per Hunter, class-specific ownership, not universal harmful status. Death/invalid target clears it; legitimate manual/auto target commitment may replace it with bounded transition rules, no swap spam.
- A landed eligible trap, pursuit or restraint setup skill on Quarry creates one temporary nonstacking Opening. Next eligible direct damaging ordinary active (payoff-tagged, distinct activation) against that target consumes Opening for additional Penetration and Armor depletion. Setup skills cannot also consume or refresh by their own secondary damage. Resolve consumption on first eligible landed hit (candidate; snapshot relevant effect for that activation, normalize multihit). Openings can be created on control-resistant bosses even when displacement/Slow fails, provided setup lands.
- No mandatory trap, gauge, crit or successful CC. Non-trap setups viable. Trap damage and restraint effects have useful baseline without Quarry. Trait only functions while Hunter active; applied effects and placed traps retain bounded normal lifetime and paid ownership through swaps, no inactive Trait gain unless explicitly approved. Exact duration, re-target policy, caps, coefficients and event ordering open.
- Auto places traps in selected enemy/cluster's valid combat area, waits normal arming delay, triggers if an enemy is already occupying or enters footprint; stationary bosses don't need to walk into traps. No tracking after placement by default, no detonation outside footprint, no automatic refund for expired traps. Manual target/zone overrides use existing controls. Limit active traps per caster and total runtime objects; no pre-pull infinite setup, scripted zone bypass or recursive trigger. Use visible footprint and armed state.

## Selectable class passives (2)
- Trapper: baseline Effect Potency, improved trap coverage and reduced arming delay to a floor; also modest restraint effectiveness for non-trap builds.
- Pursuer: baseline Penetration; after successfully exploiting an Opening, next distinct pursuit or restraint setup gains bounded recovery/approach effectiveness. No cooldown reset or duplicate trigger.

## Legendary Core skills (2)
- Trailblazer (guaranteed, either): balanced direct sequence with a sweeping finisher. Completing chain improves the next eligible trap's arming speed or restraint skill's impact, one readiness, floor/cap; no trap requirement.
- Stalker's Rhythm (alternative, either): faster focused sequence; finishing strike gains additional Armor depletion against Quarry when an Opening exists, does not consume it. Baseline finisher useful outside Opening. No automatic target teleport. Both reuse weapon-family animations.

## Ordinary active skills (10, 3 equipped)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Snare Trap | Either | Throw trap into valid target area; after short arming, occupancy triggers physical damage and Slow if susceptible. Setup. |
| Normal | Tracking Shot | Bow | Direct precision projectile; bonus Penetration against designated Quarry, eligible payoff. No automatic mark transfer. |
| Normal | Driving Thrust | Polearm | Advancing thrust with Armor pressure, creates Opening on Quarry even if movement resisted. Setup. |
| Normal | Flush Out | Either | Short sweeping attack displaces susceptible enemies away from Hunter within valid geometry; additional Armor depletion if control fails. Setup. |
| Rare | Shrapnel Trap | Either | Armed physical burst with directional fragment damage, stronger primary hit against intact Armor. Setup, no new Bleed requirement. |
| Rare | Binding Line | Either | Throw tether to target, applies Slow if eligible; direct physical impact and bonus Armor depletion against control-resistant enemies. Setup. No forced boss movement or unique universal tether status. |
| Rare | Ambush | Either | Swift approach or stationary close-range strike against Quarry, then retreat within permitted geometry; direct impact creates Opening, no free teleport. Setup. |
| Rare | Crossfire | Bow | Direct spread volley, focuses initial projectile on Quarry and reduced secondary hits on nearby enemies; eligible payoff, useful isolated-target baseline. |
| Legendary | Deadfall | Either | Deploy heavy trap with longer visible arming delay; large physical area impact, strong Armor depletion; creates Opening, useful stationary bosses. Setup. |
| Legendary | Apex Strike | Either | Powerful concentrated ranged shot or polearm strike based on wielded weapon; when consuming Opening, concentrates bonus impact on primary target with useful normal baseline. Payoff. |
All actives use Energy, cooldown, normal accuracy/crit and existing Impulse/Armor rules. Tags are draft; inherited compatible direct actives may be payoff-tagged by explicit registry, not automatically every inherited skill.

## Collectible passive skills (5)
- Quickset: Snare Trap arms sooner and has larger trigger radius, at cost of reduced initial damage; no instant or invisible activation.
- Fragmentation: Shrapnel Trap trades some primary burst for wider fragment coverage; no recursive fragments or repeated same-target hits.
- Dragline: Binding Line pulls susceptible smaller enemies a short distance toward impact location; on control-resistant foes substitutes bounded Armor pressure instead. Obeys encounter rules; no forced boss relocation.
- Trail Memory: when Quarry is defeated by an eligible direct payoff, the next distinct setup gains a bounded Energy discount; once per action with internal cooldown; no refunds for proc kills.
- Execution Window: Apex Strike used against an opened Quarry gains stronger concentrated impact, at cost of reduced secondary coverage/recovery (choose one tradeoff during tuning); useful against bosses independent of low-Health execution, no instant kill.

## Example builds
- Trapper: Trailblazer / Snare Trap, Deadfall, Apex Strike / Trapper / Warfare + Flow. Both weapons compatible. Automatic trap placement on valid occupied zone, separate setup/payoff.
- Pursuer: Stalker's Rhythm / Ambush, Driving Thrust, Apex Strike / Pursuer / Tempo + Opportunity. Polearm build with no traps.
- Battlefield controller: Trailblazer / Binding Line, Shrapnel Trap, Crossfire / Trapper / Warfare + Endurance (or candidate Influence if approved). Bow needed for Crossfire.
- Inherited builds may use eligible Ranger direct skills as payoff, subject to explicit compatibility, not inherited Trait.

## Talents — Hunting Grounds (working name)
Innate bonus: Break Power and Effect Potency. Two independent forks. Base section (P0 cost profile 1–3) and first expansion (P I profile 2–6) proposed; promoted-class section availability unresolved. Each legal route costs 30 TP; no acquisition before class unlock implied.

### Base (1–3 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [1] ATK; [1] Energy; [2] Penetration |
| Fork 1 L — Trapper | [1] Effect Duration; [1] Trap damage; [2] Trap arming speed within minimum delay; [3] Prepared Ground: compatible traps gain a wider trigger radius and may be thrown at a valid target zone without requiring movement to placement |
| Fork 1 R — Stalker | [1] Movement Speed; [1] Core damage against Quarry; [2] Pursuit skill recovery; [3] Track and Strike: Driving Thrust and Flush Out retain their setup effect against a Quarry even when displacement is resisted; compatible approach attacks gain a bounded approach-range bonus |
| Shared | [1] Energy Recovery; [2] Opening Penetration; [2] Opening lifetime |
| Fork 2 L — Containment | [1] Effect Potency; [2] Trap and restraint radius; [2] Break Power against intact Armor; [3] Crippling Ground: Snare Trap and Binding Line leave short Slow zones along their existing impact footprint; against control-resistant targets, substitute capped Armor pressure once per cast |
| Fork 2 R — Exploitation | [1] Accuracy; [2] Direct active damage against Quarry; [2] Opening Armor depletion; [3] Cull the Herd: compatible payoff skills transfer a portion of primary Opening benefit to other targets hit by the same setup, without extra primary hits |
| Conclusion | [1] Energy Efficiency; [2] Penetration; [3] Predator's Rhythm: exploiting an Opening strengthens the next distinct setup skill's primary damage or control property, once per cycle |

### First expansion (2–6 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [2] ATK; [2] Effect Potency |
| Fork 1 L — Trapper | [3] Trap damage and coverage; [5] Mobile Snare: eligible thrown traps can be attached to the Quarry at placement, arming after normal delay and following permitted movement until activation; trades some area radius for reliable contact |
| Fork 1 R — Stalker | [3] Pursuit skill effectiveness; [5] Relentless Tracking: eligible pursuit skills adapt between a short approach and stationary close-range strike without forced displacement, retaining Opening creation and reducing unnecessary recovery |
| Shared | [2] Energy Efficiency; [2] Opening effect strength |
| Fork 2 L — Containment | [4] Restraint and Armor pressure effectiveness; [6] Hunting Grounds: eligible trap/restraint skills maintain a bounded residual control area; the first subsequent direct payoff skill hitting the Quarry within that area converts its remaining duration into capped extra Armor pressure, or damage against Broken targets, and ends the field |
| Fork 2 R — Exploitation | [4] Opening exploitation damage; [6] Kill Corridor: eligible direct payoff skills striking the opened Quarry transmit a reduced share of their existing impact to other enemies affected by the same setup; isolated-target fallback concentrates a capped portion of that share on the Quarry rather than adding a separate hit |
| Conclusion | [4] Master of the Hunt: after exploiting an Opening, a legitimate target transition preserves a bounded preparation benefit for the next distinct setup skill; no transfer of an unspent Opening or reset of cooldowns |

## Critical review
References: Last Epoch Falconer skill interactions https://support.lastepoch.com/hc/en-us/articles/46363186901019-Falconer-Skills and https://support.lastepoch.com/hc/en-us/articles/46363019656859-Falconer-Skill-Tree ; Diablo IV Rogue trap interactions (historical patch, not current numerical values) https://news.blizzard.com/en-us/article/24196854/diablo-iv-patch-notes-2-2 ; Guild Wars 2 trap/control https://wiki.guildwars2.com/wiki/Trap and https://wiki.guildwars2.com/wiki/Trapper%27s_Expertise . GGM remains accessibility and auto-build reference.
- Biggest risk: a trapper becomes a delayed AoE caster in automatic combat, or traps become useless when foes move. Preserve visible setup/arming, purposeful control, timing and manual placement advantage without forcing manual play. Mobile Snare changes spatial reliability at cost of area; not universal mandatory upgrade.
- Compare trapper and pursuit builds against moving mobs, stationary bosses, control resistance, isolated targets, grouped enemies, forced zones, target death, class swaps and co-op. Avoid permanently exposing bosses, global CC bypass, cascading proc loops or idle trap stockpiling. Prevent Cull the Herd/Kill Corridor from double multiplying damage; explicit source tracking and area hit budgets required.
- Avoid stealing Ranger's precision, Trickster ricochet, Druid nature companion, Gunslinger firearm, or Assassin execution territory. Hunter isn't a pet summoner; animal-themed skill variants optional later.
- Some branch talents are deliberately tag-restricted; test weapon and rarity coverage and ensure both compatible weapon-only builds have usable setups/payoffs. Validate exact skill names, recovery modifiers and UI; Execution Window's tradeoff needs selection, final tuning TBD. No gameplay or numerical validation. Eight static route-cost checks passed.
