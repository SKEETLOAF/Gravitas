# Elements, reactions and cosmic catalysts
2026-11-26 | Owner concept and recommended refinement; individual mechanics and tuning exploratory.

## Owner direction
The owner proposed Fire, Water, Earth, Resonance (Wind or Sound), Cold, Lightning, Necrotic, Force (Gravity), Light and Dark. Light and Dark add universal Radiance/Corruption modifiers to other elements; Force similarly affects elements but occupies a beyond-core, neutral median between Light and Dark, encompassing gravity, space and kinetics. Owner supplied a nine-element alternative merging Necrotic into Dark and partially conflating Resonance with Force, a 3x3 reaction matrix, four cosmic reactions, and suggested blended VFX/gradients. Owner asks to refine, not unconditionally finalize every suggestion.
Recommended taxonomy: retain all ten original named elements, with six core (Fire, Water, Earth, Resonance, Cold, Lightning), Necrotic as specialized attrition, and Light/Force/Dark as cosmic catalysts. Resonance covers vibrations, sound and wind pressure; Force covers gravity, spatial distortion and kinetic manipulation. Necrotic covers decay/vitality, not synonymous with Dark corruption. Cosmic versatility does not imply automatic damage superiority. Primer/reactor categories describe tendencies, not mandatory application order. Exact classification and individual mechanics pending owner confirmation.

## Elemental effects (candidates)
| Element | Status | Identity |
| --- | --- | --- |
| Fire | Burn | periodic damage, sustained pressure |
| Water | Soaked | prepares reactions; water also supports healing/utility |
| Earth | Fracture | susceptibility to posture damage; stagger remains universal |
| Resonance | Reverberation | lingering vibrations, secondary impact/reaction opportunities |
| Cold | Chill | movement/action slow; freezing via reaction |
| Lightning | Shock | electrical instability and additional discharge; not automatic hard stun |
| Necrotic | Decay | vitality deterioration, potential anti-heal/life absorption |
| Light | Radiance | universal luminous modification, potential ally protection/cleanse |
| Dark | Corruption | universal corrupting modification, potential offensive attrition |
| Force | Distortion | universal spatial modification, grouping/displacement |
Damage type, element, status application, and reaction are separate concepts. Not every elemental hit must apply a status. Healing, shields, movement and buffs need not be exclusive to any element.

## Primary core reaction matrix (recommended nine; names from owner)
| Primer / Reactor | Resonance | Cold | Lightning |
| --- | --- | --- | --- |
| Fire | Wildfire: spread Burn | Thermal Shock: burst and posture damage | Overload: explosive impact/displacement |
| Water | Tempest: grouping, recurring field damage | Freeze: ordinary enemy disable, boss break contribution | Electro-Charge: recurring chain damage |
| Earth | Sandstorm: offensive/targeting debuff | Shatter: physical defense/posture vulnerability | Magnetize: movement disruption/posture pressure, possible interrupt |
Recommend either order triggers when eligible statuses exist. These are tactical effects, not exact coefficients or guaranteed durations. Distinguish Tempest (sustained wind/water field) from Collapse (gravity compression and spread). Avoid incessant scatter or hard stun.

## Optional expansion (not initial scope)
Same-category pairs: Fire+Water Steam (obscuring field); Fire+Earth Molten (ground damage); Water+Earth Mire (slow); Resonance+Cold Blizzard (spread Chill); Resonance+Lightning Thunderclap (area impact/interrupt); Cold+Lightning Superconduction (damage susceptibility).
Necrotic candidates: Fire+Necrotic Wither (accelerated attrition); Water+Necrotic Blight (spread Decay); Cold+Necrotic Mortification (recovery suppression). No requirement every pair react. Unlisted pairs may coexist without a named reaction.

## Cosmic modifiers and reactions (recommended distinction)
Infusion is an intentional ability/equipment modifier to a base element, not a new element or mandatory reaction. Radiant Fire, Corrupted Fire, Distorted Fire reuse base Fire mechanics with a consistent cosmic overlay; the same universal rule can be applied across all seven ordinary/specialized elements. Candidate common rules: Radiance creates a bounded protective/healing benefit on successful application, Corruption adds a bounded lingering damage component, Distortion nudges targets toward an impact center or adds posture pressure against displacement-resistant targets. Exact effects and targeting pending; distinguish Radiance/Corruption from Necrotic anti-heal, and separate Force from Resonance.
Reaction is a discrete encounter event when a qualifying elemental application meets an existing status. Candidate cosmic rules:
- Force + any of seven noncosmic elements = Collapse: compress nearby enemies, spread a reduced copy or amplify a selected active status once; boss substitute posture damage.
- Force + Light = Nova: outward radiant pulse, potential ally cleanse, enemy posture damage/displacement.
- Force + Dark = Singularity: inward crushing well, sustained pressure/slow; no automatic true damage or universal cooldown suppression recommended.
- Light + Dark = Eclipse: opposed energies detonate, strong burst or posture damage; no default defense bypass.
- Light/Dark + ordinary elemental effects can use the same Radiance/Corruption modifier rules rather than seven separate named pair reactions. Whether triggered on contact or specifically imbued is an open implementation choice; avoid automatically conflating infusion with reaction. Limit to one cosmic infusion per ability as a candidate; multi-cosmic combinations possible explicit abilities only. No 3+ element bespoke matrix.
Force is neutral, not a moral alignment or default stronger element.

## Reaction rules and test questions
- Apply eligible elemental status, then evaluate one reaction per application using deterministic priority; reaction-generated secondary damage cannot recursively trigger other reactions by default. Existing statuses can coexist; consume/refresh/attenuate participating status as defined per reaction, not blanket removal. Define per-target/source ICD, stack cap, duration/ticks, scaling, ownership, assist credit and immunity.
- Cross-class and co-op elemental primers persist across swap when allowed; automated rotations recognize existing statuses without requiring manual timing. Shared per-target reaction protection avoids multiplayer chain explosions and permanent CC. Bosses replace hard CC/displacement with break/posture contribution where appropriate; ordinary enemies may be fully controlled briefly. No automatic true damage, indefinite freeze, or permanent lockdown.
- Decide source scaling, crit eligibility, reward credit and damage cap; avoid double scaling and multiplying all status effects indiscriminately.
- Keep ability element and reaction tags distinct from physical/magical damage, buff/debuff, status and equipment stat systems. Single-element and non-elemental builds should remain viable.
- Recommended first prototype: 6 core effects, 9 core reactions, then cosmic overlays and four cosmic reaction rules, Necrotic distinct status and limited reactions as scope permits. Order is a recommendation, not launch commitment.

## Presentation and technical asset strategy
Owner favors combining existing elemental VFX or gradient colors. Reuse a base effect's silhouette, timing and motion with a secondary accent (palette/gradient), shared reaction shape (burst, field, chain, pull, shatter) and cosmic overlay (Radiance halo/rays, Corruption dark veins/particles, Distortion lens/rings/compression). Do not rely on color alone: distinct silhouettes, direction, audio and status icons for readability. Distinguish Force compression from Resonance oscillation. Shared modular VFX templates, pooled particles/emitters, capped effects per target, simplified effects for remote players/mobile, reduced flashes; avoid stacking every full emitter for each combination. Keep reaction names and icons distinct; optional damage/FX settings. No finished art or code.

## Additional progression directions (owner confirmed existence)
- Relics: unique upgrades. Candidate build-defining effects: alter status/reaction, class swap behavior, resource or defense. Slot count, equip rules, acquisition and upgrades open; avoid duplicating ordinary equipment affixes or mandatory relics for element functionality.
- Mounts and pets: both available from the start, each has one usable skill; pets also have their own basic attacks. Mounts primarily enhance the character. Pet generations improve with class progression plus high character level; mounts more universal; potential pet ascension using another pet and resources. See [SKILLS-AND-COLLECTION.md](SKILLS-AND-COLLECTION.md) for the current direction. Exact gates, slots, stats and skill behavior remain open. Preserve one-character focus. No named mount/pet, numerical bonus or rarity system confirmed.


## Closure proposal (2026-11-26)
Owner requests closing explored systems before opening equipment itemization or other new branches. Candidate final interaction rules: different statuses coexist; periodic effects such as Burn/Bleed/Poison/Decay may stack intensity with caps; ordinary stat debuffs refresh or retain stronger application; control effects have resistance/diminishing returns. Both application orders can react, with per-reaction consumption/refresh and short per-target reaction protection. Applied statuses persist through class swaps; party members and pets can contribute and trigger reactions; resistant bosses substitute posture/stagger for hard CC/displacement. Cosmic infusions retain universal behavior. No universal elemental weakness wheel recommended, only encounter-specific resistance/vulnerability. Exact durations, caps, scaling and reaction coefficients deferred to tuning. These are closure proposals awaiting owner approval, not new confirmed mechanics.

## Owner refinement (2026-11-26)
Supersedes earlier order-independent and per-target reaction cooldown proposals. Primer-dependent reactions require the primer first; reactor+reactor pairs work in either order; cosmic effects may stack in any order. Repeated reactions have no general cooldown. Repeated control effects instead use diminishing returns or a recovery/immunity interval before building back to full control; per-control-family resistance is a recommendation, exact implementation open. Distinguish no general reaction cooldown from preventing reaction-generated damage from recursively chaining without bound (earlier recommendation remains open). Cosmic stacking limits, primer consumption, exact status caps and control recovery values are not finalized.

## Owner approval and final conceptual rules (2026-11-26)
Owner approves remaining refinement recommendations with the following specifics. DoTs stack; no universal fixed stack cap is established. Application, scaling, stack decay and potential ceilings are determined by individual effects, skills, weapons and build modifiers; ceilings may be raised by build investments. Stacks diminish over time. Buffs refresh and retain stronger effects; ordinary debuff refresh/stronger retention recommendation accepted. Reactions transform and consume participating elemental statuses; exact quantities consumed and resulting effect behavior are reaction-specific implementation details. Primer-first applies where required, reactor pairs any order, cosmic effects stack any order, no universal reaction cooldown, CC diminishing returns or recovery windows. Enemy-specific elemental resistance rather than universal type wheel approved. Prior contrary proposals superseded. Conceptual refinement complete; numerical tuning and exact per-effect rules deferred.
