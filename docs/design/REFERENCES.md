# Design references

References are study targets, not imported requirements. Specific mechanics and current versions should be verified when they become relevant.

## Owner-selected
| Game | Study focus |
| --- | --- |
| Sword x Staff | Hybrid idle RPG and explorable world, single-character build customization, skill sequencing and automated movement/pursuit; study co-op, progression pacing and active engagement |
| AFK Dungeon | Moving automated hack-and-slash combat, farming and boss progression |
| Go Go Muffin | Class changes, skill summons, separate resettable talent trees that grant stats and modify skills, pets, mounts, gear sets and slot investment |
| Diablo IV | Branching skill customization, especially transformative upgrades in April 2026 rework; loot and encounters |
| Torchlight: Infinite | ARPG loot, build construction, skills, modifiers and synergy |
| Black Desert Mobile | Automated action combat, character growth, farming and large-scale encounters |
| AFK Arena | Idle reward accumulation and progression-linked rewards |
| Ulala: Idle Adventure | Cooperative progression, encounter preparation, skill sequencing |
| IdleOn | Interconnected progression and specialization |
| Blade & Shield Girl | Single-character power fantasy and equipment interactions |
| The War of Genesis | Incremental growth and spectacular skills; exact installment open |
| Wuthering Waves | Fluid action, expressive animations and impact |
| Phantom Blade Zero | Aggressive choreography, weapon identity and combat transitions |
| Dragon Ball: Sparking! ZERO | Pursuit, ranged tracking and mixed basic/skill combo flow |
| Dragon Ball FighterZ | Sparking-style combo extension and cancel feel |

## Optional study targets
Last Epoch (shared base/mastery passive tree structure), Granblue Fantasy: Relink (co-op action), Dragon's Dogma 2 (vocations), Nioh 2 (weapon identities), Black Desert Online (class awakening and PvE). These are suggestions, not additional scope.

## Reference resources
- Go Go Muffin: level-linked stat/skill-modifying resettable talents https://boarhat.gg/games/go-go-muffin/guide/beginner-guide/ ; separate class change skill summon banners https://boarhat.gg/games/go-go-muffin/guide/cc1-guide/
- Diablo IV April 2026 skill tree rework: https://news.xbox.com/en-us/2026/04/22/diablo-4-skill-tree-overhaul/ ; passive node removal https://news.blizzard.com/en-gb/article/24267729/prepare-for-the-reckoning-lord-of-hatred-draws-near
- Last Epoch mastery passive access: https://support.lastepoch.com/hc/en-us/articles/46363282865435-Can-I-spend-Passive-points-in-the-Mastery-trees
- Torchlight: Infinite talent panels and Hero Traits: https://tlidb.com/en/Basic_Rules
- Black Desert Mobile Transcendence rework: https://www.world.blackdesertm.com/Ocean/News/Detail?boardNo=4521
- Torchlight: Infinite: https://torchlight.xd.com/
- Black Desert Mobile: https://www.world.blackdesertm.com/
- Roblox paid random items: https://create.roblox.com/docs/production/monetization/paid-random-items
- Roblox PolicyService: https://create.roblox.com/docs/reference/engine/classes/PolicyService

These links are reference starting points, not a completed research audit.

- Go Go Muffin Stellar Path reference: https://boarhat.gg/games/go-go-muffin/guide/stellar-path/ (verified 2026-11-26; class-independent Paths, Authority modifiers and Ascension equipment; CC3 unlock). Secondary cross-reference: https://muffincompass.com/stellar-path. Adapt purpose, not a required copy of mechanics.

- Sword x Staff (owner-selected): official Google Play description, updated Nov 24, 2026: https://play.google.com/store/apps/details?hl=en-US&id=com.zjcs.android.us ; official launch announcement https://swordxstaff.boltray.com/news/200. Publisher describes explorable regions, idle resources, flexible class/skill sequencing and automated repositioning/pursuit. Study actual gameplay before adopting particular mechanics; no claim that the game implements Gravitas's proposed clash QTEs.

## Encounter and preparation study (2026-11-27)
Research references, not approved new mechanics:
- Go Go Muffin CC2 Rifts and dragon encounters: https://boarhat.gg/games/go-go-muffin/guide/cc2-guide/ — Pulse of the Sand Abyss has destructible horns that reset a boss power meter; Lumberyard Ablaze has clickable cleansing fruit; Battle of the Construct Factory has lingering targeted hazards and tank-directed attacks; Calamity Breaker Dragon requires specific numbers of players in marked zones. Useful reference for Gravitas's approved active encounter categories.
- Go Go Muffin mode presets: https://boarhat.gg/games/go-go-muffin/guide/game-mode/ ; more role/interrupt/positioning examples: https://boarhat.gg/games/go-go-muffin/guide/cc3-guide/ .
- Sword x Staff: https://www.prydwen.gg/sword-x-staff/guides/beginner-guide — guide updated July 22, 2026 describes fully automated PvE/PvP fights with no direct manual character control. Distinguish automated movement from player-controlled movement. https://www.prydwen.gg/sword-x-staff/guides/classes-and-roles describes solo-capable roles and separate skill/charm/pet loadouts; https://www.prydwen.gg/sword-x-staff/guides/daily-dungeons describes node choices, completion-based ranks and dungeon rewards. Study activity-specific presets, route choice and performance rewards; these are proposals, not new Gravitas requirements. Avoid importing mandatory daily attempt limits or full-auto-only combat.

Owner-approved adaptation direction: designated combat-zone repositioning for semi-idle boss/raid encounters (Go Go Muffin reference); reserve direct free movement for the later action-RPG alternative. Retain automated battlefield movement and pursuit. Owner welcomes collaborative development of the other encounter/preparation references; specific implementations remain proposals until individually agreed.

- Owner-selected Sword x Staff inspiration for cosmetic Style Score: adapt a rarity-weighted collection progression bar with appearance-independent milestone benefits. Community database https://www.purrwikimania.com/cosmetics (checked 2026-11-27) reports wardrobe Style point values by rarity: Common 20, Rare 40, Epic 70, Legendary 100, Mythic 250, Divine 400, Immortal 800. Gravitas adopts a 0/100 bar (owner-confirmed); owner requires multiples of five; owner-specified doubling weights 5/10/20/40/80/160 (Common through Mythic), inferred Secret 320 pending confirmation from Common through Secret, inspired by the reference's rarity progression rather than a direct conversion. Specific original Style Level thresholds were not verified; Gravitas's weights, rollover and milestone rewards remain open.
