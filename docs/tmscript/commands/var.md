---
tags:
  - TMScript
---

# var

> Declare variables and assign values.

**var \[name\] \[name\]...\[name\]**

**var \[name\] = \[value\] op \[value\]...op \[value\]**

_____

**\[name\]** - The name of the variable.
>Variable names cannot have spaces or contain special characters.

**\[op\]** - Operators. The following operators can be used:

* (+) Addition
* (-) Subtraction
* (*) Multiplication
* (/) Division
* (%) Modulus

Operators do not need to be surrounded by square brackets.

Example:

``` title="operators.txt" linenums="1"
// With square brackets
var [value] = [4] [+] [2]

// Without square brackets
var [value] = [4] + [2]

// Both will work and the variable will be set to 6
```

**\[value\]** - A defined mathematical object. Values may be either a numeric literal, another variable or a built in value type as listed below.

> All built-in value type names must be succeeded by a color before the closing square bracket, even if they don't have parameters.

* \[Abs:x\] - The absolute value of x.
* \[Sin:x\] - The sine of x.
* \[Cos:x\] - The cosine of x.
* \[Tan:x\] - The tangent of x.
* \[Sqrt:x\] - The square root of x.
* \[Single:x\] - x converted to single precision.
* \[Int:x\] - x converted to an integer.
* \[Neg:x\] or \[-x\] - Negate x.
* \[pi:\] - The value of (π) Pi.
* \[Clamp:x,y,z\] - Clamp x to y and z.
* \[Lerp:x,y,t\] - Linear interpolation from x to y based on t.
* \[Rand:x\] - A random number between 0 to x inclusive.
* \[Hash:text\] - Returns an integral hash of text.
* \[Clock:\] - The world's current clock time between 0 to 24.
* \[Health:\] - The player's current health.
* \[MaxHealth:\] - The player's current maximum health (i.e. 100% current health).
* \[Reach:\] - The player's current reach.
* \[Pos:x|y|z\] - The player's current X, Y, or Z position.
* \[Eye:x|y|z\] - The player's current X, Y, or Z eye position.
* \[Vel:x|y|z\] - The player's current X, Y, or Z velocity.
* \[View:x|y|z\] - The player's current X, Y, or Z view direction.
* \[Rel:x|y|z\] - The script's relative X, Y, or Z block position.
* \[Prel:x|y|z\] - The player's X, Y, or Z block position.
* \[Crel:x|y|z\] - The player's X, Y, or Z cursor position.
* \[Script:x|y|z\] - The script's X, Y, or Z offset.
* \[Skill:x\] - The player's current skill level.
* \[Skillxp:x\] - The player's current skill xp.
* \[History:key\] - The value of the player's historical record \[key\].
* \[Syshistory:key\] - The value of the world's historical record \[key\].
* \[ClanHistory:key\] - The value of the clan's historical record \[key\].
* \[Viewport:width|height\] or \[vp:w|h\] - The viewport's width or height.
* \[Block:x,y,z\] - The id of the block at position XYZ.
* \[Aux:x,y,z\] - The aux data of the block at position XYZ.
* \[Light:x,y,z\] - The light level of the block at position XYZ.
* \[SunLight:x,y,z\] - The light level of the block at position XYZ (only light from the sun is considered in this value type).
* \[BlockLight:x,y,z\] - The block light level of the block at position XYZ (only light from light blocks, such as torches or sun boxes, are considered in this value type.)
* \[Item:left|right|event\] - The item id that is in either hand, or that caused the \[swing\], \[equip\], or \[unequip\] event to execute.
* \[Inv:\[item\]\[x,y,z\]\] - The amount of an item in the player's inventory. The \[XYZ\] parameter is optional, and if used, this will instead return the amount of an item in the block's inventory at XYZ position.
* \[Distance:\[x,y,z\]\[x,y,z\]\] - The distance between two points in the world.
* \[Gamercount:all|local|remote\] - The number of players in the world, specified by type.
* \[Gamercount:\[zone\]\[all|local|remote\]\] - The number of players in a zone, specified by type.
* \[Gamercount:\[x,y,z\]\[x,y,z\]\[all|local|remote\]\] - The number of players in a cubic area, specified by type.
* \[Gamercount:\[x,y,z\]\[radius\]\[all|local|remote\]\] - The number of players in a spherical area, specified by type.
* \[NpcCount:npctype\] - The number of type of NPC in the world.
* \[NpcCount:\[zone\]\[npctype\]\] - The number of a type of NPC in a zone.
* \[NpcCount:\[x,y,z\]\[x,y,z\]\[npctype\]\] - The number of a type of NPCs in a cubic area.
* \[NpcCount:\[x,y,z\]\[radius\]\[npctype\]\] - The number of type of NPCs in a spherical area.

_____

There are two forms of the var command. One declares one or more variable names:

**var \[name\] \[name\]...\[name\]**

The other assigns a value to a single variable, based on an expression:

**var \[name\] = \[value\] op \[value\]...op \[value\]**

A script can only have up to 256 variables.
_____

## Examples

``` title="delcaring-variables.txt" linenums="1"
// Declare variables
var [velx] [vely] [velz] [length] [distance] [dir]
```

Declares 6 variable names. If these variables have not been passed from a calling script, they are assigned a value of 0. All variables used in a script must be declared before they are used. They may be declared anyhwere in a script, as long as it is before they are used.

## See Also

* [Input command](input.md)

_____

## Depreciates

> The following commands and/or parameters are depreciated and are only available to support maps and scripts which have used these in the past. It is recommended to not use these depreciated commands and/or parameters over the newer alternatives.

**\[value\]** has depreciated built-in value types as listed below:

* \[MobCount:mobtype\] - Works the same as the \[NpcCount:npctype\] value type. Zone, cubic, and spherical variations also exist.
