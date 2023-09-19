---
tags:
  - TMScript
---

# CopyBlock

> Copies a block from one location to another in the world.

**CopyBlock \[x,y,z\] \[x,y,z\]**

_____

**\[x,y,z\]** - The 1st coordinate is the source location (the block to copy).

**\[x,y,z\]** - The 2nd coordinate is the destination location (where to place the copy).

_____

The copied block retains all data and settings associated with the source block.

_____

## Examples

``` title="copyblock-example.txt" linenums="1"
CopyBlock [0, 100, 0] [100, 100, 100]
```

Copies the block at \[0, 100, 0\] to \[100, 100, 100\].
