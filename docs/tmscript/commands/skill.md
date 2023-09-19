---
tags:
  - TMScript
---

# Skill

> Set, add, or subtrack a player's current skill level.

**Skill \[name\] \[+|-|level\]**

_____

**\[name\]** - The name of the skill.

**\[+|-|level\]** - The level to set the skill to, or to add or subtract levels from the skill.

_____

## Examples

``` title="skill-example-1.txt" linenums="1"
// Set skill levels
Skill [Attack] [10]
Skill [Defence] [25]
Skill [Health] [50]
```

Sets three different skills to different skill levels for the player who activated this script.

``` title="skill-example-2.txt" linenums="1"
// Add 2 skill levels to building
Skill [Building] [+2]

// Subtract 3 skill levels to cooking
Skill [Cooking] [-3]
```

Adds 2 skill levels to the Building skill and subtracts 3 levels to the Cooking skill for the player who activated this script.

## See Also

* [HasSkill command](/tmscript/commands/query-commands/hasskill/)
* [IsSkills command](/tmscript/commands/query-commands/isskills/)
* [SkillXP command](/tmscript/commands/skillxp/)
* [Skills System](/documentation/skills-system/)
