# Combat switching and shared loadout
Updated 2026-11-26. Owner-confirmed loadout architecture; detailed execution and balance open.

## Established
- Maximum two equipped class selections and two shared weapon slots for now. This is not a limit on learned classes; hybrid classes remain planned.
- Player selects two classes, two compatible weapons and each class's skills. Equipment, weapons, armor, accessories, pet, mount and future relics are shared and remain equipped when switching classes. Class selections have their own skill slots and class-specific talent loadouts.
- Selecting the same class twice is permitted and provides a scaling specialization buff instead of another kit or cooldown bank. Cooldown reduction is a candidate additional benefit; magnitude, affected coefficients and stacking are open. Do not duplicate skills or class benefits.
- Class swapping has a 0.5-second cooldown. Each weapon has one weapon skill. Weapon skill ownership, active weapon selection and whether weapon switching shares that cooldown are open.
- Swapping accesses the incoming class's selected skills. Recommend individual ability cooldowns continue during inactivity and never reset simply due to swaps; shared weapon skills retain their cooldowns across class swaps. Shared Health/Energy and persistent applied statuses/effects recommended, subject to explicit skill rules.

## Compatibility and execution
See [Weapons](WEAPONS.md) for class-linked weapon families. The two equipped weapons remain the same throughout class swaps; no per-class gear replacement. Recommend validating that each distinct selected class can use at least one equipped weapon. Whether swaps automatically select a compatible weapon, or require separate weapon selection, is open. Do not require both classes to share a weapon. Each weapon supplies one skill, not an additional class kit.

## Open
- Automatic vs manual swap triggers, independent weapon swap rules, cooldown scope for weapon switching, cancel/recovery windows, target continuity and animations.
- Class skill counts, passive/trait activation scope, talent preset switching restrictions, persistent effects, specialization buff and potential cooldown reduction.
- Shared weapon attribute contribution (both equipped vs currently wielded), weapon skill activation/slot presentation, duplicate weapon eligibility.
- Slot unlock milestones and out-of-combat loadout editing restrictions.
- Prototype compare same-class specialization vs two distinct classes for uptime, survivability, role utility, automation and readability. Maintain server-authoritative cooldowns and prevent re-equipping/reset abuse.
