# Stats System

A dual-layered stat system featuring primary attributes and specialized secondary skills, designed for pseudo-infinite progression.

## Naming Conventions

**Should we keep D&D-style names or create new ones?**

_Option A: Keep familiar names (Strength, Dexterity, etc.) - makes the system approachable_
_Option B: Create unique names to distinguish our system_
_Option C: Hybrid - keep some, change others_

**Current choice: Using D&D-inspired names for accessibility** (edit as needed)

## Two-Tier Stat System

### Primary Stats (Broad Attributes)
The six core attributes that define overall capability:

- **Might** - Physical power, raw strength, carrying capacity
- **Agility** - Reflexes, coordination, overall nimbleness
- **Endurance** - Stamina, health, physical resilience
- **Intellect** - Reasoning, memory, learning capability
- **Awareness** - Perception, intuition, mental acuity
- **Presence** - Force of personality, social influence

### Secondary Stats (Specializations)
Focused skills that fall under each primary stat:

**Might Skills:**
- Athletics (climbing, jumping, swimming)
- Heavy Melee (greatswords, axes, hammers - strength-based combat)
- Physical Intimidation (threatening presence through raw power)

**Agility Skills:**
- Acrobatics (balance, tumbling, aerial maneuvers)
- Sleight of Hand (pickpocketing, lockpicking, fine manipulation)
- Stealth (hiding, moving silently)
- Ranged Combat (bows, thrown weapons)
- Light Melee (rapiers, daggers, finesse weapons - dexterity-based combat)

**Endurance Skills:**
- Fortitude (resisting poison, disease, harsh conditions)
- Stamina (sustained physical activity)

**Intellect Skills:**
- Arcana (magical theory and knowledge)
- History & Lore (recalling information)
- Investigation (deduction, finding clues)
- Crafting (creating items, understanding mechanisms)

**Awareness Skills:**
- Insight (reading people, detecting lies)
- Perception (noticing details, searching)
- Survival (tracking, foraging, navigation)
- Sixth Sense (danger detection, intuition)

**Presence Skills:**
- Persuasion (convincing, negotiating)
- Deception (lying, disguising)
- Performance (entertaining, acting)
- Leadership (inspiring, commanding)
- Looks (physical attractiveness, first impressions, charm through appearance)

### Important Distinctions

**Dual Melee Combat Systems:**
- **Heavy Melee (Might):** Power-based fighting with heavy weapons. Slow, devastating strikes that rely on raw strength. Think barbarians, knights in heavy armor.
- **Light Melee (Agility):** Finesse-based fighting with light weapons. Fast, precise strikes that rely on speed and technique. Think duelists, rogues, swashbucklers.
- You can invest in both if you want versatility, or specialize in one fighting style.

**Looks vs Other Presence Skills:**
- **Looks:** Natural attractiveness and physical charm. Affects first impressions, seduction, modeling, and situations where appearance matters. Passive influence.
- **Persuasion:** Active convincing through logical arguments and rhetoric. Works regardless of appearance.
- **Performance:** Entertaining and captivating an audience through skill and showmanship.
- **Leadership:** Inspiring and commanding through force of will and authority.

High Looks helps in social situations where appearance matters, but won't replace the need for actual social skills in many contexts. A beautiful person (high Looks, low Persuasion) might catch attention but fail to negotiate effectively.

## Starting Stats

### Character Creation
- **Primary Stats:** Start at 0, receive **12 points** to distribute
- **Secondary Stats:** Start at 0, receive **8 points** to distribute among skills
- No limits on distribution - specialize or generalize as desired
- Minimum 0, no maximum

### Starting Recommendations
- Primary: Spread 2-3 points per main stat, or focus 5-6 in one
- Secondary: Pick 3-4 skills to specialize in with 2 points each

## Leveling Progression

### Level System
- **Pseudo-infinite levels** - no hard cap
- XP scales gradually for sustainable progression
- Early levels (1-20): Fast progression, level every 1-2 sessions
- Mid levels (21-50): Moderate pace, every 2-3 sessions
- High levels (51+): Slower but steady, every 3-5 sessions

### Stat Point Allocation

**Primary Stat Points:**
- Gain **+2 Primary Points** every **3 levels**
- Levels 3, 6, 9, 12, 15, 18, etc.
- Can split between multiple primaries or focus one

**Secondary Stat Points:**
- Gain **+2 Secondary Points** every **2 levels**
- Levels 2, 4, 6, 8, 10, 12, etc.
- Can allocate to any secondary skills

**Combined Schedule:**
- Level 1: Start
- Level 2: +2 Secondary
- Level 3: +2 Primary
- Level 4: +2 Secondary
- Level 5: (nothing)
- Level 6: +2 Primary + 2 Secondary
- Level 7: (nothing)
- Level 8: +2 Secondary
- Level 9: +2 Primary
- Level 10: +2 Secondary
- etc.

## Roll Calculation

### Scaling Dice System
Unlike D&D's fixed d20, your dice size and bonus scale with your stats:

**For Primary Stat Checks:**
```
Roll = d(Stat/2) + Stat/2
```
Round down when dividing.

**For Secondary Skill Checks:**
```
Total Stat = Primary + Secondary
Roll = d(Total/2) + Total/2
```

### Why This Works

**Traditional d20 System Problem:**
- Low stat character (d20 + 2): High variance, luck-dependent
- High stat character (d20 + 30): Luck barely matters, very consistent

**Our Scaling System:**
- Variance scales with power level
- Skilled characters have bigger swings but higher floors
- Luck always matters, but your skill determines the range

### Examples:

**Character A - Level 1 Beginner:**
- Agility: 3
- Sleight of Hand: 2
- Total for lockpicking: 3 + 2 = 5

Picking a lock:
- Roll: `d(5/2) + 5/2` = `d2 + 2`
- **Range: 3-4**
- Average: 3.5

**Character B - Level 10 Specialist:**
- Agility: 5
- Sleight of Hand: 8
- Total for lockpicking: 5 + 8 = 13

Picking a lock:
- Roll: `d(13/2) + 13/2` = `d6 + 6`
- **Range: 7-12**
- Average: 9.5

**Character C - Level 10 Generalist:**
- Agility: 9
- Sleight of Hand: 2
- Total for lockpicking: 9 + 2 = 11

Picking a lock:
- Roll: `d(11/2) + 11/2` = `d5 + 5`
- **Range: 6-10**
- Average: 8

**Character D - Level 30 Master:**
- Agility: 12
- Sleight of Hand: 28
- Total for lockpicking: 12 + 28 = 40

Picking a lock:
- Roll: `d(40/2) + 40/2` = `d20 + 20`
- **Range: 21-40**
- Average: 30.5

**Character E - Pure Primary Check:**
- Might: 14 (checking raw strength to break door)

Breaking door:
- Roll: `d(14/2) + 14/2` = `d7 + 7`
- **Range: 8-14**
- Average: 11

### Mathematical Properties

| Total Stat | Die Size | Bonus | Min Roll | Max Roll | Average |
|------------|----------|-------|----------|----------|---------|
| 2 | d1 | +1 | 2 | 2 | 2 |
| 4 | d2 | +2 | 3 | 4 | 3.5 |
| 10 | d5 | +5 | 6 | 10 | 8 |
| 20 | d10 | +10 | 11 | 20 | 15.5 |
| 40 | d20 | +20 | 21 | 40 | 30.5 |
| 60 | d30 | +30 | 31 | 60 | 45.5 |
| 100 | d50 | +50 | 51 | 100 | 75.5 |

**Key Insight:** Variance is always ~50% of your maximum roll. High-level play stays exciting because there's always meaningful randomness.

## Progression Examples

### Level 1 Rogue (Specialist Build)
**Primary Stats:**
- Might: 1, Agility: 5, Endurance: 2, Intellect: 2, Awareness: 1, Presence: 1

**Secondary Stats:**
- Sleight of Hand: 3
- Stealth: 3
- Perception: 2

**Key Check:**
- Picking a lock: Total = 5 + 3 = 8 → **d4 + 4** (range: 5-8, avg 6.5)

### Level 10 Rogue (After Growth)
_Gained 6 Primary points (levels 3, 6, 9) and 10 Secondary points (levels 2, 4, 6, 8, 10)_

**Primary Stats:**
- Might: 1, Agility: 10, Endurance: 2, Intellect: 2, Awareness: 2, Presence: 1

**Secondary Stats:**
- Sleight of Hand: 8
- Stealth: 7
- Perception: 4

**Key Check:**
- Picking a lock: Total = 10 + 8 = 18 → **d9 + 9** (range: 10-18, avg 14)

### Level 10 Heavy Fighter (Generalist Build)
_Same level progression, different allocation_

**Primary Stats:**
- Might: 7, Agility: 4, Endurance: 5, Intellect: 1, Awareness: 1, Presence: 0

**Secondary Stats:**
- Heavy Melee: 5
- Athletics: 4
- Fortitude: 3
- Perception: 1

**Key Checks:**
- Heavy weapon attack: Total = 7 + 5 = 12 → **d6 + 6** (range: 7-12, avg 9.5)
- Raw strength check: Might = 7 → **d3 + 3** (range: 4-6, avg 5)

### Level 10 Duelist (Agility Fighter)
_Dexterity-based melee combatant_

**Primary Stats:**
- Might: 2, Agility: 9, Endurance: 3, Intellect: 1, Awareness: 2, Presence: 1

**Secondary Stats:**
- Light Melee: 6
- Acrobatics: 5
- Stealth: 2
- Perception: 0

**Key Checks:**
- Light weapon attack: Total = 9 + 6 = 15 → **d7 + 7** (range: 8-14, avg 11)
- Dodging (Acrobatics): Total = 9 + 5 = 14 → **d7 + 7** (range: 8-14, avg 11)

### Level 10 Social Character (Looks-focused)
_Charm and persuasion build_

**Primary Stats:**
- Might: 1, Agility: 2, Endurance: 2, Intellect: 3, Awareness: 2, Presence: 8

**Secondary Stats:**
- Looks: 6
- Persuasion: 5
- Deception: 2
- Performance: 0

**Key Checks:**
- First impression (Looks): Total = 8 + 6 = 14 → **d7 + 7** (range: 8-14, avg 11)
- Negotiation (Persuasion): Total = 8 + 5 = 13 → **d6 + 6** (range: 7-12, avg 9.5)

## Key Design Principles

### Specialization vs Generalization
- **Specialists:** High secondary stats, moderate primaries → Excel at specific tasks
- **Generalists:** High primary stats, spread secondaries → Competent at many things
- Both viable, creates meaningful choices

### Pseudo-Infinite Scaling
- No hard caps on stats or levels
- Linear growth prevents exponential power creep
- Variance scales with power, keeping gameplay dynamic at all levels
- **A level 50 character might have:**
  - Primary stats: ~15-25 in main stats
  - Secondary stats: ~25-35 in specializations
  - Check totals: 40-60 → rolling **d20-d30 + 20-30**
  - Range: 21-60 on specialized skills
- **A level 100 character might have:**
  - Primary stats: ~30-40
  - Secondary stats: ~50-70
  - Check totals: 80-110 → rolling **d40-d55 + 40-55**
  - Range: 41-110 on specialized skills

### Why This System Works

**Avoids D&D's (Stat-10)/2 Problem:**
- D&D's formula creates dead zones where stat increases don't matter
- Going from 12→13 does nothing (both give +1)
- Our system: every point counts immediately

**Meaningful Choices Every Level:**
- Not every level gives points, but alternates between primary/secondary
- Creates different planning strategies
- Do you boost your foundation (primary) or your specialty (secondary)?

**Smooth Power Curve:**
- No dramatic power spikes at specific levels
- Progression feels consistent
- Easier to balance encounters

## Difficulty Benchmarks

Setting DCs for checks in this system:

### DC Guidelines by Character Level

Since roll ranges scale with stats, DCs should be set based on average character capabilities:

| Task Difficulty | DC Setting Rule | Example DC (Level 10) | Success Rate |
|----------------|-----------------|---------------------|--------------|
| Trivial | Below average roll | 6 | ~90% |
| Easy | Average roll - 2 | 10 | ~65% |
| Medium | Average roll | 12 | ~50% |
| Hard | Average roll + 2 | 14 | ~35% |
| Very Hard | Near max roll | 16 | ~15% |
| Nearly Impossible | Max roll only | 18 | ~5% |

### Scaling DCs for Level

Unlike D&D's fixed DCs, your challenges should scale:

**Level 1-5 Tasks:**
- Easy: 4-6
- Medium: 7-9
- Hard: 10-12

**Level 10-15 Tasks:**
- Easy: 10-12
- Medium: 14-16
- Hard: 18-20

**Level 30+ Tasks:**
- Easy: 25-30
- Medium: 35-40
- Hard: 45-50

**Level 50+ Tasks:**
- Easy: 40-50
- Medium: 55-65
- Hard: 70-80

### Dynamic DC Setting

**Method 1: Benchmark Against Stat Total**
- Easy task: Total stat × 0.6
- Medium task: Total stat × 0.8
- Hard task: Total stat × 0.95

**Method 2: Use Character Averages**
- Check what the party's average roll would be
- Set DC just above (hard) or just below (easy) that average

### Contest Rolls

When two characters oppose each other (arm wrestling, sneaking past guard, etc.):
- Both roll their relevant stat check
- Higher roll wins
- Ties: Re-roll or advantage to defender/status quo

**Example Contest:**
- Rogue (Agility 10 + Stealth 8 = 18): rolls d9 + 9 → gets 15
- Guard (Awareness 6 + Perception 4 = 10): rolls d5 + 5 → gets 8
- Rogue wins and sneaks past

## Related
- [[Character Creation]]
- [[Game Mechanics]]
- [[Ability Tree]]
- [[Combat]]
- [[Combat System]]
