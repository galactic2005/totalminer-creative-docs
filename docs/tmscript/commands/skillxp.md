---
tags:
  - TMScript
---

# SkillXP

> Set, add, or subtrack a player's current skill XP.

**SkillXP \[name\] \[+|-|xp\]**

_____

**\[name\]** - The name of the skill.

**\[+|-|xp\]** - The xp to set the skill to, or to add or subtract xp from the skill.

_____

## Examples

``` title="skillxp-example-1.txt" linenums="1"
// Set some skills to have different amounts of xp
SkillXP [Mining] [500]
SkillXP [Digging] [750]
SkillXP [Chopping] [100]
```

Sets three different skills to different amounts of xp for the player who activated this script.

``` title="skillsp-example-2.txt" linenums="1"
// Add 3000 xp to building
Skill [Building] [+3000]

// Subtract 2000 xp from crafting
Skill [Crafting] [-2000]
```

Adds 3000 xp to the Building skill and subtracts 2000 xp from the Crafting skill for the player who activated this script.

## See Also

* [HasSkill command](/tmscript/commands/query-commands/hasskill/)
* [IsSkills command](/tmscript/commands/query-commands/isskills/)
* [Skill command](/tmscript/commands/skill/)
* [Skills System](/documentation/skills-system/)
