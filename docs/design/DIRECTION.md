# Current direction and decision ledger
Updated 2026-11-26. Owner decisions supersede earlier suggestions. A proposal is not an implementation requirement.

## Established
- Roblox semi-idle RPG centered on one persistent customizable character, rather than a collectible team or roster.
- The same character can wield multiple classes. Classes have linked weapons (confirmed 2026-11-26); exact compatibility and switching rules remain open.
- Hybrid world and instanced encounters. Players can join another player's world and help clear stages; cooperative play and guilds are desired.
- Fast-paced, real-time hack-and-slash combat: physical movement/pursuit, continuous battles, expressive attack sequences, satisfying automated combat. Not Raid: Shadow Legends-style stationary/turn-based combat.
- AFK Dungeon is the closest reference for actual combat flow. Wuthering Waves and Phantom Blade Zero influence visual fluidity, choreography and impact, not a requirement to build their entire manual combat system.
- Auto-combat available wherever combat occurs. Active input is optional and can offer advantages or a better method in certain circumstances; it is not a prerequisite for ordinary participation.
- Full manual combat mode is planned for later. Build shared underlying combat actions with that possibility in mind (technical recommendation).
- Personal character development remains the central fantasy. Co-op does not mean managing multiple characters.

## Class architecture (2026-11-26)
- Class expansion is established: unlocking a descendant adds a distinct, independently developable and equippable discipline; no parent is replaced or consumed. Players can progress every accessible class, including sibling branches, and return to previous styles with their progression retained. Class lineage represents a common concept and unlock ancestry, not a mandatory power hierarchy. Every foundational, advanced, hybrid or special class must have a distinct combat identity and benefit, even relative to its parents or descendants. Combos, synergies and future hybrid unlock paths may originate from any class or branch, not only foundations; exact combinations, unlock requirements and equipment compatibility are still design work. This does not promise that every pair yields a bespoke hybrid.
- Four foundational classes with individual advancement branches; Warrior and Mage locked, Rogue and Cleric tentative. Every class should have its own benefit.
- Warrior -> Berserker is an advancement example. Hybrid classes unlock through progression of multiple disciplines; Warrior + Cleric -> Paladin is an example, not a finalized roster commitment. Main class branches and template take priority over hybrid design.
- Independent special classes may come from game passes, limited events/battle passes, or dungeons; acquisition and balance remain exploratory.
- See [class architecture and template](CLASSES.md) for candidate branches and open decisions.

## New exploratory direction
- Possible in-combat class or weapon switching to increase combat liveliness and extend combos.
- Swapping should let the character access another kit's available skills rather than all kits sharing one skill cooldown pool.
- Additional swap options earned through grinding/progression.
- Tentative maximum: three classes and two weapons. Which switching layer(s) exist and how these limits relate remain open.
- Owner proposal (2026-11-26): secondary/alternative compatible weapons can bridge classes. Example: sword is Warrior's primary, gauntlets are Warrior's secondary but Monk's primary. These are illustrative classes; exact compatibility rules remain open.
- See [combat switching](COMBAT-SWITCHING.md). These are owner proposals, not finalized mechanics.

## Inspirations and intended study areas
Owner-named references:
| Reference | Design study focus (interpretation, not imported canon) |
| --- | --- |
| AFK Dungeon | Automated moving 3D combat, rapid enemy/stage progression, combinations and power scaling |
| Go Go Muffin | Class development/advancements, talent builds, co-op, encounter-sensitive abilities |
| The War of Genesis | Incremental growth, spectacular skills and power progression; exact installment not confirmed |
| Ulala: Idle Adventure | Skill sequencing, encounter counters, party synergy and preparation |
| IdleOn | Branching disciplines, interconnected professions and growth, specialized AFK builds without requiring multiple characters in Gravitas |
| Blade & Shield Girl | Single-character power fantasy, visually satisfying combat, equipment/gem interactions |
| Wuthering Waves | Fluid movement, expressive combat, class-specific mechanics, animation and counters |
| Phantom Blade Zero | Aggressive choreography, attack/defense transitions, impact, weapon identity |

Additional assistant-suggested references (not owner-confirmed requirements): Granblue Fantasy: Relink (co-op action and assists), Dragon's Dogma 2 (vocations), Nioh 2 (weapon/mastery builds), Diablo IV (loot and repeatable co-op encounters), Black Desert Online (flashy PvE, class awakening and life skills). Reference descriptions are brainstorming interpretations, not independently verified specifications.

## Exploratory principles and options
- Seamless automatic/assisted participation; selective input could temporarily override automation and then resume it.
- Active advantages could emerge from execution (timing, targeting, repositioning, combos) rather than arbitrary manual XP multipliers.
- Build quality and automation configuration may let an optimized idle player outperform an unprepared active player.
- Consider class-specific automated behavior, tactical presets, conditional skill usage, mastery affecting behavior; none confirmed.
- Character-wide progression vs discipline mastery; class expansion and switching established; primary/secondary roles and inheritance details exploratory.
- Visual growth: new chains, follow-ups, animations, fighting styles, transformations, equipment-changing abilities; not required for all classes.
- Personal world progression and shared hubs, host/guest credit, worthwhile helper rewards, co-op scaling, carrying rules: details open.
- Offline simulation is separate from online AFK; offline mechanics not confirmed.
- Optional modes, PvP, professions, pets, races, origins, monetization, gacha and all other branches in the master tree are exploratory.
- Avoid progression bloat, redundant systems, compulsory active play and default assumptions that stronger friends helping is exploitative.

## Unresolved decisions
- Final title, setting, audience, art direction, narrative.
- Core gameplay loops and early/long-term progression goals.
- Camera, targeting, launch inputs, offensive/defensive mechanics, skill counts and resource systems.
- Class/weapon ownership, switching model, progression requirements, cooldowns and swap limits.
- World structure, stage topology, party size, matchmaking, progression credit, difficulty scaling and guild depth.
- Offline gains, itemization, stats, balance formulas, economy, monetization and release scope.

## Pending architecture alternative (2026-11-26)
Owner is considering five core role lineages (Tank, Ranger, Mage, Melee DPS, Support) with sequential earned promotions inspired by Go Go Muffin, and independent special unlocks for unusual classes. This is an alternative to the previously established four-family branching model, not a confirmed replacement. Prior class expansion and hybrid eligibility decisions remain in force unless explicitly revised. See [class architecture](CLASSES.md#alternative-architecture-under-consideration-2026-11-26-promotion-lineages).

## Weapon roster (2026-11-26)
Owner's planned full-game weapons: Sword, Greatsword, Polearm, Dagger, Mace, Gauntlet, Shield, Bow, Firearms (Light, Medium, Heavy), Magic Staff, Tome. Each foundational class should have a primary and secondary weapon; Warrior uses Sword primary and Shield secondary, Ranger Dagger secondary, Rogue Sword secondary, Mage Magic Staff primary with Tome secondary, Cleric Tome primary with Shield secondary recommended from the earlier options. Owner's Tome clarification supersedes earlier Mage Dagger and Cleric Mace proposals. Recommended mapping and status distinctions are in [WEAPONS.md](WEAPONS.md).

## Shared foundations discussion priority (2026-11-26)
Owner wants general RPG mechanics (DPS, tank, sustain, burst, DoT, buffs/debuffs, healing, CC, status effects and equipment slots) explored before individual class design. See [COMBAT-FOUNDATIONS.md](COMBAT-FOUNDATIONS.md); candidate mechanics are not accepted automatically.

## Elemental and supplemental growth direction (2026-11-26)
Owner wants Fire, Water, Earth, Resonance (Wind/Sound), Cold, Lightning, Necrotic, Force (Gravity), Light and Dark explored; supplied nine-element alternative and reaction matrix for refinement. Light/Dark apply universal Radiance/Corruption; Force a neutral cosmic median with universal modification. VFX should reuse combinations/gradients. Recommended separation of Resonance and Force, Necrotic and Dark, individual statuses and reaction behaviors are documented in [ELEMENTS.md](ELEMENTS.md), pending approval. Owner confirms relics as unique upgrades and wants mounts and pets enhancing the player; details remain open.

## Combat, collection and adventure decisions (2026-11-26)
Energy is the universal skill resource; no universal ultimate gauge. Attack rate/cooldowns govern automated hack-and-slash; defense checks use block/evasion stats vs counters, and detailed combat flow is deferred. Base skills acquired with classes; summons unlock alternatives and duplicate star ranks; earned upgrades, cooldown/charge systems, selectable summon focus, multiple pity levels, max duplicates become Stardust. Pets are mini partners with skills; mounts modestly enhance character; both collectable by rarity with summon/duplicate upgrades. Both unlock mid-to-late early game, mount at first class promotion. Relic deep design deferred to update. Paid acceleration desired with attainable free equivalents. Aggro attribute; world party cap 4, raids 6/8, server-wide bosses, flexible global events; shared party progression in same location, character collects XP and loot. Each map ends in a dungeon clear/loot gate; 10-minute cooldown or Robux skip. See [skills and collection](SKILLS-AND-COLLECTION.md) and [world and idle](WORLD-AND-IDLE.md) for established versus recommended details; regeneration rates, pity thresholds, cooldown scope and idle rates remain open.
