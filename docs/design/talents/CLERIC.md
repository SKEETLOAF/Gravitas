# Cleric lineage talent tree

Status: assistant proposal for owner review, not approved numerical tuning. Canonical shared rules and point economy: [TALENTS](../TALENTS.md); established architecture: [CLASSES](../CLASSES.md), [PROGRESSION](../PROGRESSION.md). Class-exclusive Trait/skills remain in [foundation kit](../classes/CLERIC.md). All effects are intended as modest linear per-effective-rank increments. No node unlocks an ordinary skill or introduces an attribute. Explicitly tagged compatible skills only; no automatic change to all attacks from equipping a lineage.

Healing, protecting and enhancing combat. Support nodes include self where appropriate so solo builds remain viable. No new Healing Power or Shield Power attribute.

## Section 1 — Foundation (50 native TP)
### Restoration (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.1.1.1 | Devout Mind | Attribute | 5 | MATK |
| cleric.1.1.2 | Spiritual Recovery | Attribute | 5 | Energy Recovery |
| cleric.1.1.3 | Healing Practice | Conditional | 4 | Direct ordinary healing coefficient on a valid recipient; excludes overheal shields and secondary proc heals by default |
| cleric.1.1.4 | Reaching Prayer | Transformative | 3 | Range of eligible targeted healing skills within encounter bounds; unchanged target cap |

### Protection (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.1.2.1 | Protective Faith | Attribute | 5 | Maximum HP |
| cleric.1.2.2 | Sacred Defense | Attribute | 5 | MDEF |
| cleric.1.2.3 | Shield Discipline | Conditional | 4 | Shield strength of eligible ordinary protective skills; skill-specific scaling |
| cleric.1.2.4 | Sheltering Reach | Transformative | 3 | Area radius of eligible protective fields; no extra pulse or automatic movement |

### Benediction (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.1.3.1 | Steady Spirit | Attribute | 5 | Critical Resistance |
| cleric.1.3.2 | Lasting Prayer | Attribute | 4 | Effect Duration |
| cleric.1.3.3 | Timely Support | Conditional | 4 | Energy Efficiency briefly after a direct support skill |
| cleric.1.3.4 | Guiding Light | Transformative | 3 | Eligible Light-tagged direct attacks gain modest radius on their existing splash component; no extra element or automatic healing |

## Section 2 — Prestige I (50 native TP)
### Restoration (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.2.1.1 | Restorative Study | Attribute | 5 | MATK |
| cleric.2.1.2 | Renewed Spirit | Attribute | 5 | Energy Recovery |
| cleric.2.1.3 | Urgent Care | Conditional | 4 | Direct ordinary healing bonus against low-Health recipients; self eligible |
| cleric.2.1.4 | Distributed Care | Transformative | 3 | Eligible existing multi-target healing skills retain a little more effectiveness on secondary recipients; no new target or self-bounce |

### Protection (17 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.2.2.1 | Resilient Faith | Attribute | 5 | Resistance |
| cleric.2.2.2 | Blessed Constitution | Attribute | 5 | DEF |
| cleric.2.2.3 | Safe Haven | Conditional | 4 | Block Chance for self while protected by an eligible shield; bounded refresh and no automatic ally conversion |
| cleric.2.2.4 | Lingering Shelter | Transformative | 3 | Duration of eligible protective fields extends modestly, with total pulse healing budget conserved unless a specific skill permits additional pulses |

### Benediction (16 TP)
| Stable node ID | Talent | Type | Ranks | Per-rank effect direction (magnitude TBD) |
| --- | --- | --- | ---: | --- |
| cleric.2.3.1 | Prayer Rhythm | Attribute | 5 | Cooldown Reduction |
| cleric.2.3.2 | Devotional Focus | Attribute | 4 | Energy Efficiency |
| cleric.2.3.3 | Radiant Response | Conditional | 4 | Direct magical damage briefly after effective ordinary healing; self eligible, no overheal trigger |
| cleric.2.3.4 | Benediction Reach | Transformative | 3 | Range of eligible existing ally-targeted buffs increases modestly; no added targets, no extra magnitude or duration |

## Expansion direction (not yet designed)
P II: preparation, cleanse, sustained restoration and offensive support. P III: broader protective and amplification options. Conditional blessings and enemy suppression stay primarily within Oracle/Exorcist kits until those are drafted.

## Verification and dependencies
24 nodes, 100 native investment ranks, 50 per section. First two nodes in a branch proposed open on section access, third/fourth gated by invested branch ranks (5/10; review). All magnitudes, exact conditions, units, event flags and effect caps TBD. At effective ranks above normal investment caps, preserve linear magnitude until explicit safety cap. Do not count bonus effective ranks toward paid prerequisites. Transformative nodes modify a measurable existing component per rank rather than unlocking entire extra actions at rank one. Direct hits, proc hits, status duration, skill geometry, target caps and resource loops require review against existing combat rules. Later sections deferred until their class kits exist.
