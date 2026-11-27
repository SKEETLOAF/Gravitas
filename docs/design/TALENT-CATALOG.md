# Talent catalog

Owner accepted conceptual direction 2026-11-27. Latest class effect drafts below; coefficients, tags, exact per-skill behavior, cooldowns and route balance remain draft. [Canonical architecture](TALENTS.md). No implementation. Each semicolon-separated entry is one node; costs correspond in order. Each fork is independent.

## Warrior
Innate: Block Chance, Break Power. [Kit](classes/WARRIOR.md).

### Prestige 0
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 1, 1, 2 | Health;DEF;Block Chance |
| Fork 1 L | 1, 1, 2, 3 | Aggro;Block effectiveness;defensive skill duration;Ironwall: Shield Bash and Shield Toss grant a brief increased-block window |
| Fork 1 R | 1, 1, 2, 3 | ATK;Core damage;Break Power;Heavy Artillery: heavy impacts concentrate extra Armor damage on primary target |
| Shared | 1, 2, 2 | Resistance;Fighting Spirit generation;Fighting Spirit effectiveness |
| Fork 2 L | 1, 2, 2, 3 | MDEF;protective skill radius;defensive effect duration;Frontline Commander: defensive Battle Cry and Iron Guard share reduced protection with nearby allies |
| Fork 2 R | 1, 2, 2, 3 | Penetration;Core finisher damage;Broken-target damage;Sundering Force: Cleave, Rupture and compatible heavy strikes weaken surviving Armor |
| Conclusion | 1, 2, 3 | Health;DEF/MDEF;Battle Tempered: consuming Fighting Spirit empowers next defensive skill |

### Prestige I
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 2, 2 | DEF/MDEF;Break Power |
| Fork 1 L | 3, 5 | Super Block effectiveness;Iron Reversal: Retaliation converts prevented damage into post-counter protection |
| Fork 1 R | 3, 5 | Heavy impact damage;Siege Engine: capped excess Armor depletion on breaking strike contributes direct damage |
| Shared | 2, 2 | Resistance;Fighting Spirit capacity |
| Fork 2 L | 4, 6 | Defensive skill effectiveness;Bastion of Steel: compatible defensive skills create a short area intercepting limited ally damage |
| Fork 2 R | 4, 6 | Armor-breaking effectiveness;Ruinous Impact: Fighting Spirit-empowered heavy impacts extend directional Armor pressure behind primary target |
| Conclusion | 4 | Veteran's Instinct: maximum Fighting Spirit strengthens applicable defensive or break property of consuming skill |

Review: Prevent recursive interception, repeated Armor weakening and Warmonger conflicts. Preserve Berserker aggression and Knight protection.

## Ranger
Innate: Accuracy, Critical Damage. [Kit](classes/RANGER.md).

### Prestige 0
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 1, 1, 2 | ATK;Accuracy;Critical Damage |
| Fork 1 L | 1, 1, 2, 3 | Penetration;same-target damage;Precision effectiveness;Focused Trajectory: ranged attacks gain Penetration at longer relative distances, smaller close-range benefit |
| Fork 1 R | 1, 1, 2, 3 | Movement Speed;Attack Speed;repositioning effectiveness;Mobile Arsenal: eligible attacks preserve offensive effectiveness during movement transitions |
| Shared | 1, 2, 2 | Energy Recovery;Precision capacity;Core finisher damage |
| Fork 2 L | 1, 2, 2, 3 | Accuracy;projectile travel speed;single-target damage;Pierce and Scatter: penetrating projectiles retain more damage, multi-target volleys widen |
| Fork 2 R | 1, 2, 2, 3 | Evasion;Movement Speed;advancing skill effectiveness;Ranger's Pursuit: Quickdraw, shared lineage starter Flank and eligible approaches retain some Precision on acquiring a target |
| Conclusion | 1, 2, 3 | ATK;Critical Chance;Perfect Release: maximum Precision improves damage and Accuracy without sacrificing secondary coverage |

### Prestige I
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 2, 2 | Accuracy;Attack Speed |
| Fork 1 L | 3, 5 | Same-target damage;Predetermined Shot: empowered projectiles concentrate otherwise wasted coverage on isolated enemies |
| Fork 1 R | 3, 5 | Attack recovery;Running Volley: compatible rapid-fire attacks permit limited repositioning |
| Shared | 2, 2 | Penetration;Precision effectiveness |
| Fork 2 L | 4, 6 | Projectile damage retention;Perfect Trajectory: eligible penetrating projectiles redirect after passing through or defeating target within strict hit limit |
| Fork 2 R | 4, 6 | Repositioning/Core effectiveness;Relentless Hunt: pursuit skills transition to abbreviated Core sequence preserving progress |
| Conclusion | 4 | Instinctive Aim: maximum Precision improves applicable targeting/travel/impact property |

Review: Dagger fallbacks, zone restrictions, no free hits/target cycling. Preserve Hunter traps and Gunslinger firearms.

## Mage
Innate: MATK, Energy Efficiency. [Kit](classes/MAGE.md).

### Prestige 0
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 1, 1, 2 | MATK;Energy;Energy Efficiency |
| Fork 1 L | 1, 1, 2, 3 | Effect Potency;spell damage;Spellweaver effectiveness;Potent Weaving: empowered spells strengthen primary impact and harmful status application |
| Fork 1 R | 1, 1, 2, 3 | Energy Recovery;Core damage;Cooldown Reduction;Efficient Weaving: higher-base-cost empowered spells receive greater capped reductions |
| Shared | 1, 2, 2 | MDEF;Spellweaver capacity;MATK |
| Fork 2 L | 1, 2, 2, 3 | Penetration;area radius;projectile impact;Arcane Geometry: compatible projectiles gain small impact area |
| Fork 2 R | 1, 2, 2, 3 | Effect Duration;persistent spell damage;ward duration;Lingering Script: eligible fields briefly persist at reduced effectiveness |
| Conclusion | 1, 2, 3 | Energy Recovery;spell damage;Arcane Continuity: alternating distinct ordinary spells improves next Core-chain empowerment |

### Prestige I
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 2, 2 | MATK;Energy |
| Fork 1 L | 3, 5 | Empowered spell damage;Greater Invocation: fully empowered spells may spend extra Energy for property-specific impact/area/potency |
| Fork 1 R | 3, 5 | Energy Efficiency;Arcane Economy: bounded Energy saved via Spellweaver contributes next damaging spell effectiveness |
| Shared | 2, 2 | Effect Potency;Penetration |
| Fork 2 L | 4, 6 | Area/projectile effectiveness;Spatial Distortion: eligible area spells concentrate against isolated foes or distribute across groups |
| Fork 2 R | 4, 6 | Persistent effect duration;Spell Inscription: fully empowered spell cast into own magical field reinforces remaining effects without full refresh |
| Conclusion | 4 | Masterful Weaving: fully empowered spells improve primary property (damage/duration/area) |

Review: Bound spend/save order and echo recursion, differentiate Overchannel. Preserve Elementalist reactions and Warlock curses.

## Assassin
Innate: Critical Chance, Evasion. [Kit](classes/ASSASSIN.md).

### Prestige 0
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 1, 1, 2 | ATK;Evasion;Critical Chance |
| Fork 1 L | 1, 1, 2, 3 | Critical Damage;Penetration;Exploit effectiveness;Surgical Precision: empowered single-target strikes gain Penetration against reduced-Health enemies |
| Fork 1 R | 1, 1, 2, 3 | Evasion;Attack Speed;Exploit gain from evasion;Counterstep: evasive skills improve next compatible approach/thrust |
| Shared | 1, 2, 2 | Energy Recovery;Exploit readiness duration;active damage |
| Fork 2 L | 1, 2, 2, 3 | ATK;Broken-target damage;finishing damage;Exposed Anatomy: heavy thrusts/finishers stronger against Broken enemies without extending Break |
| Fork 2 R | 1, 2, 2, 3 | Core damage;Attack Speed;recovery;Flowing Blades: eligible multihit skills preserve Core progress |
| Conclusion | 1, 2, 3 | Critical Damage;Penetration;Ruthless Intent: consuming Exploit readiness empowers next qualifying direct attack at reduced strength |

### Prestige I
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 2, 2 | ATK;Critical Chance |
| Fork 1 L | 3, 5 | Exploit damage;Anatomical Precision: Exploit-empowered single-target strikes improve critical effectiveness and Penetration against vulnerable targets |
| Fork 1 R | 3, 5 | Evasion effectiveness;Phantom Approach: after evasion, advancing attacks gain range and reduced recovery within encounter rules |
| Shared | 2, 2 | Critical Damage;Energy Efficiency |
| Fork 2 L | 4, 6 | Finishing effectiveness;Death Sentence: Deathmark, Severance and compatible finishers gain vulnerability-based finishing properties on activation |
| Fork 2 R | 4, 6 | Core transition effectiveness;Seamless Assault: designated fast actives extend rather than interrupt Core chain, advancing toward finisher |
| Conclusion | 4 | Exploit Mastery: consuming Exploit strengthens applicable finishing or sequence-extension property |

Review: Specify Death Sentence per skill. No guaranteed crits, corpse/mark recursion or free chain loops. Reserve broader combos for Blade Dancer.

## Cleric
Innate: Energy Recovery, ordinary healing effectiveness. [Kit](classes/CLERIC.md).

### Prestige 0
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 1, 1, 2 | MATK;Energy Recovery;healing effectiveness |
| Fork 1 L | 1, 1, 2, 3 | Energy;healing effectiveness;Divine Favor healing empowerment;Compassion: direct healing redistributes capped unused healing to another injured ally |
| Fork 1 R | 1, 1, 2, 3 | MATK;Light damage;offensive Divine Favor;Radiant Force: eligible Light projectiles improve impact against Radiance-afflicted enemies |
| Shared | 1, 2, 2 | MDEF;Energy Efficiency;Divine Favor effectiveness |
| Fork 2 L | 1, 2, 2, 3 | Shield effectiveness;protective area radius;defensive effect duration;Sacred Ground: Sanctuary and compatible areas briefly retain reduced protection on exit |
| Fork 2 R | 1, 2, 2, 3 | Core damage;Effect Potency;Light damage;Divine Exchange: consuming offensive Divine Favor also improves next protective skill |
| Conclusion | 1, 2, 3 | Health;MATK;Divine Reciprocity: alternating empowered restorative/damaging spells improves subsequent Energy Efficiency |

### Prestige I
| Segment | Costs | Talents |
| --- | --- | --- |
| Opening | 2, 2 | MATK;Energy Recovery |
| Fork 1 L | 3, 5 | Healing empowerment;Greater Communion: area heals distribute more restorative potential toward most injured recipients |
| Fork 1 R | 3, 5 | Offensive empowerment;Radiant Geometry: Divine Favor-empowered Light attacks improve secondary-target effectiveness |
| Shared | 2, 2 | Energy Efficiency;Effect Duration |
| Fork 2 L | 4, 6 | Protective effectiveness;Lasting Mercy: targeted heals/protection gain substantially improved protection on critically injured allies, auto prioritizes them |
| Fork 2 R | 4, 6 | Light damage;Sacred Convergence: compatible damaging spells cast into own restorative area reinforce next pulse based on actual damage, capped |
| Conclusion | 4 | Divine Harmony: consuming both Divine Favor forms successively improves next applicable restorative/damaging property |

Review: Self fallback, no recursive healing or multiplication with party size, clarify manual target override and Overflowing Grace. Preserve Oracle and Exorcist.

## Universal catalog
Six original trees retained. Warfare is latest full example; other five preserve earlier linear layouts with candidate skill-mod substitutions reflecting final owner direction. Exact substitutions and coefficients are assistant proposals, not separately approved. Influence candidate seventh tree. No forks. Compatibility tags, not exclusive class Traits.

### Foundation
Innate: Health, Energy.
- P0: [1] Health → [1] Energy → [2] DEF → [3] Constitution: max Health → [1] MDEF → [2] Health → [2] Energy → [3] Reinforced Casting: eligible long-casting skills grant Resistance during activation → [1] DEF → [2] MDEF → [2] Health → [3] Structural Integrity: DEF/MDEF → [1] Energy → [1] Health → [2] Critical Defense → [3] Fortitude: max Health/Energy.
- PI: [2] Health → [2] Energy → [3] DEF/MDEF → [4] Greater Constitution: max Health → [2] Health → [3] Critical Defense → [3] Resistance → [5] Structural Reinforcement: bounded DEF/MDEF cross-contribution without recursion → [6] Perfect Physique: bounded defense-based Health scaling, eligible protective skills use portion of base Health (candidate).

### Warfare
Innate: ATK, MATK.
- P0: [1] Physical Strength: ATK → [1] Magical Strength: MATK → [2] Piercing Force: Penetration → [3] Forceful Impact: damaging skills inflict extra Armor depletion → [1] Offensive Training: Core damage → [2] Battle Proficiency: ordinary active damage → [2] Concentrated Force: Break Power → [3] Broad Assault: compatible area radius → [1] Combat Precision: Accuracy → [2] Destructive Force: ATK/MATK → [2] Armor Exploitation: Broken-target damage → [3] Follow Through: penetrating/sweeping attacks lose less damage on subsequent targets → [1] Battle Instinct: Critical Damage → [1] Armament: Penetration → [2] Overwhelming Strength: direct damage → [3] Domination: Armor-breaking skills temporarily improve offensive effectiveness.
- PI: [2] Greater Strength: ATK → [2] Greater Intellect: MATK → [3] Siegecraft: Break Power → [4] Expansive Force: area skills stronger near impact center → [2] Piercing Mastery: Penetration → [3] Destruction: ordinary active damage → [3] Exploit Armor: Broken-target damage → [5] Concentrated Impact: area skills concentrate more damage on isolated targets → [6] Devastation: capped excess Armor depletion converts to direct damage.

### Tempo
Innate: Attack Speed.
- P0: [1] Attack Speed → [1] Movement Speed → [2] Cooldown Reduction → [3] Acceleration: Attack Speed in sustained combat → [1] Movement Speed → [2] Attack Speed → [2] Cooldown Reduction → [3] Quickening: movement bonus above Attack Speed threshold → [1] Attack Speed → [2] Cooldown Reduction → [2] Movement Speed → [3] Rhythm: Attack Speed when ordinary actives cooling down → [1] Attack Speed → [1] Movement Speed → [2] Cooldown Reduction → [3] Momentum: eligible skill recovery shortened within animation floors (candidate).
- PI: [2] Attack Speed → [2] Movement Speed → [3] Cooldown Reduction → [4] Greater Acceleration: sustained-combat speed → [2] Movement Speed → [3] Attack Speed → [3] Cooldown Reduction → [5] Synchronization: bounded Attack Speed contribution to Cooldown Reduction → [6] Accelerated Recovery: eligible long-cooldown skills benefit more from recovery, enforce floor (candidate).

### Flow
Innate: Energy Recovery.
- P0: [1] Energy → [1] Energy Recovery → [2] Energy Efficiency → [3] Expanded Reserves: max Energy → [1] Energy Recovery → [2] Energy → [2] Energy Efficiency → [3] Conservation: efficiency at low reserves → [1] Energy → [2] Energy Recovery → [2] Energy Efficiency → [3] Replenishment: recovery at low reserves → [1] Energy Recovery → [1] Energy → [2] Energy Efficiency → [3] Heavy Investment: bounded skill effectiveness from actual Energy expenditure (candidate).
- PI: [2] Energy → [2] Energy Recovery → [3] Energy Efficiency → [4] Greater Reserves: max Energy → [2] Energy Recovery → [3] Energy Efficiency → [3] Energy → [5] Wellspring: capped maximum Energy contribution to recovery → [6] Excess Recovery: capped otherwise wasted Energy recovery empowers next paid skill (candidate).

### Endurance
Innate: Resistance, Health Regeneration.
- P0: [1] Health Regeneration → [1] Lifesteal → [2] Resistance → [3] Recovery: regeneration in combat → [1] Block Chance → [2] Health Regeneration → [2] Critical Resistance → [3] Survival Instinct: Resistance at low Health → [1] Evasion → [2] Lifesteal → [2] Health Regeneration → [3] Fighting Recovery: Lifesteal at low Health → [1] Resistance → [1] Critical Defense → [2] Health Regeneration → [3] Lasting Protection: shields retain limited protection against depleting hit (candidate).
- PI: [2] Health Regeneration → [2] Resistance → [3] Lifesteal → [4] Greater Recovery: regeneration while injured → [2] Critical Resistance → [3] Critical Defense → [3] Health Regeneration → [5] Second Wind: actual substantial healing temporarily improves Resistance (candidate) → [6] Unbroken: bounded Resistance/recovery rise with missing Health.

### Opportunity
Innate: Critical Chance, Accuracy.
- P0: [1] Accuracy → [1] Critical Chance → [2] Critical Damage → [3] Precision: Accuracy → [1] Critical Chance → [2] Critical Damage → [2] Accuracy → [3] Exploitation: Critical Damage against afflicted enemies → [1] Accuracy → [2] Critical Chance → [2] Penetration → [3] Vulnerability: Critical Chance against Broken foes → [1] Accuracy → [1] Critical Chance → [2] Critical Damage → [3] Critical Momentum: Super Crit briefly improves Attack Speed (candidate).
- PI: [2] Accuracy → [2] Critical Chance → [3] Critical Damage → [4] Greater Precision: Accuracy scaling → [2] Penetration → [3] Critical Chance → [3] Critical Damage → [5] Calculated Strike: bounded Accuracy contribution to Critical Damage → [6] Perfect Opening: damaging skills gain stronger conditional critical bonuses against targets meeting multiple vulnerability conditions.

### Influence (candidate)
Effect Potency/Duration, status and support, persistent skill properties, Lingering Presence (persistent effects last longer), Cascading Affliction (eligible harmful status spreads at reduced potency on defeat, capped and nonrecursive). Full sections and roster inclusion open.

## Validation
Static cost arithmetic checked: 40 class routes and 12 universal sections, each 30 TP. No gameplay tests. Resolve compatibility registry, modifier order and derived tags (e.g. Mage Arcane Geometry area then Warfare Broad Assault only if explicitly supported), active-class/persistent scope, cooldown/refund floors, binary stacking, actual resource expenditure and missing Health, tooltip clarity, no recursive statuses/heals/hits. Major talents must justify opportunity cost in manual/auto, solo/co-op, farming/bossing. Vague property modifiers need per-skill definitions before implementation.

Pre-PII audit clarification: Assassin Exploit is bounded readiness, not a confirmed multi-stack meter; these nodes modify readiness duration/payoff, not capacity. Mage Spellweaver explicitly permits additional Core chains up to a cap; exact cap still open. Ranger Flank is a shared lineage starter. Cleric talent renamed Lasting Mercy to avoid confusion with Oracle's Legendary Divine Intervention. Promotion talent sections are in their individual class documents. See [pre-PII audit](PRESTIGE-I-AUDIT.md).
