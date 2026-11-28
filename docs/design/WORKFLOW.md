# Design notebook workflow

- Start with [current direction](DIRECTION.md) and the [master tree](MASTER-TREE.md). The master tree is a stable index, not a commitment or release schedule.
- Keep one canonical system document per subject. When a decision changes, edit its current rule in place, update affected cross-references, and remove obsolete alternatives or examples that no longer help. Git history retains previous versions; do not append chronological correction logs to active specifications.
- Distinguish Established (owner-confirmed), Proposed (under review), Future (deferred), and Open (not yet decided). Never silently promote assistant examples into canon.
- Maintain [design learning notes](DESIGN-LESSONS.md) as critique, reference comparisons and tests reveal reusable principles. Consolidate lessons separately from canonical rules; distinguish preferences, hypotheses and verified results. Reuse lessons when reviewing subsequent kits.
- Preserve meaningful unresolved alternatives and implementation questions, but avoid repetitive recaps, speculative filler and redundant copies of specifications.
- Keep this project separate from ORBIT!, OMDB and other Roblox concepts. Do not import their mechanics without approval.
- Maintain concise README navigation and stable branch IDs. Validate links, current terminology and contradictions after changes.
- Optional depth is a game-wide requirement; ordinary play should not require detailed mechanical knowledge.
- Current priority: owner review of [Oracle](classes/ORACLE.md) and [pre-Prestige II audit](PRESTIGE-I-AUDIT.md); talent economy approved (see TALENTS.md); resolve tree access, hybrid cap compatibility, skill inheritance, combat event contract, auto/encounter contract and balance prototype before P II. Ten class drafts structurally verified. Earlier working decisions remain in canonical CLASSES, TALENTS, PROGRESSION, COMBAT-SWITCHING, SKILLS-AND-COLLECTION and DESIGN-LESSONS; do not treat open proposals as approved.
- No gameplay implementation is represented by this design notebook.

## Legendary class skill weapon compatibility
Owner direction (2026-11-27): both native Legendary Core Skills and both native Legendary ordinary active skills of a class must work with either of its compatible weapons; no mandatory single weapon for class-defining Legendary skills. Preserve normal skill acquisition and class eligibility. Use weapon-appropriate choreography and skill-defined range, without requiring another equipped weapon. Dedicated weapon skills remain weapon-specific; existing Normal/Rare starting-skill restrictions are unchanged pending further owner direction. Whether rarity promotion of a lower-starting-rarity skill changes its compatibility remains open. Test both weapon loadouts and inherited skill eligibility; do not infer universal cross-class access.
