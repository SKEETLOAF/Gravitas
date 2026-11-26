# Elements, reactions and statuses
Updated 2026-11-26. Conceptual interaction rules established; individual reaction behavior and tuning remain open.

## Element working roster
Ten elements. Six core, one specialized (Necrotic), three cosmic (Light, Force, Dark). Resonance covers wind/sound/vibration; Force covers gravity, space and kinetics. Necrotic is vitality/decay, distinct from Dark corruption. Exact individual effects below are design candidates.
| Element | Status | Identity |
| --- | --- | --- |
| Fire | Burn | DoT and sustained pressure |
| Water | Soaked | Prepares reactions; healing/utility possible |
| Earth | Fracture | Structural/Armor pressure |
| Resonance | Reverberation | Vibration, secondary impacts |
| Cold | Chill | Slow, freezing reactions |
| Lightning | Shock | Electrical instability/discharges |
| Necrotic | Decay | Attrition, potential anti-heal/life absorption |
| Light | Radiance | Universal luminous modifier |
| Dark | Corruption | Universal corrupting modifier |
| Force | Distortion | Universal spatial modifier |
Damage type, element, status and reaction are distinct. No universal elemental weakness chart; individual enemies can have resistances/weaknesses.

## Core reactions (working matrix)
Primer-dependent reactions require the primer first. Reactor+reactor works either order.
| Primer / Reactor | Resonance | Cold | Lightning |
| --- | --- | --- | --- |
| Fire | Wildfire: spread Burn | Thermal Shock: burst/break | Overload: explosive impact/displacement |
| Water | Tempest: grouping field | Freeze: disable | Electro-Charge: recurring chain damage |
| Earth | Sandstorm: offensive debuff | Shatter: defense/armor vulnerability | Magnetize: movement disruption/break |
Additional candidates: Steam (Fire+Water), Molten (Fire+Earth), Mire (Water+Earth), Blizzard (Resonance+Cold), Thunderclap (Resonance+Lightning), Superconduction (Cold+Lightning), Wither (Necrotic+Fire), Blight (Necrotic+Water), Mortification (Necrotic+Cold). No requirement every pair reacts.

## Cosmic effects
Light and Dark apply universal Radiance and Corruption; Force similarly adds Distortion, a neutral cosmic median, not inherently superior damage. Infusions can modify base elements; cosmic effects stack in any order. Suggested consistent effects: Radiance protective/restorative, Corruption offensive lingering pressure, Distortion grouping/spatial impact.
| Reaction | Candidate behavior |
| --- | --- |
| Force + noncosmic = Collapse | Compress targets and spread/amplify elemental effect |
| Force + Light = Nova | Outward radiant pulse, disruption, possible purification |
| Force + Dark = Singularity | Crushing well, sustained damage/slow |
| Light + Dark = Eclipse | Concentrated burst/break |
No automatic true damage or defense bypass recommended. Distinguish infusion from discrete reaction; no bespoke three-element matrix necessary.

## Interaction rules
- Different statuses coexist. Reactions transform and consume participating effects; quantities and resulting effects vary by reaction. Primer-first where required, reactor pairs either order, cosmic effects any order. No universal repeated-reaction cooldown.
- DoT stacks diminish over time; application, scaling, decay and potential ceiling depend on effect, skill, weapon and build. No universal stack limit; ceilings can be raised.
- Same-source buff/debuff reapplication refreshes, with stronger application retained. Owner wants independent modifiers to stack multiplicatively; cap proposal below.
- CC has diminishing returns or recovery interval before full control can be rebuilt. Resistant bosses may convert control into Armor/Break pressure as appropriate. See [Combat](COMBAT-FOUNDATIONS.md).
- Statuses persist across class swaps; party members and pets may contribute to reactions. Automation supports reaction opportunities. Recommend bounded reaction processing to avoid recursion, not a general cooldown. Single-element and non-elemental builds should remain viable.
- Ordinary status candidates: Bleed, Poison, Burn, Decay; Slow, Weaken, Vulnerable, Sunder; Stun, Root, Silence, Freeze; displacement/knockdown/launch as reactions; Haste, Fortify, Regeneration, Barrier, Empower, Immunity; Cleanse and Dispel. Marks, taunt, anti-heal etc. optional. Exact catalog and effect math open.

## Temporary modifier cap (under review)
Owner favors cap relative to passive stats (base, equipment, permanent/unconditional bonuses), excluding skill coefficients. Recommended +100% ordinary positive temporary modifiers and -50% enemy stat reduction per affected stat, independent eligible effects multiply; same-source refresh. Positive multiplier min(product(1+b),2); negative max(product(1-d),0.5). Exact +50 vs +100% buff cap not confirmed. Raw stat overflow, DoT and CC independent; skill scaling excluded. Chance, speed, cooldown and damage amplification may need specialized rules. No strongest-buff-dependent cap in current proposal.

## Presentation
Reuse base elemental effects, secondary gradients/accents, shared burst/chain/field/pull/shatter templates and cosmic overlays. Distinct silhouettes, motion, sound and icons rather than color alone. Mobile-friendly pooling, effect caps and simplified remote VFX recommended.
