# Berserker — Prestige I kit (working draft)

Status: owner explicitly approved missing-Health mitigation and faster Bloodlust generation as part of Berserker's defining identity on 2026-11-27, alongside the previously proposed Frenzy loop. Remaining kit, growth, weapon assignments, talent nodes and coefficients are assistant working proposals, not separately approved or implemented. [Class architecture](../CLASSES.md), [Warrior](WARRIOR.md), [Talents](../TALENTS.md).

## Profile
Offensive bruiser; sustained aggression, committed heavy impacts and self-sustain. Warrior converts blocks into offense; Berserker grows resilient and dangerous while wounded; Knight retains protection territory. Primary Greatsword, secondary Sword (proposed; existing weapon families). Inherit compatible learned ordinary Warrior skills, never Fighting Spirit or Warrior-exclusive class passives. Shield-specific skills require compatible equipped weapon and are not implicitly converted. Both new Core skills work with either proposed weapon family and reuse weapon-family animations. Growth Health B(4), Energy D(2), ATK S(6 + 1 surcharge), MATK F(1), DEF C(3), MDEF D(2): 19 total. Proficiencies Attack Speed, Lifesteal, Break Power, Critical Damage.

## Trait — Bloodlust
- Undying Fury: continuous missing-Health damage mitigation and increased Bloodlust generation. Illustrative curve from discussion: mitigation 0.4 x missing-Health fraction (up to 40% near zero Health), generation bonus 0.5 x missing-Health fraction. Not tuned. Use pre-hit Health snapshot and capped multiplicative mitigation, not a new universal stat; final order/caps open. No lethal-hit immunity or minimum Health floor.
- Completing Core chains and landing heavy-impact ordinary actives builds bounded Bloodlust, once per qualifying action (not per target/hit). Incoming damage is not required. After inactivity, progress decays.
- At maximum, enter Frenzy automatically after triggering action resolves; increased Attack Speed, heavy-impact damage, and explicit compatible skill properties. Baseline duration, generation, cooldowns and thresholds TBD. No Bloodlust banking during Frenzy (proposed), bounded duration extensions, no proc recursion. Frenzy effects use activation snapshot except live defensive mitigation; do not reset or refill when swapping. Proposed inactive Trait stops functioning, timer continues, state retained only until normal expiry; verify against switching rules.
- Health reduction does not require Frenzy. Healing still valuable; do not teach auto to deliberately stand in hazards or refuse healing. No separate spendable resource, no ultimate slot. Show Trait progress and state legibly.

## Selectable class passives (2)
- Juggernaut: Break Power and limited resistance to ordinary attack interruption during heavy-impact skills, never immunity to scripted mechanics.
- Ravenous: Lifesteal with greater effectiveness during Frenzy and while missing Health; cap actual healing and avoid multiplying proc-generated damage.

## Legendary Core skills (2)
- Ravager (guaranteed): escalating heavy swings; finisher delivers extra Armor depletion, gains coverage in Frenzy.
- Bloodrush (alternative): faster sequence, smaller individual impact, finisher has improved Lifesteal and greater Bloodlust contribution while injured outside Frenzy. Normalize generation across Core speeds.

## Ordinary active skills (10; 3 equipped)
| Rarity | Skill | Weapon (proposed) | Function |
| --- | --- | --- | --- |
| Normal | Reckless Swing | Either | Broad heavy sweep; Frenzy widens impact. |
| Normal | Stampede | Either | Advancing shoulder strike and brief momentum bonus to next direct attack; obey permitted combat zones. |
| Normal | War Cry | Either | Temporary ATK and Lifesteal, offensive bonus scales with missing Health at activation; no taunt or shield. |
| Normal | Heavy Cleaver | Either | Concentrated heavy strike with additional damage against intact Armor; distinct from Warrior Rupture's dedicated Armor depletion. |
| Rare | Whirlwind | Either | Sustained surrounding attacks, limited movement during activation; normalized Bloodlust if eligible, not per hit. |
| Rare | Earthshaker | Greatsword | Ground slam with directional shockwave beyond primary impact; distinct targeting from sweep. |
| Rare | Unchained | Either | Limited interruption resistance and accelerated Bloodlust outside Frenzy; during Frenzy grants brief capped additional mitigation instead (proposed refinement). |
| Rare | Savage Reprisal | Either | Heavy retaliatory blow, capped bonus based on recent actual Health lost from hostile damage; not prevented damage, no self-damage exploit; baseline when unhurt. |
| Legendary | Rampage | Either | Advancing heavy sequence; during Frenzy adds finisher, stronger when wounded; respect zone and recovery. |
| Legendary | Cataclysm | Either | Committed overhead strike and area shockwave; missing Health boosts primary impact, Frenzy concentrates existing shockwave force toward primary target. |
All skills use normal Energy/cooldown/Impulse rules. No new status or mandatory gauge beyond Trait readiness. Skills should remain useful at full Health. Snapshot missing-Health offensive modifiers at activation to prevent healing during a skill from unpredictably weakening it.

## Collectible passive skills (5)
- Reckless Abandon: War Cry trades Lifesteal bonus for stronger ATK/Attack Speed. A genuine offensive alternative, not unconditional improvement.
- Moving Tempest: Whirlwind permits greater movement and coverage, lower per-hit damage; obey zones.
- Aftershock: Earthshaker leaves delayed reduced-power ground impact with Armor depletion; secondary event cannot generate Bloodlust or recursively proc.
- Relentless Fury: direct heavy-impact activations during Frenzy extend remaining duration, strict cumulative extension limit, cannot extend from secondary damage.
- Death's Defiance: Cataclysm gains further bounded missing-Health impact and restores a limited amount of actual missing Health on primary hit. Tune independently of Lifesteal and avoid double-counting missing-Health damage.
Shared Warrior-lineage starter skills are not duplicated; compatible inheritance as established. Passive scope and inheritance rules remain open.

## Example builds
- Destroyer: Ravager / Heavy Cleaver, Earthshaker, Cataclysm / Juggernaut / Warfare, Opportunity. Greatsword required only for Earthshaker; Cataclysm works with Sword or Greatsword.
- Ravager: Bloodrush / War Cry, Whirlwind, Rampage / Ravenous / Tempo, Endurance.
- Unstoppable: Ravager / Unchained, Savage Reprisal, Rampage / Juggernaut / Flow, Endurance.
- Mixed Warrior/Berserker can use shared Sword; Warrior remains the stronger protection/Block specialist. Class-exclusive Trait interactions do not carry over.

## Talent tree — Primal Fury (draft)
Innate bonus: ATK and Lifesteal. Two independent forks, no route locking across them. Base and first expansion use established P0/P I cost profiles respectively; precise availability of a promoted class's sections relative to lineage Prestige is open. Do not interpret base label as acquisition before class unlock, or assume both sections are immediately available. Later sections deferred. Each route sums to 30 TP. Exact effects, tags, fallback coverage, caps and comparative value untested.

### Base (1–3 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [1] Health; [1] ATK; [2] Break Power |
| Fork 1 L — Frenzy | [1] Attack Speed; [1] Core finisher damage; [2] Bloodlust gain from completed Core sequences; [3] Rising Fury: Ravager and Bloodrush retain an offensive finisher benefit on the first heavy active after Frenzy begins |
| Fork 1 R — Destruction | [1] Penetration; [1] Heavy skill damage; [2] Directional shockwave coverage; [3] Crushing Advance: Earthshaker and Heavy Cleaver transfer a capped portion of primary-target Armor pressure to enemies in their natural impact path |
| Shared | [1] Energy Recovery; [2] Frenzy heavy-skill damage; [2] Missing-Health Bloodlust generation |
| Fork 2 L — Defiance | [1] Health; [2] Lifesteal; [2] Undying Fury effectiveness; [3] Bloodied Resolve: Unchained reduces interruption for longer while injured, and during Frenzy instead strengthens mitigation for a brief bounded window |
| Fork 2 R — Recklessness | [1] Critical Damage; [2] ATK while injured; [2] Heavy finisher impact; [3] Desperate Force: Rampage and Cataclysm concentrate more of their existing damage against their primary target at low Health, with reduced secondary coverage |
| Conclusion | [1] Energy Efficiency; [2] Break Power; [3] Primal Fury: the first eligible heavy skill during Frenzy receives improved impact or recovery according to its skill definition |

### First expansion (2–6 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [2] ATK; [2] Health |
| Fork 1 L — Frenzy | [3] Bloodlust generation from heavy impacts; [5] Feral Tempo: during Frenzy, eligible Core finishers reduce recovery of the next heavy active without altering its cooldown or granting a free cast |
| Fork 1 R — Destruction | [3] Heavy-impact effectiveness; [5] Fault Line: Earthshaker and Cataclysm convert a capped share of unused area coverage into forward shockwave reach; no additional damage event against the original target |
| Shared | [2] Energy Efficiency; [2] Frenzy skill effectiveness |
| Fork 2 L — Defiance | [4] Undying Fury mitigation effectiveness within its cap; [6] Defiant Heart: while wounded, qualifying heavy skills grant a brief, bounded recovery bonus based on actual direct damage dealt; no proc damage, no recursive healing. Stronger for slow committed impacts, normalized by skill frequency |
| Fork 2 R — Recklessness | [4] Missing-Health heavy-skill damage; [6] All or Nothing: at low Health during Frenzy, designated heavy finishers gain a stronger primary impact at the cost of longer recovery; trade-off and safe auto scheduling explicit |
| Conclusion | [4] Unbroken Rampage: first qualifying heavy skill in Frenzy gains improved ordinary interruption protection; no scripted mechanic immunity |

## Design review / test priorities
- Reference: Riot's Olaf (missing-Health Attack Speed/Lifesteal) https://www.leagueoflegends.com/en-au/champions/olaf/ and Last Epoch Cornered Beast (low-Health mitigation/melee damage) https://support.lastepoch.com/hc/en-us/articles/46363313327387-Primalist-Passive-Tree . Adapt principles, not exact tuning. Black Desert's physical combat presentation and GGM accessibility remain references.
- Main risk: simultaneously multiplying low-Health offense, Frenzy speed, mitigation and Lifesteal can create an immortal DPS or make healing undesirable. Compare effective time-to-kill and survival at high/low Health, sustained and burst damage, solo/party healing, gear scaling and class swap. Preserve Warrior tank advantage and alternate healthy builds. No self-harm requirement.
- Compare sword-only vs greatsword routes; ensure major talents have useful compatible alternatives before finalizing (e.g. Sword-compatible Cataclysm as an alternative to Earthshaker). Explicitly define damage distribution, animation recovery floors, effect snapshots and skill eligibility. Frenzy should alter skill behavior and feedback rather than be a generic red aura.
- Test all four routes in each section for opportunity cost, uptime and proc loops. Avoid double counting the same actual damage in multiple conversions. No numerical simulation or gameplay validation yet. 8 static route-cost checks passed.

## Legendary weapon compatibility (owner direction)
Both Legendary Core choices and both native Legendary ordinary actives work with either class-compatible weapon. Use appropriate weapon or spell choreography without changing the skill's essential role, cooldown identity or creating a hidden equipment requirement. Skill range follows its authored behavior and valid combat geometry. Separate dedicated weapon skills remain weapon-specific; lower starting rarity ordinary skills retain existing restrictions pending further direction. No change to normal class/skill acquisition or inheritance eligibility. Numerical and animation parity still require testing.
