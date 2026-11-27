# Shinobi — Prestige I kit (working draft)

Status: owner requests Naruto-like Shinobi feel and broader comparative research, including observed failures and revisions. Assassin -> Shinobi -> Blade Dancer is the established working sequence; ninjutsu, deception, afterimages and evasive counters are broad identity. Specific Trait, kit, weapons, growth and talents below are assistant proposals, not individually approved or playtested. [Assassin](ASSASSIN.md), [Elements](../ELEMENTS.md), [Classes](../CLASSES.md), [Talents](../TALENTS.md).

## Identity and profile
Anime-inspired martial ninja: hand seals, short-lived clones, substitution, thrown tools, martial combinations and elemental techniques. Assassin exploits existing vulnerability with precision; Shinobi creates opportunities with authored deception; Blade Dancer retains sustained broad combo identity; Summoner retains persistent autonomous units. No copyrighted character names, signature moves or assets copied; original visual language. Proposed Dagger primary, Gauntlet secondary (both existing families; Sword compatibility alternative remains open). Inherit compatible learned ordinary Assassin skills, not Exploit or exclusive passives. Sword-exclusive skills not silently converted. Health D(2), Energy B(4), ATK A(5), MATK C(3), DEF D(2), MDEF C(3) = 19. Proficiencies Evasion, Movement Speed, Effect Potency, Energy Efficiency. Physical martial/tool skills primarily ATK; explicitly magical elemental ninjutsu may use MATK or defined hybrid coefficients with ATK-majority where appropriate (candidate). No general dual-stat formula or new Chakra currency; Energy remains the paid resource. Keep physical-only and mixed builds viable.

## Trait — Art of Deception
- Completing a Core sequence while active creates one temporary Echo; a qualifying paid Mirror Double activation can also prepare one. Nonstacking, same-source refresh within cap; no creation from Echo actions, proc damage or inactive Core. Echo is a short-lived visual construct and authored secondary action, not persistent AI, targetable summon, separate inventory or independent skill loadout.
- Next explicitly Echo-compatible paid technique consumes the Echo once on activation, producing a skill-specific complementary action: a crossing strike, supplemental projectile coverage, second impact location or a defensive decoy. Not a full copy of a cast. No additional cooldown reset, resource refund, extra status budget or automatic critical. No arbitrary duplicate of inherited skill. Define compatible inherited skills explicitly if any.
- Echo action resolves promptly, with no separate targeting minigame or cinematic lock. If target dies, eligible area action may resolve at valid original location, no autonomous target pursuit or extra refunds. Short action cancellation and impact behavior TBD. Reuse animation/VFX pool, no independent pathfinding or physics. All damage attributed to Shinobi; secondary action cannot itself create/consume Echo, proc itself or multiply normal on-hit/reaction budget. Distinct visual and sound cue; simple automated rotations use the same rules.
- Substitution is a paid defensive technique, not universal free dodge: brief readiness against one eligible incoming ordinary attack targeted at Shinobi. Reduce a bounded part of resolved hit damage and relocate within valid zone if possible; stationary smoke/decoy fallback if not. No guaranteed evasion event, lethal prevention, threat reset, scripted mechanic immunity or movement through geometry. With Echo, improved protection or authored follow-up as specified. If no incoming hit, baseline short Evasion window remains useful; readiness expires normally. Echo is consumed on casting compatible technique; substitution-specific Echo effect is reserved for that cast until its expiry, cannot create second Echo. No automatic additional cooldown or shared resource.
- Active class Trait only; timer continues on swap, no new Echo while inactive; already committed actions may finish normally. Exact lifetime, coefficients, eligibility and stack order open. Core preparation makes co-op effective even if tank receives all incoming attacks.

## Selectable class passives (2)
- Phantom Arts: baseline Effect Potency; Echo-assisted offensive skills improve complementary impact/coverage within existing budget, not a second cast. For martial builds, eligible physical complementary strike benefits without requiring elemental status.
- Escape Artist: baseline Evasion; Echo-assisted defensive techniques gain stronger limited protection and shorter permitted movement recovery, including ordinary Substitution. No invulnerability or free repeated activation.

## Legendary Core skills (2)
- Silent Blade (guaranteed, either): swift martial sequence with a concentrated finisher; completing it creates Echo via Trait. First compatible technique after chain receives modest direct impact improvement. Dagger cuts/Gauntlet strikes reuse weapon-family animations.
- Sealbreaker (alternative, either): deliberate martial sequence ending in a short hand-seal gesture and neutral Energy-infused impact; completes Echo preparation and improves next eligible elemental technique application within cap. Neutral impact does not silently apply any element. Different cadence, not mandatory for ninjutsu; both Cores have normal baseline damage.

## Ordinary active skills (10; 3 equipped)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Kunai Volley | Either | Throw a fan of kunai, concentrated first hit; Echo assists from another angle using shared secondary coverage budget. Physical tool, not a new weapon family. |
| Normal | Substitution | Either | Brief Evasion window and one eligible incoming-hit decoy/mitigation as defined above; Echo enhances mitigation and valid lateral reposition. Defensive technique, not guaranteed evasion. |
| Normal | Flame Breath | Either | Brief hand seals then directional Fire wave applying Burn; Echo produces a reduced side impact, shared application cap per target. |
| Normal | Flash Palm | Gauntlet | Fast advancing martial strike with knockback if permitted, capped Armor pressure otherwise; Echo adds complementary flank strike, not free teleport. |
| Rare | Stormstep | Either | Lightning-infused dash/strike applies Shock, stops at valid target; Echo attacks across the approach path with reduced impact and shared application budget. |
| Rare | Mirror Double | Either | Creates Echo if absent or refreshes bounded lifetime if present; sends a short neutral decoy strike with normal paid baseline. Does not consume or create a second Echo. Useful in ordinary rotation. |
| Rare | Smoke Veil | Either | Brief local smoke zone improving own Evasion against eligible ordinary attacks, no invisibility/aggro wipe; Echo expands protective coverage for Shinobi only, not a party-wide permanent field. No new universal Blind status. |
| Rare | Wind Cutter | Either | Hand-seal Resonance crescent directed through enemies, applies Reverberation with bounded application; Echo redirects complementary impact along secondary angle. |
| Legendary | Phantom Formation | Dagger | Fast coordinated cross-slash sequence; with Echo, a pair of visual copies divide authored complementary attacks across eligible targets; baseline player sequence remains useful without Echo. One shared hit budget, no long camera lock. |
| Legendary | Tempest Palm | Gauntlet | Compressed Resonance-infused palm strike, short directional burst and Armor pressure; Echo assists by focusing part of existing area impact on primary target or distributing across grouped enemies, not a copied cast. |
All actives use standard Energy, cooldown, recovery, Impulse and Armor rules. Elemental tags explicit; no implicit Dark or Force from shadow/clone imagery. Tools are animated skill props. No ultimate, manual hand-seal minigame, wall-running or free movement expansion implied.

## Collectible passive skills (5)
- Paper Double: Substitution trades some mitigation for a short delayed neutral decoy impact on attacker, one eligible hit only; no full damage reflect.
- Scattersteel: Kunai Volley trades some first-target damage for more fan coverage and distinct-target hits, shared hit cap.
- Cinder Seal: Flame Breath trades some direct impact for longer residual Burn application, fixed application budget and no per-tick refresh.
- Hidden Step: Smoke Veil trades zone duration for a short movement/recovery benefit on leaving its footprint; no forced movement outside zone or evasion event from empty space.
- Twin Technique: Mirror Double trades some direct damage for a longer usable Echo lifetime within cap; if Echo already exists, modestly enhances next complementary action rather than adding second Echo. No self-trigger or repeated indefinite refresh.

## Example builds and automation
- Phantom striker: Silent Blade / Kunai Volley, Mirror Double, Phantom Formation / Phantom Arts / Warfare, Tempo. Dagger.
- Ninjutsu: Sealbreaker / Flame Breath, Stormstep, Wind Cutter / Phantom Arts / Flow, candidate Influence if approved (otherwise Warfare). Both weapons; can trigger existing Fire+Lightning Overload or Fire+Resonance Wildfire only through actual valid application; no special reaction bypass.
- Evasive martial: Silent Blade / Substitution, Flash Palm, Tempest Palm / Escape Artist / Endurance, Tempo. Gauntlet; baseline defense on cooldown if no targeted attack, conditional timing improves manual/auto.
- Mixed Dagger/Gauntlet with compatible inherited Assassin actives possible. Weapon slot assignment, inheritance and exact mixed scaling remain open. Auto generic executor prefers Core finishers before compatible skills without waiting indefinitely; no new manual input required. Preserve action/zone/recovery constraints.

## Talent tree — Hidden Arts (working name)
Innate bonus Evasion and Energy Efficiency. Independent class forks; base and first expansion use approved P0/P I cost profiles. Promoted-class section eligibility open; no availability before acquisition implied. All legal routes cost 30 TP; effects provisional.

### Base (1–3 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [1] ATK; [1] Energy; [2] Evasion |
| Fork 1 L — Phantom Arts | [1] Effect Duration; [1] Echo complementary impact effectiveness; [2] Echo lifetime within cap; [3] Double Formation: eligible Echo-assisted projectiles or area techniques allocate their complementary impact to a second angle or nearby target, with isolated-target fallback; no full duplicate cast |
| Fork 1 R — Martial Arts | [1] Attack Speed; [1] Core finisher damage; [2] Martial technique recovery; [3] Flowing Seal: completing a Core sequence shortens the hand-seal windup of the next eligible paid martial/ninjutsu technique within animation floors; no cooldown reset |
| Shared | [1] Energy Recovery; [2] Technique damage; [2] Echo complementary action effectiveness |
| Fork 2 L — Substitution | [1] Movement Speed; [2] Evasion during defensive skills; [2] Substitution mitigation effectiveness; [3] False Retreat: Echo-assisted Substitution leaves a brief deceptive smoke footprint that weakens eligible ordinary targeting attacks against Shinobi via Accuracy/Evasion interaction; no threat wipe or invisibility immunity |
| Fork 2 R — Ninjutsu | [1] MATK; [2] Effect Potency; [2] Elemental technique coverage; [3] Dual Weave: eligible Echo-assisted elemental techniques redistribute a bounded portion of the original application budget to the Echo's impact area; never double-apply on the same target or grant an extra reaction |
| Conclusion | [1] Energy Efficiency; [2] Penetration; [3] Silent Art: after consuming an Echo, the next distinct Core finisher gains improved impact or preparation property, no additional Echo generation beyond normal finisher |

### First expansion (2–6 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [2] ATK and MATK; [2] Evasion |
| Fork 1 L — Phantom Arts | [3] Echo impact effectiveness; [5] Mirror Formation: eligible area techniques split the authored Echo action across two visual copies attacking separate nearby targets; shared damage/application budget and one Echo consumption, isolated fallback concentrates existing budget |
| Fork 1 R — Martial Arts | [3] Martial technique effectiveness; [5] Seal Breaker: after a completed Core sequence, eligible close-range ninjutsu transitions into its next martial strike with reduced recovery; no extra actions or cooldown resets, obey existing Impulse rules |
| Shared | [2] Energy Efficiency; [2] Echo lifetime and effectiveness |
| Fork 2 L — Substitution | [4] Substitution protection and defensive duration; [6] Counterfeit: Echo-assisted Substitution may replace the normal retreat with an eligible short lateral relocation and a delayed decoy strike against the attacker; one ordinary-hit trigger, capped mitigation, no scripted immunity; stationary fallback uses the strike without relocation |
| Fork 2 R — Ninjutsu | [4] Ninjutsu impact and elemental application; [6] Crossing Seals: eligible Echo-assisted elemental techniques place the complementary impact in a second valid area selected by enemy distribution; the original and Echo share application budget and cannot independently react on the same target from this activation, solo fallback concentrates existing impact |
| Conclusion | [4] Master of Deception: completing the first Core chain after an Echo-assisted technique grants a bounded preparation bonus to the next eligible technique; no additional Echo, no recursive chain extension |

## Reference study and critical review
- Naruto to Boruto: Shinobi Striker official developer letters on clone-assisted tools and substitution balancing: https://naruto-official.com/en/news/01_2669 and https://naruto-official.com/en/news/01_2713 ; https://naruto-official.com/en/news/01_1695 (reduced clone explosion radius). Learn the fantasy of complementary clones and defensive reversals without oversized free offense. Naruto Storm Connections substitution and resource adjustments: https://en.bandainamcoent.eu/naruto/news/naruto-x-boruto-ultimate-ninja-storm-connections-patch-120-notes . 
- FFXIV Ninja official job guide https://na.finalfantasyxiv.com/jobguide/ninja/ and community guide https://www.thebalanceffxiv.com/jobs/melee/ninja/skills-overview/ : expressive hand seals, but invalid inputs can fail into Rabbit Medium. Keep seal animation and authored techniques without manual input punishment in auto.
- Sekiro official https://www.sekirothegame.com/ and https://support.activision.com/content/atvi/support/web/en_gb/sekiro/articles/using-the-shinobi-prosthetic-in-sekiro-shadows-die-twice.html : tools complement sword/martial offense. Black Desert Ninja https://cert-www.console.playblackdesert.com/GameInfo/Class?classType=26 : agile approach and concealment, not copied full stealth.
- Warframe official Ash revisions https://www.warframe.com/uk/patch-notes/pc/38-5-0 (one mark per target, cancelable player participation), community feedback https://forums.warframe.com/topic/1448074-ash-blade-storm-improved-usability/ (players report slow resolution and teammates killing targets first; anecdote, not universal verdict). Avoid marking overhead, animation lock and slow independent clone AI.
- Guild Wars 2 https://wiki.guildwars2.com/wiki/Shadowstep and https://wiki.guildwars2.com/wiki/Game_updates/July_2026 (melee Deadeye Mark awkwardness addressed with gap close). Test both weapons and close/ranged fallback; no forced positional mechanics. GGM remains accessible build/auto reference.
- Main risks: Echo turns into generic double damage or expensive VFX; defensive mitigation becomes permanent immunity; physical/magic split creates gear tax; prep slows farming. Test clone resolution, actual damage budget, targeting in co-op, boss immunity, no incoming attack, forced zones, low energy, weapon-only builds, class swapping and mobile performance. Ensure Mirror Double competes for scarce slots and defensive path isn't dead in raid DPS.
- Major talent concerns: Double Formation/Mirror Formation/Crossing Seals overlap; distinguish targeting, number of visual copies and application vs damage budgets, simplify if redundant. Counterfeit must not provide free evade credit, excess damage or positional bypass. Explicitly define recovery and geometry floors, caps and per-skill fallbacks. Eight static route-cost checks passed; no gameplay tests or numerical validation.
