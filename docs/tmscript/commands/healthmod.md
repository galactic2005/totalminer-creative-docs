---
tags:
  - TMScript
---

# HealthMod

> Manipulates an actor's health regeneration multiplier.

**HealthMod \[multiplier\]**
_____

**\[multiplier\]** - How fast health regenerates. A value of 0 removes health regeneration, and a negative value damages the player over time. The default value is 1.

_____

Health regenerates at the rate of the health multiplier per second. So for example, a multiplier of 1 will regenerate 1 health per second, and a multiplier of 5 will regenerate 5 health per second. This works the other way around too with negative multipliers.

_____

## Examples

``` title="healthmod-example.txt" linenums="1"
// Default regneration
HealthMod [1]
```

Sets the actor's health regeneration multiplier to 1, which is the default regeneration.
