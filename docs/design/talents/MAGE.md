# Mage lineage talent tree

Status: assistant proposal for owner review, not approved numerical tuning. Canonical shared rules and point economy: [TALENTS](../TALENTS.md); established architecture: [CLASSES](../CLASSES.md), [PROGRESSION](../PROGRESSION.md). Class-exclusive Trait/skills remain in [foundation kit](../classes/MAGE.md). All effects are intended as modest linear per-effective-rank increments. No node unlocks an ordinary skill or introduces an attribute. Explicitly tagged compatible skills only; no automatic change to all attacks from equipping a lineage.

Direct magic, elemental/status reliability and casting economy. Supports neutral magical builds as well as reactions, without requiring the future Elementalist's specialized loop.

## Section 1 — Foundation (50 native TP)
### Arcane Mastery (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.1.1.1 | Arcane Study | Attribute | 5 | MATK |
| mage.1.1.2 | Deep Wells | Attribute | 5 | Maximum Energy |
| mage.1.1.3 | Spell Focus | Attribute | 4 | Effect Potency |
| mage.1.1.4 | Focused Casting | Conditional | 3 | Direct magical damage of next ordinary active following a completed Core chain |

### Elemental Control (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.1.2.1 | Elemental Study | Attribute | 5 | Effect Duration |
| mage.1.2.2 | Arcane Stability | Attribute | 5 | Resistance |
| mage.1.2.3 | Elemental Reach | Transformative | 4 | Area radius of eligible elemental area spells; no added targets beyond defined cap |
| mage.1.2.4 | Lingering Embers | Conditional | 3 | Magnitude of eligible damage-over-time effects applied by ordinary spells, not reaction output |

### Spellcraft (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.1.3.1 | Efficient Mind | Attribute | 5 | Energy Efficiency |
| mage.1.3.2 | Quick Incantation | Attribute | 4 | Cooldown Reduction |
| mage.1.3.3 | Recovery Cycle | Conditional | 4 | Energy Recovery briefly after completing a Core chain |
| mage.1.3.4 | Measured Casting | Transformative | 3 | Shift a small portion of eligible delayed-damage spell output from delayed impact to initial impact, preserving total nominal damage |

## Section 2 — Prestige I (50 native TP)
### Arcane Mastery (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.2.1.1 | Greater Arcana | Attribute | 5 | MATK |
| mage.2.1.2 | Expanded Reserve | Attribute | 5 | Maximum Energy |
| mage.2.1.3 | Arcane Precision | Conditional | 4 | Penetration for direct magical skills |
| mage.2.1.4 | Overtone | Transformative | 3 | Neutral magical area attacks gain modest falloff retention toward the edge of their defined area; no new elemental tag |

### Elemental Control (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.2.2.1 | Elemental Fluency | Attribute | 5 | Effect Potency |
| mage.2.2.2 | Persistent Magic | Attribute | 5 | Effect Duration |
| mage.2.2.3 | Reaction Readiness | Conditional | 4 | Direct damage of an elemental spell against a target already carrying a compatible primer, whether or not a reaction succeeds; no recursive trigger |
| mage.2.2.4 | Status Pressure | Transformative | 3 | Eligible status-applying damaging spells contribute a small additional Armor-depletion component when the intended control is rejected by intact Armor; no forced control |

### Spellcraft (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| mage.2.3.1 | Mana Discipline | Attribute | 5 | Energy Recovery |
| mage.2.3.2 | Efficient Sequence | Attribute | 4 | Energy Efficiency |
| mage.2.3.3 | Casting Rhythm | Conditional | 4 | Cooldown Reduction briefly after using distinct ordinary skills in sequence; bounded refresh |
| mage.2.3.4 | Stabilized Channel | Transformative | 3 | Eligible multi-hit channeled spells deliver a small portion of their later damage earlier, preserving total nominal damage and recovery; no free recast |

## Expansion direction (not yet designed)
P II: sustained spell cadence, duration and efficient elemental/magical output. P III: deeper elemental specialization, conditional efficiency and spell geometry. Reserve reaction alteration and affliction detonation for actual promotion kits and reviewed transforms.

## Verification and dependencies
24 nodes, 100 native investment ranks, 50 per section. First two nodes in a branch proposed open on section access, third/fourth gated by invested branch ranks (5/10; review). All magnitudes, exact conditions, units, event flags and effect caps TBD. At effective ranks above normal investment caps, preserve linear magnitude until explicit safety cap. Do not count bonus effective ranks toward paid prerequisites. Transformative nodes modify a measurable existing component per rank rather than unlocking entire extra actions at rank one. Direct hits, proc hits, status duration, skill geometry, target caps and resource loops require review against existing combat rules. Later sections deferred until their class kits exist.
