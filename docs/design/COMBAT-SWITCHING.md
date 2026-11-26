# Combat switching proposal
Started 2026-11-25; updated 2026-11-26 | Class-linked weapons confirmed; switching details exploratory.

## Owner intent
Make automated hack-and-slash combat more lively and dynamic by enabling in-combat class and/or weapon swaps. Swapping extends combos and gives access to available skills in the incoming kit instead of all classes/weapons being held by the outgoing kit's cooldowns. Players grind to unlock more swap options. Tentative caps: 3 classes and 2 weapons. The owner has not decided whether switching is class-based, weapon-based, or both.

## Compatibility
Class expansion and retained progression are established in [CLASSES.md](CLASSES.md). Current primary/secondary weapon assignments in [WEAPONS.md](WEAPONS.md) are canonical.
Shared weapons may support common base movesets while classes supply distinct skills/modifiers. For example, Warrior and Rogue share Sword, while Rogue and Ranger share Dagger. A class swap may change weapon if necessary, or use an already compatible weapon; whether both swaps are independent remains open. Shared weapon skills should retain cooldowns, distinct class skills have independent cooldowns (recommended). If two weapon slots are global, three equipped classes need compatible coverage; scope remains open.

## Models to evaluate (constrained by class-linked compatibility)
| Model | Description | Key tradeoff |
| --- | --- | --- |
| Class swap | One character rotates between equipped class kits; each has its own abilities. | Strong expression of multi-discipline mastery; classes have compatibility mappings. |
| Weapon swap | One active class, two equipped weapons with distinct movesets/weapon skills. | Easier visual continuity; class switching may happen separately. |
| Both | Up to three class selections and two weapon selections, with a defined relationship. | More build variety but potentially large interaction and balance cost. |
| Bound kits | Each equipped discipline has a defined compatible weapon or loadout; one swap changes the kit. | Lower control complexity; less freedom than independent swapping. |

Do not assume six separate cooldown banks from 3 classes x 2 weapons. Do not assume the caps apply to lifetime unlocks; the interpretation as equipped swap slots is provisional.

## Cooldown semantics (recommended baseline, not confirmed)
- Each distinct ability/kit owns its cooldown; leaving a kit does not impose that cooldown on unrelated incoming skills.
- Outgoing timers continue to tick while inactive; returning does not inherently reset them.
- Incoming kit may feel refreshed because its own abilities are available, not because swapping magically erases cooldowns.
- Energy is the universal skill resource; shared pool across swaps recommended. Shared abilities, swap lockouts and special reset effects need explicit policies.
- Distinguish a global skill cooldown pool from a short action recovery or swap lockout. The owner rejects the former for the desired swap behavior; the latter is undecided.
- Persistent server-authoritative timers and stable ability IDs are technical recommendations, not implementation.

## Illustrative combat sequence
Warrior opens with a dash and launch; uses its available skills. Switch to an illustrative Mage kit for an aerial/area follow-up while Warrior abilities recover. Switch to an illustrative third discipline for a finisher or continued pressure; return to Warrior if its abilities have recovered. No actual class names, ability counts, timers or mechanics are confirmed by this example.

## Subbranches to explore
- Progression: initial slot count; second/third class slots; second weapon slot; mastery vs quests vs milestone/grind requirements; equipped vs learned disciplines; loadouts and out-of-combat reconfiguration.
- Combo flow: swap timing, cancel windows, transition animations, carry target/position/momentum, launch and stagger interactions, follow-up attacks, optional swap attacks, failure/recovery.
- Cooldowns: per-ability vs per-kit ownership, ticking while inactive, duplicate skills, shared resources, swap restrictions, re-equipping and disconnect persistence.
- Automation: rotate when kit exhausted vs prioritize damage windows/enemy needs; configurable sequencing; avoid excessive swaps; manual overrides; automatic resumption; should one kit remain viable?
- UI/control: clear active kit, available kits, cooldown indicators, mobile/PC/console inputs, future full manual compatibility.
- Balance: action uptime, burst stacking, optimal rotations vs single-class investment, crowd-control chains, invulnerability/cancel abuse, PvE and co-op synergy, skill budget per kit.
- Technical: shared action interface, ability state ownership, authoritative transitions, animation and replication, AI decision rules, performance, tests.

## Prototype questions
1. Is swapping classes, weapons, or both the actual combat identity?
2. If both, are weapon and class selection independent or bound? Which skills belong to each?
3. Is swapping automatic, manual, or available in both? What triggers it?
4. Is the initial progression one class/weapon, and which milestones grant slots?
5. Are there swap attacks, short lockouts, or combo-cancel windows? What remains active across swaps?
6. What resource and cooldown behavior creates continuous combat without endless unrestricted burst?
7. How much benefit should extra slots confer, and can a specialist still be viable?

## Suggested prototype validation
Compare one kit vs two kits with the same enemy encounter; measure damage uptime, idle gaps, transition readability, cooldown accuracy, AI swap churn, manual override behavior and co-op/network stability. Add a third class and two weapons only after the fundamental relationship is understood. These are suggested tests, not an approved launch scope.
