# Ability Tree

A classless progression system featuring a massive interconnected graph of abilities, spells, and features that characters unlock through stat-based prerequisites.

## Core Concept

**No Classes, Only Choices**

Instead of choosing a class (Fighter, Wizard, Rogue), characters build their identity by:
1. Investing in **Primary and Secondary Stats**
2. Meeting **Prerequisites** for desired abilities
3. Unlocking nodes on the **Ability Tree**
4. Scaling those abilities through continued stat investment

Think Path of Exile's passive tree meets D&D's spell list and class features.

## How It Works

### The Ability Tree Structure

The Ability Tree is a massive interconnected graph containing:
- **Spells** (Fireball, Misty Step, Healing Word, etc.)
- **Combat Techniques** (Extra Attack, Divine Smite, Sneak Attack, etc.)
- **Passive Abilities** (Darkvision, Rage, Evasion, etc.)
- **Utility Features** (Tool Proficiencies, Skill Expertise, Language, etc.)
- **Supernatural Abilities** (Wildshape, Channel Divinity, Ki Powers, etc.)

All abilities exist on a single tree, with connections showing prerequisites and related powers.

### Unlocking Abilities

**Step 1: Meet Prerequisites**
- Each ability has stat requirements
- Once your stats meet the threshold, the ability becomes **available**

**Step 2: Spend an Ability Point**
- Characters gain **1 Ability Point per level**
- Spend a point to permanently unlock an available ability
- Starting characters (Level 1) have **3 ability points** to spend

**Step 3: Use and Scale**
- Unlocked abilities can be used according to their rules
- Abilities automatically scale with your stats

### Prerequisites

Abilities require specific stat thresholds to unlock.

**Example Prerequisites:**

| Ability | Prerequisites |
|---------|---------------|
| Fireball | Intellect 12, Arcana 8 |
| Misty Step | Intellect 10, Arcana 18, Acrobatics 10 |
| Extra Attack (Heavy) | Might 15, Heavy Melee 12 |
| Extra Attack (Light) | Agility 15, Light Melee 12 |
| Divine Smite | Presence 12, Awareness 8 |
| Sneak Attack | Agility 14, Stealth 10 |
| Rage | Might 12, Endurance 10 |
| Evasion | Agility 18, Acrobatics 12 |
| Counterspell | Intellect 14, Arcana 16 |
| Polymorph | Intellect 16, Arcana 20, Awareness 10 |
| Charm Person | Presence 10, Looks 8 |
| Intimidating Presence | Presence 12, Looks 10 OR Physical Intimidation 10 |

**Design Philosophy:**
- Higher-tier abilities require higher stats
- Multi-stat requirements encourage diverse builds
- Some abilities require specific secondary skills
- Prerequisites naturally gate power level

## Ability Scaling

**Unlike D&D where abilities have fixed power, all abilities scale with your stats.**

### Damage Scaling

Abilities that deal damage scale with relevant stats:

**Formula:**
```
Damage = Base Damage + (Scaling Stat × Scaling Factor)
```

**Example: Fireball**
- Prerequisites: Intellect 12, Arcana 8
- Base Damage: 3d6 fire damage
- Scaling: +1d6 per 5 points of Arcana
- Area: 20-foot radius

**Progression:**
- Arcana 8: 3d6 damage (10.5 average)
- Arcana 15: 5d6 damage (17.5 average)
- Arcana 25: 8d6 damage (28 average)
- Arcana 40: 12d6 damage (42 average)

**Example: Divine Smite**
- Prerequisites: Presence 12, Awareness 8
- Base Damage: 2d8 radiant damage
- Scaling: +1d8 per 6 points of Presence
- Usage: Add to a melee hit

**Progression:**
- Presence 12: 2d8 damage (9 average)
- Presence 18: 3d8 damage (13.5 average)
- Presence 30: 5d8 damage (22.5 average)

### Non-Damage Scaling

**Healing:**
```
Healing = Base Healing + (Stat × Scaling Factor)
```

**Example: Cure Wounds**
- Prerequisites: Awareness 10, Insight 6
- Base Healing: 1d8 + Awareness modifier
- Scaling: +1d8 per 8 points of Awareness

**Duration/Range/Targets:**

**Example: Haste**
- Prerequisites: Intellect 14, Arcana 16
- Base Duration: 1 minute
- Base Targets: 1 creature
- Scaling: +1 target per 10 Arcana (16→1, 26→2, 36→3, etc.)

**Save DC (Difficulty Class):**

For abilities that enemies must resist:
```
Ability DC = 10 + (Primary Stat / 2) + (Secondary Stat / 2)
```

**Example: Hold Person**
- Prerequisites: Intellect 12, Arcana 12
- Effect: Target must make Awareness save or be paralyzed
- DC: 10 + (Intellect/2) + (Arcana/2)
- At Intellect 14, Arcana 14: DC = 10 + 7 + 7 = **DC 24**

### Usage Limits

Unlike D&D's spell slots, abilities use various limiting mechanics:

**Cooldown System:**
- **At-Will:** No cooldown (cantrips, basic attacks)
- **Per Encounter:** Usable once per combat, recharges after rest
- **Short Cooldown:** 2-3 round cooldown
- **Long Cooldown:** Once per day

**Resource Systems:**
- Some abilities cost **Mana** (scales with Intellect)
- Some cost **Stamina** (scales with Endurance)
- Some cost **Focus** (scales with Awareness)

**Example Resource Costs:**

| Ability | Cost Type | Base Cost | Cooldown |
|---------|-----------|-----------|----------|
| Fireball | Mana | 15 | None |
| Misty Step | Mana | 10 | None |
| Extra Attack | Passive | N/A | N/A |
| Divine Smite | None | N/A | Per encounter |
| Rage | Stamina | 20 | Per encounter |
| Sneak Attack | None | N/A | Once per turn |

## Ability Types

### 1. Spells (Arcane & Divine)

**Arcane Spells** (Intellect + Arcana):
- Fireball, Lightning Bolt, Magic Missile
- Misty Step, Dimension Door, Teleport
- Counterspell, Dispel Magic
- Polymorph, True Polymorph
- Time Stop, Meteor Swarm

**Divine Spells** (Awareness + Insight):
- Cure Wounds, Heal, Mass Heal
- Bless, Shield of Faith, Sanctuary
- Turn Undead, Banishment
- Resurrection, True Resurrection

**Nature Magic** (Awareness + Survival):
- Entangle, Spike Growth, Wall of Thorns
- Goodberry, Pass Without Trace
- Wildshape, Beast Sense

### 2. Combat Techniques

**Martial Abilities:**
- **Extra Attack** - Attack multiple times per turn
- **Great Weapon Master** - Trade accuracy for damage
- **Parry** - Reaction to reduce incoming damage
- **Whirlwind Attack** - Strike all adjacent enemies

**Precision Abilities:**
- **Sneak Attack** - Bonus damage with advantage
- **Assassinate** - Critical hits on surprised enemies
- **Aimed Shot** - Bonus to ranged attack rolls

**Defensive Abilities:**
- **Evasion** - Dodge area effects
- **Uncanny Dodge** - Halve damage from attacks
- **Shield Master** - Bonus AC and saving throws

### 3. Passive Abilities

**Always Active:**
- **Darkvision** - See in darkness
- **Unarmored Defense** - AC based on stats without armor
- **Spell Resistance** - Advantage on saves vs magic
- **Fast Movement** - Increased movement speed

### 4. Resource & Utility Abilities

- **Arcane Recovery** - Regain mana on short rest
- **Second Wind** - Heal yourself mid-combat
- **Tool Expertise** - Double proficiency with specific tools
- **Ritual Casting** - Cast spells without resource cost (takes longer)

## Example Ability Chains

### Fire Magic Path

```
Prerequisites → Ability

Intellect 8, Arcana 5 → Fire Bolt (At-will fire damage)
  ↓
Intellect 10, Arcana 8 → Burning Hands (Cone of fire)
  ↓
Intellect 12, Arcana 12 → Scorching Ray (Multiple fire beams)
  ↓
Intellect 12, Arcana 15 → Fireball (Area damage)
  ↓
Intellect 14, Arcana 20 → Wall of Fire (Persistent barrier)
  ↓
Intellect 16, Arcana 25 → Delayed Blast Fireball (Massive explosion)
  ↓
Intellect 18, Arcana 30 → Meteor Swarm (Ultimate fire spell)
```

### Heavy Melee Combat Path (Strength)

```
Might 10, Heavy Melee 8 → Power Attack (Trade accuracy for damage)
  ↓
Might 12, Heavy Melee 10 → Cleave (Hit multiple foes)
  ↓
Might 15, Heavy Melee 12 → Extra Attack (Attack twice)
  ↓
Might 18, Heavy Melee 18 → Whirlwind Attack (Hit all adjacent)
  ↓
Might 20, Heavy Melee 22 → Triple Attack (Attack three times)
  ↓
Might 22, Heavy Melee 26 → Devastating Blow (Massive single strike)
```

### Light Melee Combat Path (Finesse)

```
Agility 10, Light Melee 8 → Riposte (Counter-attack after dodge)
  ↓
Agility 12, Light Melee 10 → Flurry (Rapid strikes)
  ↓
Agility 15, Light Melee 12 → Extra Attack (Attack twice with finesse)
  ↓
Agility 18, Light Melee 16 → Precise Strike (Critical hit boost)
  ↓
Agility 20, Light Melee 20 → Triple Attack (Three swift strikes)
  ↓
Agility 22, Light Melee 24 → Dance of Blades (Multi-target precision)
```

### Stealth & Mobility Path

```
Agility 10, Stealth 6 → Hide in Shadows
  ↓
Agility 12, Stealth 10 → Sneak Attack
  ↓
Agility 14, Acrobatics 10, Arcana 10 → Misty Step
  ↓
Agility 16, Stealth 14 → Invisibility
  ↓
Agility 18, Acrobatics 12 → Evasion
  ↓
Agility 18, Stealth 18, Arcana 15 → Greater Invisibility
```

### Hybrid Paladin-Style Path

```
Might 10, Heavy Melee 6, Presence 8 → Lay on Hands (Healing touch)
  ↓
Might 12, Heavy Melee 8, Presence 12, Awareness 8 → Divine Smite
  ↓
Might 14, Presence 14, Awareness 10 → Aura of Protection
  ↓
Might 16, Presence 16, Awareness 12 → Divine Shield (Invulnerability)
```

### Social Manipulation Path (Charm & Looks)

```
Presence 8, Looks 6 → Charm Person (Make someone friendly)
  ↓
Presence 10, Looks 10 → Dazzling Presence (Distract with appearance)
  ↓
Presence 12, Looks 14, Persuasion 8 → Mass Charm (Charm multiple people)
  ↓
Presence 14, Looks 18 → Enthrall (Captivate audience completely)
  ↓
Presence 16, Looks 22 → Overwhelming Presence (Dominate social situations)
```

## Sample Starting Builds

### Level 1 Fire Mage
**Stats:**
- Intellect: 5, Arcana: 7

**Starting Abilities (3 points):**
1. Fire Bolt (At-will damage)
2. Mage Armor (Protective spell)
3. Shield (Reaction defense)

**Build Path:** Invest in Arcana to unlock Fireball at level 5-7

### Level 1 Sword & Board Fighter
**Stats:**
- Might: 7, Heavy Melee: 8, Fortitude: 5

**Starting Abilities (3 points):**
1. Power Attack (Damage boost)
2. Shield Bash (Bonus action attack)
3. Second Wind (Self-healing)

**Build Path:** Get Might to 15 for Extra Attack (Heavy)

### Level 1 Stealthy Scout
**Stats:**
- Agility: 8, Stealth: 8, Perception: 4

**Starting Abilities (3 points):**
1. Hide in Shadows
2. Sneak Attack
3. Quick Reflexes (Initiative bonus)

**Build Path:** Balance Agility/Acrobatics/Arcana for Misty Step

### Level 1 Hybrid Spellblade
**Stats:**
- Agility: 5, Intellect: 5, Light Melee: 5, Arcana: 6

**Starting Abilities (3 points):**
1. Weapon Bond (Magic weapon attacks)
2. Shield (Defensive spell)
3. Booming Blade (Melee + spell combo)

**Build Path:** Balance Light Melee and Arcana for agile magical combat

### Level 1 Duelist
**Stats:**
- Agility: 7, Light Melee: 8, Acrobatics: 5

**Starting Abilities (3 points):**
1. Riposte (Counter-attack)
2. Parry (Defensive reaction)
3. Fancy Footwork (Enhanced mobility)

**Build Path:** Get Agility to 15 for Extra Attack (Light)

### Level 1 Charming Face
**Stats:**
- Presence: 6, Looks: 8, Persuasion: 6

**Starting Abilities (3 points):**
1. Charm Person (Make someone friendly)
2. Silver Tongue (Bonus to persuasion)
3. Distraction (Use looks to divert attention)

**Build Path:** Invest in Looks and Persuasion for social dominance

## Design Advantages

### Player Agency
- Build exactly the character you want
- No "wrong" multiclass combinations
- Experiment without permanent commitment (could allow respec)

### Smooth Progression
- Gain 1 ability point per level
- Always something to look forward to
- No dead levels

### Natural Balance
- Stat prerequisites gate powerful abilities
- Can't rush to overpowered abilities without investment
- Specialist vs generalist trade-offs

### Infinite Expandability
- Add new abilities anytime
- Community-created abilities possible
- Modular system allows easy balancing

## Ability Tree Organization

The tree is organized into **regions** for easier navigation:

**Center:**
- Basic, universal abilities
- Low prerequisites
- Starting point for all characters

**Outer Regions:**
- **North:** Arcane Magic (Intellect/Arcana)
- **Northeast:** Divine Magic (Awareness/Insight)
- **East:** Nature Magic (Awareness/Survival)
- **Southeast:** Social Abilities (Presence skills)
- **South:** Stealth & Mobility (Agility/Stealth/Acrobatics)
- **Southwest:** Ranged Combat (Agility/Ranged Combat)
- **West:** Melee Combat (Might/Melee Combat)
- **Northwest:** Defensive/Tank (Endurance/Fortitude)

**Hybrid Zones:**
- Between regions for hybrid builds
- Paladin-style abilities (Might + Presence)
- Spellblade abilities (Might + Intellect)
- Arcane Archer (Agility + Intellect)

## Balancing Considerations

### Power Budget

Each ability has a **power level** based on:
1. Prerequisites (higher = more powerful)
2. Scaling potential
3. Usage frequency
4. Impact on gameplay

**Example Power Levels:**
- Tier 1 (Requirements ~10 total): Basic abilities
- Tier 2 (Requirements ~20 total): Moderate abilities
- Tier 3 (Requirements ~30 total): Strong abilities
- Tier 4 (Requirements ~40+ total): Elite abilities
- Tier 5 (Requirements ~60+ total): Legendary abilities

### Preventing Must-Picks

- Avoid abilities that are universally better
- Create situational power (AoE vs single-target)
- Allow multiple paths to similar goals
- Balance versatility vs specialization

### Retraining/Respeccing

**Option A: Free Respec**
- Can reassign ability points on level up
- Encourages experimentation
- Risk: Analysis paralysis

**Option B: Limited Respec**
- Can respec 1 ability point per level
- Gradual build adjustment
- Balance: Flexibility without complete do-overs

**Option C: No Respec**
- Choices are permanent
- Encourages planning
- Risk: Build regret

**Current Recommendation: Option B** (edit as desired)

## Related
- [[Stats System]]
- [[Character Creation]]
- [[Spells]]
- [[Combat]]
- [[Combat System]]
