---
tags:
  - TMScript
---

# IsSkills

> Queries if the skill system is enabled.

**IsSkills \[true|false\]**

_____

**\[true|false\]** - If true, the command will return true if the skill system is enabled.

_____

## Examples

``` title="isskills-example.txt" linenums="1"
If
    // Is the skill system enabled
    IsSkills [true]
Then
    Skill [Health] [7]
Endif
```

If the skill system is enabled, than the Health skill level of the player who activated this script will be set to 7, otherwise this script does nothing.

## See Also

* [HasSkill command](/tmscript/commands/query-commands/hasskill/)
* [Skill command](/tmscript/commands/skill/)
* [SkillXP command](/tmscript/commands/skillxp/)
* [Skills System](/documentation/skills-system/)
