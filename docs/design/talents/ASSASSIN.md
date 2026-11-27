# Assassin lineage talent tree

Status: assistant proposal for owner review, not approved numerical tuning. Canonical shared rules and point economy: [TALENTS](../TALENTS.md); established architecture: [CLASSES](../CLASSES.md), [PROGRESSION](../PROGRESSION.md). Class-exclusive Trait/skills remain in [foundation kit](../classes/ASSASSIN.md). All effects are intended as modest linear per-effective-rank increments. No node unlocks an ordinary skill or introduces an attribute. Explicitly tagged compatible skills only; no automatic change to all attacks from equipping a lineage.

Critical offense, avoiding pressure and taking advantage of vulnerable enemies. Avoid requiring stealth, positional backstabs or successful evasion for every offensive node.

## Section 1 — Foundation (50 native TP)
### Precision (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.1.1.1 | Lethal Intent | Attribute | 5 | Critical Chance |
| assassin.1.1.2 | Honed Blades | Attribute | 5 | ATK |
| assassin.1.1.3 | Fine Edge | Attribute | 4 | Critical Damage |
| assassin.1.1.4 | First Opening | Conditional | 3 | Direct damage of first offensive active against a fresh target; per-target cooldown |

### Evasion (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.1.2.1 | Agile Body | Attribute | 5 | Evasion |
| assassin.1.2.2 | Quick Feet | Attribute | 5 | Movement Speed |
| assassin.1.2.3 | Return Step | Transformative | 4 | Eligible evasive attack-and-move skills modestly extend their legal reposition distance; no guaranteed evasion |
| assassin.1.2.4 | Calm Under Pressure | Conditional | 3 | Resistance briefly after successful evasion; refresh |

### Exploitation (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.1.3.1 | Rapid Hands | Attribute | 5 | Attack Speed |
| assassin.1.3.2 | Persistent Wounds | Attribute | 4 | Effect Duration |
| assassin.1.3.3 | Opening Pressure | Conditional | 4 | Direct damage against staggered or Broken enemies |
| assassin.1.3.4 | Finisher Focus | Transformative | 3 | Eligible single-target multi-hit melee finishers shift a small portion of damage from earlier hits to the finishing hit; total nominal output conserved |

## Section 2 — Prestige I (50 native TP)
### Precision (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.2.1.1 | Killer Instinct | Attribute | 5 | Critical Chance |
| assassin.2.1.2 | Deep Cuts | Attribute | 5 | Penetration |
| assassin.2.1.3 | Lethal Opportunity | Conditional | 4 | Critical Damage against Broken enemies |
| assassin.2.1.4 | Precise Burst | Transformative | 3 | Eligible direct multi-hit actives modestly increase final-hit Accuracy; no guaranteed hit or critical |

### Evasion (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.2.2.1 | Slippery Footing | Attribute | 5 | Evasion |
| assassin.2.2.2 | Defensive Awareness | Attribute | 5 | Critical Resistance |
| assassin.2.2.3 | Escape Rhythm | Conditional | 4 | Energy Recovery briefly following successful evasion |
| assassin.2.2.4 | Counter Footwork | Transformative | 3 | Eligible evasive counter skills retain a little more of their defined counter-window duration; bounded and no new counter trigger |

### Exploitation (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| assassin.2.3.1 | Swift Punishment | Attribute | 5 | Attack Speed |
| assassin.2.3.2 | Enduring Effects | Attribute | 4 | Effect Duration |
| assassin.2.3.3 | Wounded Prey | Conditional | 4 | Direct damage against low-Health enemies; no execute bypass |
| assassin.2.3.4 | Surgical Follow-up | Transformative | 3 | Eligible melee finishers against a staggered or Broken enemy gain a small follow-up direct damage component; include it in the original action's hit budget and disable secondary proc triggers |

## Expansion direction (not yet designed)
P II: deceptive tools and rapid melee synergies supported by reusable hooks, not automatic Shinobi-only effects. P III: flexible burst/sustained precision and conditional exploitation. Bleed nodes, if added, depend on ordinary status implementation.

## Verification and dependencies
24 nodes, 100 native investment ranks, 50 per section. First two nodes in a branch proposed open on section access, third/fourth gated by invested branch ranks (5/10; review). All magnitudes, exact conditions, units, event flags and effect caps TBD. At effective ranks above normal investment caps, preserve linear magnitude until explicit safety cap. Do not count bonus effective ranks toward paid prerequisites. Transformative nodes modify a measurable existing component per rank rather than unlocking entire extra actions at rank one. Direct hits, proc hits, status duration, skill geometry, target caps and resource loops require review against existing combat rules. Later sections deferred until their class kits exist.
