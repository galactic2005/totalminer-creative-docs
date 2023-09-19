---
tags:
  - TMScript
---

# HasSkill

> Queries player skill levels.

**HasSkill \[skill\] \[compare\] \[level\]**

_____

**\[skill\]** - The skill name to query.

**\[compare\]** - Comparision based on the skill level of the player.

**\[level\]** - The skill level target for comparison.

_____

## Examples

``` title="hasskill-example.txt" linenums="1"
If
    // Does the player have 20 or more skill levels in Defence
    HasSkill [Defence] [>=] [20]
Then
    // Give the player a Steel Spear
    Inventory [actor] [actor] [add] [Steel Spear] [1]
Endif
```

If the player who activated this script has 20 or more skill levels in Defence, then they will recieve a spear, otherwise this script does nothing.

## See Also

* [IsSkills command](/tmscript/commands/query-commands/isskills/)
* [Skill command](/tmscript/commands/skill/)
* [SkillXP command](/tmscript/commands/skillxp/)
* [Skills System](/documentation/skills-system/)
