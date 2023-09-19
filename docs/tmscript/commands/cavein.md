---
tags:
  - TMScript
---

# CaveIn

> Starts a cave-in (also known as earthquakes) at a position in the world.

**CaveIn \[x,y,z\] \[seed\]**

_____

**\[x,y,z\]** - The coordinate in the world of where the cave-in occurs.

**\[seed\]** - Optional parameter that determines what random seed the cave-in uses. If omitted, a value of 0 is used.

_____

Only 1 cave-in can simultaneously occur in the world at a time. If any cave-in is currently running when the CaveIn command is executed, than it will be ignored.

_____

## Examples

``` title="cavein-example.txt" linenums="1"
// Start a cave-in
CaveIn [0, 0, 0] [10]
```

Starts a cave-in at \[0,0,0\] with a random seed of 10. If a cave-in is currently active already, this command is ignored.
