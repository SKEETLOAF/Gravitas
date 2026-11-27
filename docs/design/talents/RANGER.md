# Ranger lineage talent tree

Status: assistant proposal for owner review, not approved numerical tuning. Canonical shared rules and point economy: [TALENTS](../TALENTS.md); established architecture: [CLASSES](../CLASSES.md), [PROGRESSION](../PROGRESSION.md). Class-exclusive Trait/skills remain in [foundation kit](../classes/RANGER.md). All effects are intended as modest linear per-effective-rank increments. No node unlocks an ordinary skill or introduces an attribute. Explicitly tagged compatible skills only; no automatic change to all attacks from equipping a lineage.

Accurate direct attacks, projectile pressure and position management. Melee-compatible general precision nodes remain useful; projectile-only nodes are explicit choices, not compulsory.

## Section 1 — Foundation (50 native TP)
### Marksmanship (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.1.1.1 | Keen Sight | Attribute | 5 | Accuracy |
| ranger.1.1.2 | Piercing Aim | Attribute | 5 | Penetration |
| ranger.1.1.3 | Steady Hand | Attribute | 4 | Critical Damage |
| ranger.1.1.4 | Patient Aim | Conditional | 3 | First direct damaging active after a complete Core chain gains modest Accuracy |

### Barrage (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.1.2.1 | Swift Release | Attribute | 5 | Attack Speed |
| ranger.1.2.2 | Drawing Strength | Attribute | 5 | ATK |
| ranger.1.2.3 | Spread Control | Transformative | 4 | Eligible projectile area attacks gain a small coverage-radius bonus; unchanged single-target coefficient |
| ranger.1.2.4 | Target Focus | Conditional | 3 | Direct Core damage on consecutive hits to the same enemy, capped progress per action |

### Mobility (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.1.3.1 | Light Stride | Attribute | 5 | Movement Speed |
| ranger.1.3.2 | Evasive Instinct | Attribute | 4 | Evasion |
| ranger.1.3.3 | Economical Motion | Conditional | 4 | Energy Efficiency briefly after valid skill-driven reposition |
| ranger.1.3.4 | Passing Shot | Transformative | 3 | Eligible attack-and-reposition skills modestly increase their displacement distance within legal geometry; no mandatory move or zone override |

## Section 2 — Prestige I (50 native TP)
### Marksmanship (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.2.1.1 | True Aim | Attribute | 5 | Accuracy |
| ranger.2.1.2 | Deep Penetration | Attribute | 5 | Penetration |
| ranger.2.1.3 | Distance Discipline | Conditional | 4 | Direct ranged damage scales modestly with normalized valid attack distance; no bonus beyond usable range |
| ranger.2.1.4 | Piercing Line | Transformative | 3 | Eligible piercing projectile skills retain a little more damage on secondary hits; capped at first-hit coefficient |

### Barrage (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.2.2.1 | Rapid Volley | Attribute | 5 | Attack Speed |
| ranger.2.2.2 | Powerful Draw | Attribute | 5 | ATK |
| ranger.2.2.3 | Volley Economy | Conditional | 4 | Energy Efficiency of multi-hit direct actives; evaluated once per cast |
| ranger.2.2.4 | Concentrated Impact | Transformative | 3 | A small portion of damage in eligible multi-hit area projectile attacks shifts to the primary target; total nominal budget conserved, no penalty against isolated target |

### Mobility (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| ranger.2.3.1 | Fleetness | Attribute | 5 | Movement Speed |
| ranger.2.3.2 | Alertness | Attribute | 4 | Critical Resistance |
| ranger.2.3.3 | Reset Footing | Conditional | 4 | Accuracy briefly after a valid reposition; refresh |
| ranger.2.3.4 | Pursuit Range | Transformative | 3 | Eligible offensive gap-closing skills gain a small approach-range bonus within weapon and arena restrictions |

## Expansion direction (not yet designed)
P II: sustained projectile execution, target switching and weapon handling (including Firearms when applicable). P III: flexible precision/area trade-offs and mobility mastery. Keep Hunter-specific traps and Gunslinger-specific weapon mechanics in their kits.

## Verification and dependencies
24 nodes, 100 native investment ranks, 50 per section. First two nodes in a branch proposed open on section access, third/fourth gated by invested branch ranks (5/10; review). All magnitudes, exact conditions, units, event flags and effect caps TBD. At effective ranks above normal investment caps, preserve linear magnitude until explicit safety cap. Do not count bonus effective ranks toward paid prerequisites. Transformative nodes modify a measurable existing component per rank rather than unlocking entire extra actions at rank one. Direct hits, proc hits, status duration, skill geometry, target caps and resource loops require review against existing combat rules. Later sections deferred until their class kits exist.
