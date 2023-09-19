---
tags:
  - TMScript
---

# ReplaceRegion

> Replaces all occurrences of a block in a cubic region with another block.

**ReplaceRegion \[x,y,z\] \[x,y,z\] \[block1\] \[block2\]**

_____

**\[x,y,z\]** - The 1st coordinate is the minimum bound of the replace region.

**\[x,y,z\]** - The 2nd coordinate is the maximum bound of the replace region.

**\[block1\]** - The block type to be replaced.

**\[block2\]** - The block type to replace with.
_____

## Examples

``` title="replaceregion-example.txt" linenums="1"
// Replace Limestone with Marble
ReplaceRegion [0, 0, 0] [100, 100, 100] [Limestone] [Marble]
```

Replaces all Limestone blocks within the \[0, 0, 0\] to \[100, 100, 100\] cubic region with Marble blocks.

## See Also

* [HasSkill command](/tmscript/commands/query-commands/hasskill/)
* [IsSkills command](/tmscript/commands/query-commands/isskills/)
* [SkillXP command](/tmscript/commands/skillxp/)
* [Skills System](/documentation/skills-system/)
