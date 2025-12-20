# Combat System

A resource-based combat system using Stamina, Mana, and HP instead of traditional action economy.

## Core Resources

### Hit Points (HP)
Your health and life force.

**Calculation:**
```
Max HP = 20 + (Endurance × 5) + (Fortitude × 2)
```

**Examples:**
- Endurance 5, Fortitude 2: **20 + 25 + 4 = 49 HP**
- Endurance 10, Fortitude 5: **20 + 50 + 10 = 80 HP**
- Endurance 20, Fortitude 15: **20 + 100 + 30 = 150 HP**

**Recovery:**
- Short Rest (10 minutes): Recover Endurance × 2 HP
- Long Rest (8 hours): Recover all HP
- Healing spells and potions
- Some passive abilities

### Stamina Points (SP)
Your energy for physical and mental exertion during combat.

**Calculation:**
```
Max Stamina = 10 + (Endurance × 2) + (Stamina secondary stat × 3)
```

**Examples:**
- Endurance 5, Stamina 3: **10 + 10 + 9 = 29 SP**
- Endurance 10, Stamina 8: **10 + 20 + 24 = 54 SP**
- Endurance 20, Stamina 15: **10 + 40 + 45 = 95 SP**

**Recovery:**
- **Automatically recover 50% of Max Stamina at the start of your turn** (round down)
- Long Rest: Recover all Stamina
- Special abilities can grant extra stamina recovery

**Usage:**
- Movement
- Attacks
- Abilities
- Reactions
- Defense maneuvers

### Mana Points (MP)
Your magical energy for casting spells.

**Calculation:**
```
Max Mana = (Intellect × 3) + (Awareness × 2) + (Arcana × 2)
```

**Examples:**
- Intellect 5, Awareness 3, Arcana 7: **15 + 6 + 14 = 35 MP**
- Intellect 12, Awareness 8, Arcana 15: **36 + 16 + 30 = 82 MP**
- Intellect 20, Awareness 15, Arcana 25: **60 + 30 + 50 = 140 MP**

**Alternative for Non-Casters:**
If Arcana is 0, use this formula instead:
```
Max Mana = (Awareness × 4) + (Presence × 2)
```
This allows divine/nature casters and non-arcane characters to have mana.

**Recovery:**
- Short Rest (10 minutes): Recover 25% of Max Mana
- Long Rest (8 hours): Recover all Mana
- Mana Potions (various amounts)
- Abilities like "Arcane Recovery" or "Meditation"

## Action Economy

**There are NO action/bonus action/reaction limits. Everything costs resources.**

On your turn, you can do anything you have stamina/mana/HP to pay for.

### Movement Costs

| Movement Type | Stamina Cost |
|---------------|--------------|
| 5 feet of normal movement | 1 SP |
| 5 feet of difficult terrain | 2 SP |
| Standing up from prone | 3 SP |
| Climbing 5 feet | 2 SP |
| Swimming 5 feet | 2 SP |
| Jump (per 5 feet) | 2 SP |

**Example:**
- Move 30 feet normally = 6 SP
- Move 15 feet + climb 10 feet + move 5 feet = 3 + 4 + 1 = 8 SP

### Attack Costs

**Basic Attacks:**

| Attack Type | Stamina Cost |
|-------------|--------------|
| Light Melee attack | 3 SP |
| Heavy Melee attack | 4 SP |
| Ranged attack | 3 SP |
| Unarmed strike | 2 SP |

**You can attack as many times as you have stamina for.**

**Example Turn:**
- Character has 54 max stamina, starts turn with 27 SP (50% recovery)
- Move 20 feet (4 SP): 23 SP remaining
- Heavy attack (4 SP): 19 SP remaining
- Heavy attack (4 SP): 15 SP remaining
- Heavy attack (4 SP): 11 SP remaining
- Saves 11 SP for reactions

**Extra Attack Ability:**
If you have the "Extra Attack" ability from the [[Ability Tree]]:
- Your first attack each turn costs 0 SP
- All subsequent attacks cost normal stamina

This makes Extra Attack valuable!

### Ability Costs

Abilities from the [[Ability Tree]] have their own costs:

**Martial Abilities (Stamina):**

| Ability | Cost |
|---------|------|
| Power Attack | 5 SP |
| Cleave | 6 SP |
| Whirlwind Attack | 8 SP |
| Riposte | 4 SP |
| Parry | 3 SP |
| Dodge | 4 SP |

**Spells (Mana):**

| Spell Level Equivalent | Mana Cost |
|------------------------|-----------|
| Cantrip | 0 MP |
| Level 1-2 spell | 5-8 MP |
| Level 3-4 spell | 10-15 MP |
| Level 5-6 spell | 18-25 MP |
| Level 7-8 spell | 30-40 MP |
| Level 9+ spell | 50+ MP |

**Some abilities also cost Stamina:**
- Fireball: 8 MP + 3 SP (to cast while in combat)
- Misty Step: 6 MP + 2 SP
- Shield (reaction): 5 MP + 2 SP

**Blood Magic (HP Costs):**
Some powerful abilities can be cast using HP instead of or in addition to mana:

| Ability | Cost |
|---------|------|
| Blood Bolt | 5 HP (no mana) |
| Life Drain | 10 HP + 5 MP |
| Sacrificial Shield | 15 HP (protect ally) |
| Death's Door | 50% current HP (massive effect) |

## Turn Structure

### Initiative
```
Initiative = d(Agility/2) + Agility/2 + d(Awareness/2) + Awareness/2
```

Highest initiative goes first. Ties: re-roll.

**Example:**
- Agility 10, Awareness 8:
- Roll: d5 + 5 + d4 + 4 = (1-5) + 5 + (1-4) + 4 = **11-18 initiative**

### Your Turn

**1. Start of Turn:**
- Recover 50% of Max Stamina
- Check for ongoing effects (poison, buffs, debuffs)

**2. Take Actions:**
- Spend stamina/mana/HP to do things
- No action limit - only resource limits
- You can move and attack in any order

**3. End of Turn:**
- Declare you're done
- Remaining stamina can be used for reactions

**Example Turn:**
Character has 54 Max SP, 82 Max MP

1. **Start:** Recover 27 SP (50% of 54)
2. **Move 25 feet:** 5 SP (22 SP left)
3. **Cast Fireball:** 8 MP + 3 SP (19 SP, 74 MP left)
4. **Move 10 feet:** 2 SP (17 SP left)
5. **Light Melee attack:** 3 SP (14 SP left)
6. **Light Melee attack:** 3 SP (11 SP left)
7. **End turn:** Save 11 SP for reactions

## Reactions

Reactions can be taken on other creatures' turns if you have stamina remaining.

**Common Reactions:**

| Reaction | Trigger | Cost |
|----------|---------|------|
| Opportunity Attack | Enemy leaves your reach | 4 SP |
| Parry | You're hit by melee attack | 3 SP (reduce damage) |
| Dodge | You're targeted by attack | 4 SP (impose disadvantage) |
| Shield Spell | You're hit by attack | 5 MP + 2 SP (+5 AC) |
| Counterspell | Enemy casts spell you see | 10 MP + 3 SP |

**You can take multiple reactions per round if you have resources.**

**Example:**
- You end your turn with 15 SP
- Enemy 1 attacks you: Use Parry (3 SP), 12 SP left
- Enemy 2 attacks you: Use Dodge (4 SP), 8 SP left
- Enemy 3 leaves your reach: Opportunity Attack (4 SP), 4 SP left
- Enemy 4 attacks you: Not enough SP to react, take the hit

## Attack Resolution

### Making an Attack

**Melee Attack:**
```
Attack Roll = d(Might or Agility/2 + Heavy/Light Melee/2) + (Might or Agility/2 + Heavy/Light Melee/2)
```

Use Might + Heavy Melee for heavy weapons.
Use Agility + Light Melee for finesse weapons.

**Ranged Attack:**
```
Attack Roll = d(Agility/2 + Ranged Combat/2) + (Agility/2 + Ranged Combat/2)
```

**Compare to Target's Defense Class (DC).**

**If Attack Roll ≥ Target's DC: Hit!**

### Defense Class (DC)

```
Base DC = 10 + (Agility/2) + Armor Bonus
```

**Armor Bonuses:**

| Armor Type | AC Bonus | Requirements |
|------------|----------|--------------|
| Unarmored | +0 | None |
| Light Armor | +2 to +4 | None |
| Medium Armor | +4 to +6 | Might 8 or Endurance 8 |
| Heavy Armor | +6 to +10 | Might 12, Endurance 10 |
| Shield | +2 | Might 6 or Agility 6 |

**Special:**
- **Unarmored Defense** ability: Use Agility + Endurance/2 or similar formulas
- **Dodge Reaction:** +4 to DC against one attack (costs 4 SP)
- **Parry Reaction:** Roll opposed check to reduce damage (costs 3 SP)

**Example Defense:**
- Agility 12, Light Armor (+3), Shield (+2)
- DC = 10 + 6 + 3 + 2 = **21 DC**

### Damage Calculation

**Weapon Damage:**
```
Damage = Weapon Die + Stat Modifier + Ability Bonuses
```

**Heavy Melee Weapons:**
- Stat Modifier = Might/2
- Greatsword: 2d6 + Might/2
- Battleaxe: 1d10 + Might/2

**Light Melee Weapons:**
- Stat Modifier = Agility/2
- Rapier: 1d8 + Agility/2
- Dagger: 1d4 + Agility/2

**Ranged Weapons:**
- Stat Modifier = Agility/2
- Longbow: 1d8 + Agility/2
- Crossbow: 1d10 + Agility/2

**Ability Bonuses:**
- Power Attack: +Might/2 extra damage
- Sneak Attack: +Xd6 (scales with level)

**Example:**
- Heavy Fighter with Might 14, Heavy Melee 10
- Using Greatsword: 2d6 + 7 damage
- With Power Attack: 2d6 + 7 + 7 = 2d6 + 14 damage

### Critical Hits

**Natural 20 on the die (before modifiers):** Critical Hit!

**Critical Hit Effects:**
- Double all damage dice (not modifiers)
- Example: 2d6 + 14 becomes 4d6 + 14

**Critical Miss:**
- Natural 1: Automatic miss (optional: fumble effects)

## Damage Types & Resistance

**Damage Types:**
- Physical: Slashing, Piercing, Bludgeoning
- Elemental: Fire, Cold, Lightning, Thunder
- Magical: Force, Radiant, Necrotic, Poison, Acid
- Psychic

**Resistance:**
- Take half damage from that type
- Example: Fire Resistance, you take 20 fire damage → take 10 instead

**Vulnerability:**
- Take double damage from that type

**Immunity:**
- Take no damage from that type

## Conditions & Status Effects

**Common Conditions:**

| Condition | Effect |
|-----------|--------|
| Prone | Melee attacks against you have advantage, ranged have disadvantage. Costs 3 SP to stand |
| Stunned | Can't take actions, auto-fail saves |
| Paralyzed | Incapacitated, auto-fail physical saves, attacks against you have advantage and auto-crit if hit |
| Poisoned | Disadvantage on attack rolls and ability checks |
| Blinded | Can't see, auto-fail sight-based checks, disadvantage on attacks |
| Restrained | Speed 0, disadvantage on attacks and DEX saves |
| Frightened | Disadvantage on checks while source of fear is visible, can't move closer to source |

**Advantage/Disadvantage:**
- Advantage: Roll 2 dice, take the higher
- Disadvantage: Roll 2 dice, take the lower

## Rest and Recovery

### Short Rest (10 minutes)
- Recover Endurance × 2 HP
- Recover 25% of Max Mana
- Recover some ability uses
- Bandage wounds, catch breath

### Long Rest (8 hours)
- Recover all HP
- Recover all Stamina
- Recover all Mana
- Reset daily abilities
- Must eat and sleep

## Special Combat Maneuvers

### Grappling
- Costs: 4 SP
- Contested: Your (Might + Athletics) vs their (Might + Athletics) or (Agility + Acrobatics)
- Success: Target is grappled (restrained, speed 0)
- They can use their turn to escape (same contest)

### Shoving
- Costs: 4 SP
- Contested: Your (Might + Athletics) vs their (Might + Athletics) or (Agility + Acrobatics)
- Success: Push 5 feet or knock prone

### Disarm
- Costs: 5 SP
- Contested: Your attack roll vs their (Might + Heavy Melee or Agility + Light Melee)
- Success: They drop weapon

### Called Shot
- Target specific body part
- Attack at disadvantage
- Extra effects if hit (DM discretion)
- Examples: Headshot (extra damage), leg shot (reduce speed), arm shot (disadvantage on attacks)

## Environmental Effects

**Cover:**
- Half Cover: +2 DC
- Three-Quarters Cover: +5 DC
- Total Cover: Can't be targeted

**Difficult Terrain:**
- Costs double stamina to move through
- Examples: Rubble, thick plants, shallow water

**Hazards:**
- Fire: 1d6 damage per turn standing in it
- Lava: 10d10 damage per turn
- Spikes: 2d6 damage when stepped on
- Poison gas: Constitution save or take damage + poisoned

## Flanking (Optional Rule)

If two allies are on opposite sides of an enemy:
- Both have advantage on attacks against that enemy
- Encourages tactical positioning

## Example Combat Round

**Participants:**
- Fighter (Init 15): Might 12, Heavy Melee 10, Max SP 54, Max HP 80
- Rogue (Init 18): Agility 14, Light Melee 12, Max SP 60, Max HP 65
- Wizard (Init 12): Intellect 14, Arcana 16, Max SP 40, Max MP 82, Max HP 55
- 2 Orcs (Init 10, Init 8): Might 10, Heavy Melee 8, Max SP 45, Max HP 60 each

**Round 1:**

**Rogue (Init 18) Turn:**
- Starts with 30 SP (50% of 60)
- Move 25 feet to flank Orc 1: 5 SP (25 SP left)
- Light Melee attack with advantage (flanking): 3 SP (22 SP left)
- Rolls high, hits! 1d8 + 7 + 3d6 (Sneak Attack) = 24 damage
- Light Melee attack: 3 SP (19 SP left)
- Hits! 1d8 + 7 = 12 damage
- End turn with 19 SP for reactions

**Fighter (Init 15) Turn:**
- Starts with 27 SP (50% of 54)
- Move 20 feet to Orc 1: 4 SP (23 SP left)
- Heavy attack (Extra Attack = free): Hits! 2d6 + 6 = 15 damage
- Orc 1 dies! (24 + 12 + 15 = 51 damage)
- Move 10 feet to Orc 2: 2 SP (21 SP left)
- Heavy attack: 4 SP (17 SP left), Hits! 2d6 + 6 = 13 damage
- End turn with 17 SP

**Wizard (Init 12) Turn:**
- Starts with 20 SP, 82 MP
- Move 20 feet: 4 SP (16 SP left)
- Cast Fireball at Orc 2: 8 MP + 3 SP (13 SP, 74 MP left)
- Orc must save (Agility): Fails! Takes 7d6 = 26 damage
- Orc 2 dies! (13 + 26 = 39 damage)
- End turn with 13 SP

**Combat Over!**

**Remaining Resources:**
- Rogue: 19 SP, 65 HP
- Fighter: 17 SP, 80 HP
- Wizard: 13 SP, 74 MP, 55 HP

They can continue or take a short rest to recover.

## Balancing Notes

**Stamina Recovery Rate:**
- 50% per turn ensures you can always do something
- High stamina builds can go nova (use everything)
- Low stamina builds must be careful

**Mana Scarcity:**
- Mana doesn't recover in combat (except special abilities)
- Encourages resource management
- Spellcasters must decide when to go big

**Reactions Costs:**
- Encourages tactical choice: offense or defense?
- Going all-out leaves you vulnerable
- Saving resources for defense limits offense

**Extra Attack Value:**
- Getting a free attack each turn is huge
- Saves 3-4 SP per turn = 1-2 more attacks or reactions

## Related
- [[Stats System]]
- [[Ability Tree]]
- [[Equipment]]
- [[Basic Actions and Conditions]]
