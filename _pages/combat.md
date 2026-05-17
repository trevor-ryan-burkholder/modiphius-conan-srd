---
title: "Combat"
chapter: "Chapter IX"
subtitle: "Attacks, defenses, and the specific ways a sword meets a shield."
---

This page covers the *mechanics* of a single attack — how to roll one, how the target resists, what specific moves are available beyond "I swing." For turn order, zones, and movement, see [Action Scenes](/action-scenes/). For wound tracking and recovery, see [Damage, Wounds & Recovery](/damage-and-recovery/).

## The basic attack

An attack is a skill test. The attacker rolls **2d20** against a target number set by attribute + skill, against a difficulty set by the defender.

| Attack type        | Skill           | Default attribute |
| ------------------ | --------------- | ----------------- |
| Melee weapon       | Melee           | Agility (or Brawn for power) |
| Thrown weapon      | Ranged Weapons  | Coordination      |
| Bow / crossbow     | Ranged Weapons  | Coordination      |
| Unarmed strike     | Melee           | Brawn             |
| Grapple            | Melee           | Brawn             |
| Spell (offensive)  | Sorcery         | Willpower         |

### Default difficulties

A standing target in the open at the appropriate range is **D1**. The difficulty increases for:

- **Cover** (light cover +1, heavy cover +2, near-total cover +3).
- **Range** (a weapon used beyond its sweet spot, see weapon properties: +1 or +2).
- **Concealment** (poor light, smoke, foliage: +1 or +2).
- **Target's defenses** (most relevant for spells and exotic attacks).
- **Restrained, prone, helpless target** (–1 difficulty; often D0).

A target who **Parries** or **Dodges** as a Reaction sets the difficulty themselves — they make a test against D1 and each success they roll raises the attacker's difficulty by 1.

## Successful hits — damage

Hits inflict damage in **Combat Dice [CD]**. A weapon line reads, e.g., "Broadsword — 4 [CD], 1H, Parrying, Vicious 1." The 4 [CD] is the base damage pool, rolled and summed using the [CD reading](/core-mechanic/#combat-dice-challenge-dice).

You may **add to the damage pool**:

| Bonus damage source              | Effect                       |
| -------------------------------- | ---------------------------- |
| Each Momentum spent on the hit   | +1 [CD] (no cap, but expensive) |
| Surprise / unaware target        | +1 [CD]                      |
| Bonus from talent or spell       | varies                       |

Then the defender **Soaks** the damage: subtract their armor's *Armor Soak* (physical) or *Courage* (mental) value from the damage rolled, then apply the rest to **Vigor** (physical) or **Resolve** (mental). When Vigor or Resolve drops to 0, see *Wounds* and *Traumas* in [Damage, Wounds & Recovery](/damage-and-recovery/).

## Special attack types

Beyond "I swing," a number of structured attack maneuvers are available. Most cost Momentum on top of a successful basic attack.

| Maneuver        | Cost           | Effect                                                                                  |
| --------------- | -------------- | --------------------------------------------------------------------------------------- |
| **Disarm**      | 2 Momentum     | On a hit, the target drops or loses their weapon.                                       |
| **Knockdown**   | 1 Momentum     | On a hit, target is *Prone*. Standing back up is a Minor Action.                        |
| **Push**        | 1 Momentum     | Shove target one zone away, or out of Reach with you.                                   |
| **Grapple**     | (Standard)     | Opposed Melee. Success: target is *Restrained*. Maintain with a Minor Action each turn. |
| **Pin**         | 2 Momentum     | After Grapple, target is also *Helpless* until they escape.                             |
| **Aim**         | (Minor Action) | Next ranged attack this turn: +1d20.                                                    |
| **All-out**     | (declared)     | +1 [CD] damage on this attack, but defenses drop by 1 step until your next turn.        |
| **Defensive**   | (declared)     | Sacrifice this turn's Standard Action; +1 [CD] to your next defensive Reaction roll.    |
| **Called shot** | 2 Momentum     | Specify a location; on hit, apply an appropriate Effect (blind, hobble, disarm).        |

## Effects (5–6 on [CD])

Each face of 5 or 6 on a Combat Die triggers any **Effect** the attack carries. Effects are properties of the weapon, spell, or talent.

| Effect       | Trigger                | Result                                                            |
| ------------ | ---------------------- | ----------------------------------------------------------------- |
| **Vicious X** | per Effect rolled      | +X damage on that die (most lethal property; rarely above 2).     |
| **Knockdown** | first Effect rolled    | Target falls *Prone*.                                             |
| **Stun**      | first Effect rolled    | Target's next test is at +1 difficulty.                           |
| **Piercing X** | per Effect rolled     | Reduces target's Armor Soak by X for this attack.                 |
| **Intense**   | first Effect rolled    | Damage is delivered as mental (Resolve) instead of physical.      |
| **Fearsome X** | first Effect rolled   | If damage causes a Wound/Trauma, also deal X [CD] mental damage.  |
| **Grappling** | first Effect rolled    | On hit, may immediately *Grapple* for free.                       |
| **Toxic X**   | first Effect rolled    | Damage ignores X armor; lingering poison effects per setting.    |
| **Unforgiving X** | first Effect rolled | If the attack fails to overcome Soak, the target still takes X.   |

Effects do not stack with themselves on a single attack unless the entry says "per Effect rolled."

## Defenses summarized

| Defense       | Trigger / use                                | Cost                |
| ------------- | -------------------------------------------- | ------------------- |
| **Parry**     | Reaction to melee attack                     | 1 Reaction (free 1/round) |
| **Dodge**     | Reaction to any attack                       | 1 Reaction (free 1/round) |
| **Counter-spell** | Reaction to incoming spell               | 1 Reaction; Sorcery test |
| **Protect**   | Take an attack meant for an adjacent ally    | 1 Reaction          |
| **Cover**     | Static; raises attacker's difficulty         | None (positional)   |
| **Armor**     | Static; reduces incoming damage              | None (worn)         |

A single defender may make a second Reaction in the same round by spending 1 Momentum.

## Healing and recovery during a fight

Healing in the middle of a scene is rare and limited:

- **First Aid**: Standard Action, *Healing* test (D1 or higher depending on wound), restores some Vigor.
- **Patch up**: Minor Action, spend 1 Momentum to restore 1 [CD] of Vigor on a willing adjacent ally.
- **Rallying word**: Standard Action, *Command* test, restores Resolve to allies who can hear you.

Most real recovery happens between scenes. See the recovery page for details.

## Quick reference

- **Attack** = Skill test, default D1 (modified by cover, range, Parry/Dodge).
- **Damage** = base [CD] + bonuses; defender Soaks, remainder hits Vigor/Resolve.
- **5–6 on a [CD]** triggers Effects.
- **Reactions** are 1/round free, +1 per Momentum/Doom spent.
- **All-out** trades defense for +1 [CD].
