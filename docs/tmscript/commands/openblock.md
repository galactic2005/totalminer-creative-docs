---
tags:
  - TMScript
---

# OpenBlock

> Opens the standard interface screen for container blocks.

**OpenBlock \[x,y,z\]**

_____

**\[x,y,z\]** - The coordinate in the world of the block to open.

_____

Only the following blocks may be opened using this command:

* Block Shop
* Book
* Bookcase
* Chest
* Crate
* Furnace
* Item Shop
* Locked Chest
* Safe
* Workbench

_____

## Examples

``` title="openblock-example.txt" linenums="1"
OpenBlock [100, 100, 100]
```

Opens the block located at 100, 100, 100 for the player who activated this script.
