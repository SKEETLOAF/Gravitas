# Talent trees

Status: owner accepted the revised conceptual design on 2026-11-27. This is a design specification, not implementation or numerical validation. It supersedes the older shared-lineage, multi-rank, level-10 and 16-TP layouts. Detailed class and universal effects: [TALENT-CATALOG](TALENT-CATALOG.md). Older files under talents/ are historical references only, not implementation input.

## Architecture (approved direction)
- Each individual class (foundation, promotion, hybrid, special) has its own tree. Universal trees are reusable, linear internally, and independent of class-specific Traits or named skills. Both kinds may modify skill properties, provide attributes, conditional effects and major passives. Class trees specialize a discipline; universal trees specialize combat mechanics.
- Initial talent earning starts after P0 level 20. P0 and P I sections cost 30 TP each; P II onward 50 TP each. Preserve P0 single-purchase costs 1–3 TP and P I 2–6 TP. Later templates below are proposed; no arbitrary prestige tax.
- Each selected tree has an innate entry bonus separate from paid nodes; only selected trees grant it. Three selected trees per preset is a working recommendation, not confirmed cap. Additional universal trees/sections may unlock with progression; shared systems use Character Level and applicable stage gates; precise section eligibility open. Previously learned trees/purchases retained, descendants get distinct trees, not replacements.
- Class section: shared opening -> independent mutually restrictive left/right fork -> shared development -> second independent fork -> shared conclusion. Choosing left in one fork does not require left in the next. P0 segment costs 4/7/5/8/6; P I 4/8/4/10/4. Exact full legal route 30; unchosen branches do not count against completion. P0 has 25 visible nodes/17 bought per route; P I 13 visible/9 bought. Universal sections are linear, with no left/right choices; P0 costs 1,1,2,3,1,2,2,3,1,2,2,3,1,1,2,3; P I 2,2,3,4,2,3,3,5,6; each sums to 30. Each family uses the same node count, price sequence and fork shape at each corresponding prestige, independent of class identity. See [uniform template](#uniform-node-templates).
- Preserve ordinary skill acquisition, separate Class Trait, selectable class passives and collectible passive skills. Talents modify compatible acquired skills, not grant ordinary skills. No new mandatory meters or universal stats from a talent draft. Use canonical Health Regeneration, Penetration etc.; healing/shield/skill effectiveness are effect-specific modifiers, not new character stats.
- Recommended preset/respec UX: outside combat, preserve allocation per preset, preview full prerequisites and incompatible skills, route-aware completion, dynamic modified skill tooltips, future section previews. Exact unlock/respec costs open.

## Point economy (owner-approved 2026-11-27)
Independent lineage TP budgets retained through evolution. Talent earning starts after P0 level 20: levels 21–80 grant 60 TP. One TP per eligible level-up and one per successful Prestige rank-up; no extra award for resetting the displayed level to 1. Later stages earn from entry and levels 2 through cap. No fractional TP, variable rates or bonus milestone grants. Maximum ordinary class stage cap 150; permanent Character Level and continuous XP reference progression are separate.

| Prestige | Stage cap | TP earned in stage | Cumulative TP | New section cost | Full tree cost | Maxed trees |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| P0 | 80 | 60 | 60 | 30 | 30 | 2 |
| P I | 120 | 120 | 180 | 30 | 60 | 3 |
| P II | 150 | 150 | 330 | 50 | 110 | 3 |
| P III | 150 | 150 | 480 | 50 | 160 | 3 |
| P IV | 150 | 150 | 630 | 50 | 210 | 3 |
| P V | 150 | 150 | 780 | 50 | 260 | 3 |
| P VI | 150 | 150 | 930 | 50 | 310 | 3 |

Full tree means every applicable section through the current prestige. From P I onward each full tree costs exactly one-third of cumulative TP. P0 two trees, later three; zero surplus at the ordinary cap. Three selected trees per preset remains a proposed cap. Equal-cost sections assume native/universal rates; cross-tree premiums and promoted-tree availability require reconciliation.
- Hybrids retain independent progression and tier-equivalent grant. Updated P III entry grant is 331 TP (330 through P II plus one equivalent entry TP); do not award entry twice. Earlier proposed prefill of first two sections of both parent trees costs 120 TP, leaving 211. Prefill itself remains unapproved; immediate access to both parent trees confirmed. Earlier owner-confirmed hybrid cap 120 remains unchanged pending review: a P III-equivalent hybrid with that cap earns 119 further TP for 450 total, 30 short of three complete P III trees. Recommend aligning hybrid cap to 150 if same completion target applies, not silently changing it.
- Old 40 native/combined investment gates and 2/3 TP per rank cross-tree prices require reconciliation with single-purchase costs. Ancestral access at native cost is a recommendation. Non-parent access, pricing, respec and preset eligibility open.

## Progression cadence
Owner favors GGM-inspired milestone-led progression and separate uniform templates for class and universal trees. Talent earning starts after P0 level 20. Proposed first/second/third selection milestones at levels 20/40/60, with Class Change quest preparation around 60 and promotion eligibility at 80. Exact access gates remain open. Preserve learned disciplines and no server time locks.

## Uniform node templates
Owner approves uniform structure within each tree family. Existing P0 and P I templates unchanged; P II detailed allocation is a working proposal, with nine purchased nodes per route/section; later stages use the same 50 TP budget but their node counts and price schedules remain open. Branch alternatives have identical node count and cost sequence; effects must differ. Innate entry bonuses are separate, free on selection, not paid nodes.

| Section | Class shared opening | First fork (each side) | Shared development | Second fork (each side) | Conclusion | Visible / purchased | Total |
| --- | --- | --- | --- | --- | --- | --- | --- |
| P0 | 1,1,2 | 1,1,2,3 | 1,2,2 | 1,2,2,3 | 1,2,3 | 25 / 17 | 30 |
| P I | 2,2 | 3,5 | 2,2 | 4,6 | 4 | 13 / 9 | 30 |
| P II | 4,4 | 5,8 | 4,4 | 5,9 | 7 | 13 / 9 | 50 |

| Section | Universal linear node sequence | Visible / purchased | Total |
| --- | --- | --- | --- |
| P0 | 1,1,2,3,1,2,2,3,1,2,2,3,1,1,2,3 | 16 / 16 | 30 |
| P I | 2,2,3,4,2,3,3,5,6 | 9 / 9 | 30 |
| P II | 4,4,5,6,4,5,5,8,9 | 9 / 9 | 50 |

Owner clarification: uniformity means consistent structure, node counts and pricing conventions within each tree family at the same prestige, not identical prices for all nodes or identical density across all prestiges. Individual node prices vary by significance and generally increase with progression within a section and across prestige tiers; major branch effects and later unlocks should justify higher costs, while smaller shared nodes can remain cheaper even after a major node. Preserve exact legal route budgets of 30/30/50/50/...; both alternatives at each class fork must cost equally. P0 and P I existing schedules already use distinct prices. P II's nine-node template is proposed. Do not lock its specific prices or node count to every later prestige: with fixed 50 TP, raising average node price requires fewer purchased nodes (or redistributing costs for larger major nodes while retaining the same average). Review later sections individually, keep the two reconverging forks and meaningful node density; no arbitrary inflation or endless compression. No new P II node effects designed yet. If later balance requires a changed template, migrate all corresponding class or universal trees consistently rather than ad hoc exceptions. Section eligibility for promoted classes remains open.

## Multiclass and compatibility
Retain approved primary 100%, secondary 50%, same-class specialization 150% contribution weights. Proposed interpretation for binary ownership: scale eligible numeric coefficients, not the existence of the mechanic; one secondary extra strike at half strength rather than half a strike. Qualitative effects, thresholds, area, count rounding, overlapping universal nodes, external item bonus effects and contribution order require explicit rules. No automatic cross-class Trait or class-specific skill effects; only eligible skills/actions, respecting active class and persistent effect scope. Existing overlap intent retained, no duplicate recursive procs. Use skill tags (projectile, area, persistent, heavy impact, defense, healing, etc.) and per-skill overrides; tags and stacking not finalized. Respect encounter movement zones; auto must be able to use major effects. Modifier order and actual coefficients remain untested.

## Quality bar and references
Owner requires critical evaluation against polished RPGs; do not claim 9/10 without support. Review identity, real specialization choices, compatibility/no dead nodes, cost vs alternative investments including prerequisites, auto/manual utility, readable tooltips/visual effects, stacking/resource loops, implementation complexity, expansion and promotion identity. Conceptual assessment of latest class drafts ~8.6/10 (subjective, not measured). Expensive nodes should provide meaningful new properties or synergies, not merely bigger numbers. Smaller nodes support route identity. Test all four routes against bosses, farming, solo and co-op; balance high-frequency and long-cooldown skills; cap procs, refunds, status spreads, redirection, interception and stat conversion; avoid mandatory routes. No implementation or tuning validated.
- Primary: Go Go Muffin class disks + general disks, left/right decisions, resettable investments: https://boarhat.gg/games/go-go-muffin/class/ranger/ ; https://mobi.gg/en/tips/go-go-muffin-build/ ; https://boarhat.gg/games/go-go-muffin/guide/cc5-guide/ . Full node catalog not independently verified.
- Supplement: Black Desert skill add-ons/branch effects, Diablo IV skill variants, Last Epoch skill specialization, Torchlight: Infinite talent panels, Path of Exile 2 compatibility tags/supports, Wuthering Waves character-specific identity, AFK Dungeon automation. See [REFERENCES](REFERENCES.md).
- Completed P I kits. [Berserker](classes/BERSERKER.md) has a working kit and Primal Fury talent draft; [Hunter](classes/HUNTER.md) has a working kit and Hunting Grounds talent draft; [Elementalist](classes/ELEMENTALIST.md) has a working kit and Elemental Dominion talent draft; [Shinobi](classes/SHINOBI.md) has a working kit and Hidden Arts talent draft; [Oracle](classes/ORACLE.md) has a working kit and Threads of Fate talent draft; [pre-Prestige II audit](PRESTIGE-I-AUDIT.md) identifies decisions to resolve before further kits. Promoted-class section eligibility remains open. P II+ effects and numerical balance deferred; standard 50-TP template proposed.
