# Oracle — Prestige I kit (working draft)

Status: assistant proposal, pending owner review and playtesting. Cleric -> Oracle -> Exorcist is established working lineage. Conditional blessings and preemptive support are established broad Oracle identity. All specific traits, skills, weapon/growth choices and talent effects below are proposals. All native Legendary skills use either compatible weapon per owner rule. [Cleric](CLERIC.md), [Classes](../CLASSES.md), [Talents](../TALENTS.md), [Elements](../ELEMENTS.md).

## Profile
Proactive support / magical DPS. Cleric restores immediate losses; Oracle prepares future responses; Exorcist retains hostile suppression, Paladin frontline protection, Sage allied ability amplification. Proposed Tome primary, Magic Staff secondary; compatible inherited Cleric ordinary actives only, no Divine Favor or exclusive class passives. Shield-specific ancestral skills retain their restriction. Health C(3), Energy B(4), ATK F(1), MATK A(5), DEF D(2), MDEF B(4) = 19 (owner-approved Energy/MATK grade swap). Proficiencies Effect Duration, Energy Efficiency, Cooldown Reduction, Resistance. Healing scales MATK, no new universal attributes.

## Trait — Providence
Core sequence completion grants one temporary personal-source Blessing of Providence to an eligible recipient (self or ally in range). Auto prioritizes endangered allies, then active combatants, with self fallback; optional manual selection within standard targeting. Same-source refresh, bounded active count (propose one per Oracle); no party-wide blanket stacking. Blessing consumes once on first eligible event:
- Adversity: qualifying hostile ordinary hit against recipient, bounded mitigation evaluated before final Health loss; no lethal prevention, automatic resurrection or scripted immunity. Exclude incidental tiny ticks using configurable threshold, but ordinary chip remains eligible if threshold met.
- Opportunity: recipient lands qualifying direct damaging ordinary active while sufficiently healthy, gains bounded primary impact bonus; evaluate Health at commitment, once per activation, no proc-on-proc. No ally proc triggers from pets, DoT, secondary effects. On miss no benefit; use consistent consumption policy.
- Resolve earliest eligible event deterministically; no both outcomes, no stacking via multi-hit; same-type blessings from multiple Oracles refresh/strongest or share cap (proposal; global same-source/independent-modifier rules require reconciliation). Paid skill blessings are distinct effects with budgets and explicit compatibility, never counted as fresh Providence. On inactive Oracle, already applied blessings may resolve during normal lifetime, no new creation while inactive. Avoid passive generation from healing, reaction, Echo/Clone or pet events. No new resource meter.
- Concern: healthy targets may consume offensive blessing before incoming boss attack; defensive selectable passive and manual targeting give control. Simple rotation should work without predicting exact attack timers.

## Selectable class passives (2)
- Seer: baseline Resistance; Providence prioritizes Adversity (offensive trigger disabled until its late lifetime window), stronger capped mitigation. Solo benefit; no protection duplication.
- Harbinger: baseline Penetration; Providence improves Opportunity impact, even self, with shorter lifetime; defensive outcome retained when hit first. No party-wide offensive stacking.
Exact thresholds, lifetime, relative output and interaction with other source buffs TBD.

## Legendary Core skills (2, either weapon)
- Guiding Star (guaranteed): balanced Light magical chain, finisher applies Radiance and grants Providence; modest baseline primary damage, no additional heal from Radiance alone.
- Astral Reading (alternative): neutral magic chain, finisher creates Providence and improves next eligible paid delayed sigil's application/recovery property; no free cast. Useful solo, neither Core guarantees reaction. Tome/Staff weapon-family animations reused.

## Ordinary active skills (10; 3 equipped)
| Grade | Skill | Weapon | Function |
| --- | --- | --- | --- |
| Normal | Premonition | Either | Prepare a single ally for next qualifying hostile hit: limited personal shield created just before damage resolution, capped budget; expires into small brief Resistance bonus if untriggered. Self fallback. |
| Normal | Fortune's Light | Either | Light projectile applying Radiance; stronger direct impact if caster has an active paid blessing or Providence on an eligible recipient at commitment. Does not consume allied blessing unless it is own eligible Providence. |
| Normal | Guiding Word | Either | Temporary targeted blessing: next eligible direct active by recipient gains bounded Accuracy and Penetration; expires on qualifying use or timeout. Self eligible, no proc recursion. |
| Normal | Deferred Grace | Either | Prepare targeted restorative blessing; triggers modest MATK heal after recipient suffers qualifying Health damage below a threshold, or on expiry if injured. Baseline small direct heal when already critically injured. Single total healing budget. |
| Rare | Omenfall | Either | Place visible prophetic sigil at target area; after short delay deals concentrated Light damage plus partial area impact and Radiance. Baseline damage if no ally attack; no unavoidable targeting. |
| Rare | Protective Constellation | Tome | Place short-lived supportive field that grants a bounded ward to first eligible allies exposed to qualifying damage within it; finite aggregate budget, self included, no repeated per-tick ward. |
| Rare | Reprieve | Either | Prepare recipient to reduce duration/potency of next eligible harmful status through existing Resistance rules; on expiry if unused, brief Resistance bonus. Moderate direct heal on cast if injured, balanced alongside status protection and its expiry fallback; not a universal cleanse. |
| Rare | Fate's Turning | Either | Direct neutral magical impact; if a paid blessing resolved recently, concentrates part of existing impact into Armor depletion or primary damage against Broken foe. Does not refresh a blessing. |
| Legendary | Divine Intervention | Either | Place a powerful prepared restoration on selected ally and limited nearby allies with explicit aggregate cap. On qualifying Health damage, releases bounded MATK recovery after surviving hit; unused portion resolves on expiry only against actual missing Health. Baseline immediate modest heal if injured. No death save, rewind or double counting prevented damage. |
| Legendary | Celestial Verdict | Either | Mark valid enemy area with a visible omen; after short delay delivers a Light burst, with concentrated additional impact if an allied direct damaging active lands within preparation window. Self attacks qualify; one event only, useful baseline without ally. No repeated bonus per party member. |
Both Legendary actives and both Core choices work with either native compatible weapon. All skills follow standard Energy, cooldown, Impulse, geometry, normal damage/status and healing rules. No guaranteed survival or hidden prophecy prediction. Resolve ward creation before damage, actual healing only after surviving hit, clear on death. All quantities provisional.

## Collectible passive skills (5)
- Prepared Haven: Premonition trades some single-hit shield for longer readiness and a small residual shield, one capped budget.
- Auspicious Word: Guiding Word trades part of Accuracy for stronger Penetration against intact Armor; no separate stat.
- After the Storm: Deferred Grace trades immediate critical-health heal portion for greater reserved recovery, capped and self eligible.
- Falling Star: Omenfall trades area radius for shorter delay and concentrated primary impact; no guaranteed hit.
- Mercy of Fate: Divine Intervention trades some distributed ally coverage for stronger primary-target recovery; isolated fallback useful, never multiplies damage conversion.

## Builds
- Guardian Seer: Astral Reading / Premonition, Deferred Grace, Divine Intervention / Seer / Endurance, Flow. Both weapons.
- Herald: Guiding Star / Fortune's Light, Guiding Word, Celestial Verdict / Harbinger / Warfare, Opportunity. Solo and party.
- Prophetic Controller: Astral Reading / Omenfall, Reprieve, Fate's Turning / Seer or Harbinger / Flow, Warfare. Distinct delayed damage and status defense; Fate's Turning baseline works even without paid blessing resolving.
Auto uses existing sequence executor and target selection. No exact boss-timer knowledge needed; cast on ordinary cadence, optionally prioritize valid endangered recipients or already prepared effects. Never force ally reposition, withhold healing, or stall while waiting indefinitely for trigger. Test solo, no incoming hits, uninjured groups, tank-focused damage, raid-wide hits, simultaneous Oracles, multiple low-Health allies, death/expiry, class swaps, scripted mechanics, PvP if applicable. Support credit for actual effective heal/mitigation and contribution is open; avoid rewarding overheal, repeated buff refresh, or farming ally damage.

## Talent tree — Threads of Fate (working name)
Innate bonus Effect Duration and Energy Efficiency. Standard independent forks; base and expansion use established P0/P I cost profiles; promoted-class availability open. All routes 30 TP.

### Base (1–3 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [1] MATK; [1] Energy; [2] Effect Duration |
| Fork 1 L — Premonition | [1] Resistance; [1] Blessing protection; [2] Adversity trigger effectiveness; [3] Forewarned: eligible prepared wards prioritize damage from a committed enemy attack over incidental chip; if no qualifying attack occurs, ordinary expiry fallback still applies |
| Fork 1 R — Fortune | [1] Penetration; [1] Light damage; [2] Opportunity impact; [3] Fortunate Strike: eligible damaging blessings allocate a bounded portion of their impact to Armor depletion on intact foes or primary damage on Broken foes |
| Shared | [1] Energy Recovery; [2] Blessing lifetime; [2] MATK |
| Fork 2 L — Deliverance | [1] Health; [2] Prepared healing effectiveness; [2] Resistance during blessing; [3] Shared Burden: eligible single-target recovery blessings distribute a capped portion of unused restoration to another injured ally, never creating a second blessing; self-only fallback strengthens original heal within cap |
| Fork 2 R — Prophecy | [1] Effect Potency; [2] Direct spell damage; [2] Prophecy impact; [3] Written Fate: eligible offensive delayed sigils concentrate their existing impact on the marked primary target when it leaves their initial footprint but remains in valid range; no guaranteed hit or forced movement |
| Conclusion | [1] Energy Efficiency; [2] Blessing effectiveness; [3] Provident Cycle: after a paid blessing resolves, next distinct Core finisher improves its existing protection or damage property, once per cycle, no free new blessing outside Trait |

### First expansion (2–6 TP)
| Segment | Nodes in order |
| --- | --- |
| Opening | [2] MATK; [2] Energy |
| Fork 1 L — Premonition | [3] Prepared ward mitigation; [5] Second Sight: eligible prepared wards divide their single protection budget between a primary qualifying hit and a short residual barrier against subsequent ordinary hits; no new budget or reset, no lethal immunity |
| Fork 1 R — Fortune | [3] Offensive blessing effectiveness; [5] Fortune's Turn: eligible offensive blessings may preserve a bounded portion of their existing bonus for the next distinct damaging action when the first targets intact Armor and fails to deal Health damage; no full duplicate proc |
| Shared | [2] Energy Efficiency; [2] Effect Duration |
| Fork 2 L — Deliverance | [4] Prepared restoration effectiveness; [6] Foreseen Recovery: eligible recovery blessings can resolve a bounded portion immediately when the recipient falls below the urgent threshold, reserving the rest for expiry; one total healing budget, no overheal or two trigger credits |
| Fork 2 R — Prophecy | [4] Delayed damage skill effectiveness; [6] Constellation: eligible offensive sigils may redistribute part of their paid area impact to one additional valid target associated with a separate ally's attack; no extra original-target impact, isolated fallback concentrates unused coverage within cap |
| Conclusion | [4] Fatekeeper: first distinct paid blessing after Providence resolves gains bounded duration or activation effectiveness; no recursive blessing generation or shared cooldown reset |

## References, failures and review
- FFXIV Astrologian official job guide https://na.finalfantasyxiv.com/jobguide/astrologian/ (Earthly Star, delayed restoration, compiled damage; adapt timing not exact formulas).
- WoW developer notes https://news.blizzard.com/en-us/article/24020034/updated-nov-7-dragonflight-guardians-of-the-dream-content-update-notesnow-live and https://news.blizzard.com/en-us/article/24179386/undermine-d-content-update-notes (simplify ramp, fewer cooldowns); https://us.forums.blizzard.com/en/wow/t/class-changes/2318018 (developer identifies Penance targeting friction and proc reliance). Avoid mandatory long setup, predictable baseline support, direct ally/enemy targeting.
- GW2 Chronomancer https://www.guildwars2.com/en-gb/news/meet-the-chronomancer-mesmers-elite-specialization/ and https://wiki.guildwars2.com/wiki/Chrono (future outcomes and timed fields; no time rewind or forced invulnerability).
- Overwatch Zenyatta https://overwatch.blizzard.com/en-us/heroes/zenyatta/ and October 2023 balance https://overwatch.blizzard.com/en-us/news/patch-notes/live/2023/10/ (targeted support with offensive participation and counterplay). Keep targeted blessings readable and bounded.
- PoE2 support compatibility and reservation tradeoffs https://www.poe2wiki.net/wiki/List_of_support_gems (community reference, not exact rules). Three active slots are sufficient opportunity cost; no new Spirit resource. Mythological oracles/omens as fantasy, not mechanics.
- Major risk: reactive blessings are just automatic shields/heals, or offensive blessings become compulsory DPS amplification. Make timing, visible trigger, tradeoffs and solo fallback meaningful; distinguish Oracle from Cleric, Paladin, Sage, Exorcist. Compare time-to-kill, effective healing/mitigation, uptime, target selection, cost and party-size scaling. Second Sight/Foreseen Recovery split one budget rather than double it. Fortune's Turn must not preserve bonus against immune foes indefinitely. Eight static route-cost checks passed; no numeric or gameplay validation.

## Support healing budget
Owner direction: healing effectiveness reflects the skill's overall utility budget. Dedicated single-target healing has high per-target throughput; dedicated AoE healing has strong aggregate throughput with appropriate per-target tuning. A skill combining healing with one substantial secondary purpose (e.g. cleansing OR protection) should generally deliver moderate healing, not low healing. Reserve low healing for skills combining roughly three meaningful functions or incidental healing; tune by actual strength, coverage, duration, Energy and cooldown rather than mechanically counting labels. This is qualitative guidance, not coefficients.
