# Gravitas — design learning notes

Purpose: preserve reusable lessons from critique, comparison, design iteration and eventual playtesting. This is a living synthesis, not a chronological changelog or replacement for canonical specifications. Keep entries concise; distinguish observed owner preferences, design hypotheses and validated results. Consolidate repeated lessons as they evolve. Git history preserves discarded drafts.

## Class and skill design

### Passive skills should change play, not merely inflate numbers
Owner-preferred direction, learned during Warrior design (2026-11-27).
- Individual Class Traits establish a discipline's defining loop. Collectible passive skills supply conditional effects, triggered abilities and skill transformations that create build choices. Talent nodes provide incremental development and deeper specialization; they may also transform mechanics where appropriate.
- A passive can change an active skill's function with a real trade-off (Warrior Warmonger transforms Battle Cry from tanking to aggression). Avoid making every passive mandatory for the same build.
- Starter lineage passives can be simpler; mix accessible stat bonuses with meaningful combat interactions. Preserve useful inherited options across descendants with different playstyles.
- Higher starting skill rarity retains intrinsic power advantages; build synergy can let an evolved lower-origin skill outperform it situationally. Keep rarity meaningful without making all investment obsolete.

### Design around existing combat events
Working design principles from Warrior iteration:
- Use existing Block/Super Block, prevented damage, Armor break, basic-chain completion/extension, Impulse, weapon/class switches, Energy and status effects as hooks. Avoid adding new resource meters by default.
- Distinguish block count from damage actually prevented by Block. Exclude unrelated mitigation; normalize conversions to appropriate player scaling and bound proc output. Avoid recursive counter/shockwave triggers, duplicated damage-conversion exploits and runaway Energy loops.
- Give defensive skills and passives reasonable baseline value in ordinary automation. A counter should still act if no incoming hit arrives during its stance; tank passives should not go dead in single-target bosses; Armor-break builds need deliberate value during Broken windows and appropriate handling of unarmored enemies.
- Differentiate mechanically similar skills rather than piling overlapping triggers on the same mandatory rotation.
- Keep optional active play rewarding without requiring manual parry timing for baseline class functionality.

### Review future kits through these questions
Does the class have a distinct loop? Do passives enable different builds and interact with real combat mechanics? Is an inherited skill useful outside its original class? Does auto-combat handle its conditions reliably? Are there sensible boss, single-target, multi-target and unarmored use cases? Are stronger rarity skills rewarding? What happens at extreme stat values and when effects overlap? These are review prompts, not mandatory new mechanics.

### Lessons from designing the remaining foundation kits
Assistant-derived working design hypotheses, not playtest conclusions (2026-11-27):
- Separate a class's loop from its descendants' specialties: Ranger direct precision vs Hunter prey/traps; Mage spell cadence vs Elementalist reaction manipulation; Assassin burst openings vs Shinobi deception and Blade Dancer sustained combos; Cleric immediate restoration vs Oracle conditional blessings and Sage amplification.
- Two Core skills should change attack rhythm and payoff while reusing weapon-family animation foundations. Don't imply new range, weapon compatibility or elemental tags solely from skill names/VFX.
- Build skill transformations with explicit trade-offs (area versus focus, upfront versus delayed damage, shield size versus Critical Resistance). Let baseline skills operate without required passive combinations.
- Design valid fallback targets and baseline effects for solo/party, armored/unarmored, resistant, short-lived and single-target enemies. A heal needs a valid recipient, an evasive build needs some opportunity even while a tank holds Aggro, and chained attacks cannot self-bounce indefinitely.
- Keep effect ownership explicit: direct hits versus secondary/proc hits, actual damage versus overkill, actual healing versus overheal, cooldown/charge ownership, bounded conversions and per-action normalization. No recursive mark, echo, healing or Energy loops.
- Treat unconfirmed status implementations (e.g., Bleed) as dependencies; do not promote them into established universal rules by drafting a skill.
- All five foundations now have complete candidate pools and example builds. Review intersections before numerical tuning: active/inactive passive scope, duplicate skills, slot levels across presets, cross-class weapon compatibility and lineage inheritance, then talent interactions. No new system or resource required merely to establish identity.

## Reference leads for further verification
Prior design discussions identified Go Go Muffin's Swordbearer skill transformations and retaliation, Sword x Staff's Charms and trigger-dependent effects, Last Epoch's skill-specific trade-offs, Torchlight: Infinite's skill support interactions and Diablo IV's weapon-switch incentives. Use these as research leads, not proof of exact named effects or values; verify current primary/community documentation before relying on specific mechanics. Adapt principles to Gravitas, not exact kits. See REFERENCES.md for the wider reference index.

## Evidence and validation
No implementation/playtest evidence yet. When testing begins, record reproducible observations, relevant build/version, what changed, and the resulting lesson; do not present design hypotheses as measured outcomes.
