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

## Reference leads for further verification
Prior design discussions identified Go Go Muffin's Swordbearer skill transformations and retaliation, Sword x Staff's Charms and trigger-dependent effects, Last Epoch's skill-specific trade-offs, Torchlight: Infinite's skill support interactions and Diablo IV's weapon-switch incentives. Use these as research leads, not proof of exact named effects or values; verify current primary/community documentation before relying on specific mechanics. Adapt principles to Gravitas, not exact kits. See REFERENCES.md for the wider reference index.

## Evidence and validation
No implementation/playtest evidence yet. When testing begins, record reproducible observations, relevant build/version, what changed, and the resulting lesson; do not present design hypotheses as measured outcomes.
