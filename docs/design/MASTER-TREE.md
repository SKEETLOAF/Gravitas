# Master Game Design Tree

Status: navigation index; linked canonical system documents distinguish established rules from proposals. See [current direction](DIRECTION.md). All topics below are discussion branches, not requirements or a release schedule. IDs are stable navigation references.

## I. Game identity and design foundations
- Game identity: genre/subgenres; core fantasy; unique selling points; inspirations; target audience; setting/themes.
- Design philosophy: idle vs active participation; accessibility vs complexity; power fantasy vs challenge; freedom vs specialization; solo vs multiplayer viability.
- Gameplay loops: moment-to-moment; short sessions; daily; weekly; long-term; endgame; returning-player experience.
- Established: one persistent character per account (no alternate character saves planned at launch), multiple classes, fast semi-idle hack-and-slash combat. Reference library: [REFERENCES.md](REFERENCES.md).

## II. Character creation and identity
- Identity: name/profile; appearance (body proportions, facial features, hair/color, distinguishing features); races/species (characteristics, abilities, progression); origins/backgrounds (starting benefits, opportunities, narrative significance); traits (innate talents, strengths/weaknesses, acquired traits).
- Individuality: earned titles and cosmetics with rarity-scaled statistical bonuses using the seven equipment tiers (see ITEMIZATION.md), reputation; accomplishments; character history; visual customization; emotes/personality; inspection; profile showcases.
- Open: mechanical versus cosmetic individuality.

## III. Class and discipline systems
- Working foundation model: Warrior, Ranger, Mage, Rogue, Cleric; earned promotions and independent retained disciplines, distinct benefits, potential hybrid/special classes. Initial scope two promotions per foundation (15 ordinary classes) and one hybrid per unordered pair of core classes (10 hybrids, 25 ordinary/core-hybrid classes), plus special families (Sword Saint, Summoner, Gunslinger) with simpler horizontal variant advancement and competitive scaling; exact unlock topology and names open. See [class architecture and template](CLASSES.md).
- Architecture: base, advanced, specialized, hybrid, hidden/unlockable classes; advancements/awakenings.
  - Class expansion is established: unlocking a descendant adds a distinct, independently developable and equippable discipline; no parent is replaced or consumed. Players can progress every accessible class, including sibling branches, and return to previous styles with their progression retained. Class lineage represents a common concept and unlock ancestry, not a mandatory power hierarchy. Every foundational, advanced, hybrid or special class must have a distinct combat identity and benefit, even relative to its parents or descendants. Combos, synergies and future hybrid unlock paths may originate from any class or branch, not only foundations; exact combinations, unlock requirements and equipment compatibility are still design work. All ten unique foundational pairs have an initial hybrid candidate; promoted/special-class pairs are not promised.
  - Class switching: two class selections, two shared weapons, 0.5-second class swap cooldown, two active-skill loadouts including same-class specialization, one overall ultimate, automatic weapon selection; see [switching](COMBAT-SWITCHING.md).
  - Multiclassing: primary full/secondary weakened talent contributions, same-class empowered primary nodes, overlapping same-lineage talent nodes stack effective ranks, class-associated passives, active-class Traits, class combinations.
  - Class/weapon relationship: linked compatible weapons (confirmed); potential primary and secondary weapon roles, asymmetric shared compatibility and cross-class synergy; see [switching proposal](COMBAT-SWITCHING.md).
- Development: experience, mastery, ranks, one upgradeable passive Class Trait per class (mastery and Ascension items), five shared foundational lineage talent trees, specialization, trials, quests, mastery rewards.
- Identity: unique mechanics/resources/movement/automation; weapon proficiency; strengths/weaknesses; solo/co-op roles; fantasy/visual identity.

## IV. Combat systems
- Elemental architecture and reaction exploration: [ELEMENTS.md](ELEMENTS.md).
- Shared combat foundations and attribute roster established conceptually; exact formulas open. See [COMBAT-FOUNDATIONS.md](COMBAT-FOUNDATIONS.md).
- Offense:
  - Basic attacks: completed chain has brief recovery; class swap can extend chain and pursue knocked-back target. Chain lengths, attack speed, recovery values and hit reactions open.
  - Heavy attacks: charges, guard breaks, launchers, finishers.
  - Abilities: slots, cooldowns, resource costs, follow-ups, combinations.
  - Ultimates; aerial combat; area attacks; ranged attacks; summons.
  - Combat flow: Impulse hit-stun pulses (including support), basic-string resets/extensions, knockback after completed string, pursuit and class swaps; intact Armor prevents stagger. Mixed automatic combos; detailed timing, tracking and weapon transitions open; universal weapon/skill animation ownership established.
- Defense: dodge, block, parry, counter, mitigation, shields/barriers, interruption, hyper armor, crowd-control resistance, recovery/healing.
- Movement: pursuit, dash/gap close, reposition, target switching, lock-on, tracking, knockback, grouping, vertical movement.
- Interactions: damage types, elemental interactions, status effects (DoT, buffs/debuffs, crowd control, stacking, reactions), stagger/posture, critical attacks, weak points, executions, environmental interactions, co-op synergy.
- Feel: choreography, transitions, hitstop, camera response, impact VFX, audio, damage feedback, enemy reactions, pacing/readability.
- Principle: not every class needs every mechanic. AFK Dungeon-like real-time battlefield flow, not stationary or turn-based battles.

## V. Automation and player participation
- Current idle progression design: [WORLD-AND-IDLE.md](WORLD-AND-IDLE.md).
- Auto-combat: movement, targeting, combos, skills, defense, resource management, stage progression, recovery, looting.
- Automation: simple developer-authored presets and player-created combat macros; shared data-driven sequence executor recommended. Targeting, pursuit, skill readiness and resource management handled by common actions; advanced conditions and editor details open. See [Combat flow](COMBAT-SWITCHING.md).
- Active participation: manual ability activation, targeting, repositioning, situational inputs, opportunities, temporary overrides, auto-resumption, performance advantages, possible manual swaps.
- AFK/offline: online farming, offline simulation and limits, targeted farming, repeatable activities, auto-repeat, failure/retry, inventory management, return summaries.
- Full manual (future): direct movement, attack chains, defense, ability combinations, PC/mobile/console controls, seamless control transitions.
- Open: exact macro editor/executor rules, launch inputs and optional advanced conditions; offline progression is distinct from online automation.

## VI. Character power and progression
- Progression direction (permanent account-wide Character Level for milestone rewards, unlocks, inherent stats, level-gap penalties and percentage scaling; independent class mastery and lineage prestige levels with lossless stage resets and rising caps; catch-up; Character XP 100% once, lineage XP 100%/50%, mastery evenly split; same-lineage XP handling and source details open) and optional depth principle: [PROGRESSION.md](PROGRESSION.md).
- Fundamental: character level/XP, ranks, milestones, ascension/rebirth, vertical/horizontal growth.
- Attributes: primary, secondary, derived stats, allocation/scaling, caps/diminishing returns, interactions.
- Masteries: weapons, combat, class, abilities, professions.
- Permanent development: bonuses, character-wide unlocks, milestone abilities, achievement benefits, training, collections, potential swap-slot unlocks.
- Management: respec, catch-up, compression, pacing, soft/hard walls, newcomer/veteran growth.
- Established separate permanent account Character Level, Class Mastery, lineage levels/prestige, skill and equipment development; exact scaling, XP source attribution and same-lineage handling open. Shared systems unlock via Character Level and usually adventure-stage clears; prestige labels are intended pacing/release ranges, not mandatory lineage-prestige gates. Most major foundational systems paced for Prestige 0, including Reforge/Recast and customizable pet moves; mounts very early I, relics and evolved-pet Mythic Moves II, Pet Ascension tentatively II, equipment Enhancements II, core hybrids/awakened skills/mount equipment III, Stellar Path-like concept distant III+. Later Character Level/stage milestones may unlock additional released systems. Avoid redundant leveling.

## VII. Ability and build systems
- Owner direction on Energy, skill acquisition, upgrade/duplicate ranks, focused summons and Stardust: [SKILLS-AND-COLLECTION.md](SKILLS-AND-COLLECTION.md).
- Acquisition: classes, drops, trainers, tomes, quests/trials, crafting/discovery.
- Development: levels, proficiency, evolution, variants, modifiers, ability-specific talent branches.
- Construction: four actives per class slot (including specialization), one overall ultimate, one of two passives per distinct class (both when specializing); lineage talent trees/presets (Attribute, Conditional, Transformative nodes with 3–5 investable ranks each, linear effective rank overflow), inheritance, equipment interactions, resources, synergies, multi-kit rotation.
- Management: presets/loadouts, auto/active configurations, testing, statistics, damage analysis, sharing, recommendations.

## VIII. Equipment and itemization
- Current itemization specification: [ITEMIZATION.md](ITEMIZATION.md).
- Planned full-game weapon roster and foundational compatibility: see [WEAPONS.md](WEAPONS.md). Each foundational class has primary and secondary compatibility; two global weapon slots with one weapon skill each; primary full/secondary weakened attribute contribution; automatic action-driven wielding and universal weapon/skill animations established; detailed timing open.
- Weapons: categories, movesets, attributes, exclusive abilities, mastery, stances, dual wield, off-hand, unique/legendary weapons, potential weapon swap slots; primary and secondary class compatibility; shared weapon bridges.
- Armor/accessories: slots, categories, jewelry, relics/artifacts, set bonuses, exclusive effects.
- Generation: rarity, item levels, fixed/random stats, affixes/modifiers, unique effects, drop tables, targeted loot, duplicates.
- Development: enhancement, refinement, reforging, enchantments, gems/sockets, evolution, rerolling, inheritance, salvage.
- Inventory: gear/material storage, sorting/filtering, locking, auto-selling/salvaging, comparison, transmog, loot protection.

## IX. World structure and adventure
- Map-ending dungeon progression gate, farmable dungeon, boss-only ten-minute respawn/Robux skip, party progression rules: [WORLD-AND-IDLE.md](WORLD-AND-IDLE.md).
- Architecture: personal worlds, public areas, hubs, instances, regions/biomes, maps, fast travel.
- Progression: chapters, regions, stages/substages, difficulty tiers, unlocks, clear conditions, world scaling, co-op credit.
- Exploration: points of interest, hidden areas, treasure, environmental puzzles, secret encounters, discoverable abilities/gear.
- Activity: populations, dynamic encounters, events, wandering bosses, resource nodes, NPC interactions.
- Open: continuous traversal vs reset battlefields vs stages in regions or hybrid.

## X. Enemies and encounters
- Architecture: common enemies, elites, minibosses, bosses; families, archetypes, factions, affinities, variants, rare enemies.
- Behavior: targeting, aggression, movement/attack/defense patterns, cooperation, reinforcements.
- Encounter design: compositions, waves, spawns, density, modifiers, hazards.
- Bosses: patterns, phases, breakable defenses, weaknesses, special mechanics, co-op interactions, enrage, rewards.
- Difficulty: statistical/mechanical difficulty, scaling, co-op scaling, modifiers, automation compatibility.

## XI. Game modes and PvE content
- Campaign: stages, chapters, difficulty tiers.
- Dungeons: equipment, materials, class-specific rewards.
- Endless: towers, survival, escalating encounters.
- Boss hunts: targeted/rare/world bosses.
- Raids: group encounters, phases, raid progression.
- Trials: class/mastery/combat challenges.
- Expeditions: owner accepts companion expeditions; resources/exploration/offline activity are candidate mechanics, unlock timing open.
- Roguelite: temporary builds, randomized encounters, run modifiers.
- Challenges: time trials, restricted builds, performance rankings.
- Events: seasonal/limited encounters, special rewards.
- Training: practice arenas, simulations, build tests.
- For each accepted mode: entry, gameplay, failure, rewards, replayability, multiplayer, automation.

## XII. Multiplayer and cooperative systems
- Connectivity: friends, parties, invites, joining personal worlds, matchmaking, private sessions, rejoin.
- Progression: host/guest progress, shared clears, assistance rewards, loot, level differences, carrying/scaling.
- Combat: enemy health/difficulty scaling, threat, support, cooperative combos, heals/protection, revives, automated party participation.
- Social: profiles, inspection, chat, emotes, hubs, help requests, recruitment, mentorship.
- Established: others can enter one's world and help clear stages; carrying is not automatically an exploit.

## XIII. Guild systems
- Organization: creation, membership, recruitment, ranks/permissions, identity/customization, administration.
- Progression: XP, levels, research, resources, contributions, milestones.
- Activities: bosses, raids, expeditions, quests, challenges, assistance.
- Infrastructure: headquarters, facilities, shop, upgrades, storage.
- Competition: rankings, tournaments, wars, territory, alliances.
- Guilds established; guild features unlock via guild level-ups and guild management, not Character Level or prestige (owner direction). Individual features and scale undecided.

## XIV. Competitive and PvP systems
- Competitive PvE: stage rankings, clear times, damage records, class/solo/co-op rankings, seasonal competition.
- Direct PvP: duels, automated/assisted/manual arena, team/guild PvP.
- Infrastructure: matchmaking, ratings, divisions, seasonal rewards, normalization, class balance, spectating/replays.
- PvP not confirmed.

## XV. Professions and noncombat progression
- Gathering: possible mining, fishing, herbalism; discovery, rarity, tools, efficiency, respawns, automation.
- Production: possible smithing, alchemy, cooking; recipes, quality, specialization, conversion, gear/consumables.
- Development: levels/mastery, perks, recipes, equipment, quests.
- Economy: commissions, resource exchange, exclusive goods, trading, demand.
- Open: avoid forcing one character to interrupt combat for chores.

## XVI. Supplemental character growth
- Pet and mount collection/upgrade direction: pets available from start with basic attacks and customizable equippable moves (not a single fixed skill), evolved-pet Mythic Moves at II; mounts very early Prestige I with one skill and equipment at III; pet generations improve with class progression plus character level; mounts more universal; potential donor-sacrifice ascension for earlier pets tentatively at II. Relics unlock II, detailed design deferred: [SKILLS-AND-COLLECTION.md](SKILLS-AND-COLLECTION.md).
- Owner confirms relics as unique upgrades, and mounts/pets as character enhancement directions. Specific mechanics, slots, acquisition and scope remain open; see [ELEMENTS.md](ELEMENTS.md).
- Companions/familiars/pets: combat/gathering assistance, passive bonuses, development.
- Mounts/transport; relic/collection systems; housing; personal training facilities; reputation/factions; titles/achievements; blessings/contracts; transformations/temporary states; account-wide benefits.
- Guardrails: each needs purpose beyond another damage multiplier; no mandatory hero roster.

## XVII. Quests, narrative and worldbuilding
- Foundations: cosmology, history, magic/power, civilizations, races, factions, conflicts.
- Player narrative: origins, significance, development, choices, accomplishments.
- Quests: main, side, class, profession, guild, daily/weekly, hidden, repeatable.
- Delivery: NPC dialogue, cinematics, environmental storytelling, discoveries, boss introductions, collections/codices.
- Setting and narrative scale undecided.

## XVIII. Economy and rewards
- Currencies: standard, specialized, premium, activity-specific, conversion.
- Resources: acquisition, sinks, scarcity, recycling, inflation.
- Rewards: XP, equipment, materials, first-clear/repeatable/performance/milestone rewards, guaranteed growth, rare drops, pity/bad-luck protection.
- Shops/services: NPCs, rotating stock, specialized shops, exchanges, upgrades.
- Player economy: trading, gifting, marketplace, auctions, binding, restrictions, fraud/exploit prevention.
- Current economy proposal: [ECONOMY.md](ECONOMY.md). Offline rewards and co-op progression: [WORLD-AND-IDLE.md](WORLD-AND-IDLE.md).

## XIX. Monetization
- Cosmetics: outfits, weapon skins, hair, auras, effects.
- Expression: emotes, idle/finisher animations.
- Convenience: presets, inventory, management tools.
- Progression: boosters, passes, resources.
- Collection: limited appearances/collectibles.
- Premium services: customization/appearance changes.
- Subscriptions; possible gacha; gifting; guild customization/supporter benefits.
- Established: paid acceleration with attainable free equivalents, guaranteed acquisition paths, free cosmetic summons, minor cosmetic bonuses and optional boss respawn skips. Exact pricing, odds, progression rates and purchase scope open. See [ECONOMY.md](ECONOMY.md).

## XX. User interface and player experience
- Combat HUD: health/resources, ability slots/cooldowns, buffs/debuffs, enemy info, targeting, automation, potential swap/cooldown indicators.
- Character UI: stats, gear, classes, masteries, trees, presets.
- Adventure UI: map, stages, quests, dungeons, rewards.
- Social UI: friends, parties, guilds, invites, inspection.
- QoL: search/filter, bulk actions, notifications, upgrade indicators, comparisons, recommendations, summaries, customizable HUD.
- Accessibility: mobile/console, VFX settings, camera, input customization, text readability, damage numbers.

## XXI. Art direction and presentation
- Visual identity: art style, proportions, color language, environments, equipment, enemies.
- Animation: movement, idle, combat, class-specific animations/evolution, cooperation, possible swap transitions.
- VFX: attacks, elements, statuses, ultimates, progression, loot, optimization.
- Camera: default perspective, tracking, zoom, cinematics, manual camera.
- Audio: combat, class identity, music, boss themes, environment, UI.
- Style open; combat should be fluid, spectacular and readable.

## XXII. Onboarding, retention and live content
- New-player experience: creation, tutorial, first class/combat/rewards, automation introduction, gradual systems.
- Retention: short goals, daily/weekly activities, long projects, personal milestones, social incentives, return rewards.
- Live content: seasons, classes, regions, gear, professions, events, limited challenges, community goals.
- Longevity: replayability, random encounters, difficulty variation, build experimentation, endgame, horizontal expansion.

## XXIII. Balance and mathematical systems
- Damage: base, attribute scaling, coefficients, crit, defense/resistance, multipliers.
- Curves: XP, enemy power, item power, costs, stage difficulty.
- Builds: class/weapon strengths, ability efficiency, synergy limits, dominant strategies, swap rotation balance.
- Idle: farm efficiency, offline income, automation performance, active advantages.
- Multiplayer: party scaling, assistance rewards, roles, progression disparity.
- Economy: generation/consumption, inflation, reward frequency, monetization impact.
- Open: exponential vs restrained growth, formulas, caps and tuning.

## XXIV. Technical foundations and development
- Combat: state machines, ability framework, hit detection, damage, animations, shared auto/manual action pipeline, potential persistent per-kit cooldowns.
- AI: automation, enemy AI, navigation, targeting, decisions, optimization.
- Multiplayer: instancing, servers, party sync, network, server authority, reconnect.
- Data: character, class, inventory, offline calculations, trade transactions, recovery.
- Performance: enemy counts, animation/effect/network budgets, mobile, LOD.
- Tooling: class/ability/enemy creation, loot and encounter editors, balance simulations, automated tests, analytics, admin, anti-exploit.
- Release scope/roadmap: prototype, validation, priorities, dependencies, later manual combat. Tentative P0/I at launch, biweekly updates, P III after six full weeks, two batches of five core hybrids, subject to readiness; see PROGRESSION.md.

## Cross-branch relationship map
Character -> classes, attributes, equipment -> abilities/builds -> combat -> automation/active input -> adventure -> content/co-op/guilds -> rewards/economy/progression -> character. Switching touches III, IV, V, VI, VII, VIII, XX, XXI, XXIII and XXIV. This is not a dependency lock or implementation schedule.

## Discussion order
1. Foundations: I, IV, V, III, II.
2. Character development: VI, VII, VIII, XVI, XV.
3. Adventure: IX, X, XI, XVII.
4. Multiplayer: XII, XIII, XIV.
5. Supporting systems: XVIII, XIX, XX, XXI, XXII.
6. Implementation: XXIII, XXIV, release scope/roadmap.
