---
tags:
  - TMScript
---

# Waypoint

> Manipulates the player waypoint.

**Waypoint \[x,z\]**

**Waypoint \[delete\]**

_____

**\[xz\]** - The surface position of the waypoint to set to.

**\[delete\]** - Deletes the player's waypoint.

_____

A player can only have one waypoint at a time. If the player already has a waypoint then setting a new one will override the previous one.

_____

## Examples

``` title="waypoint-example-1.txt" linenums="1"
// Set the player's waypoint
Waypoint [-100, -100]
```

Sets the player's waypoint to \[-100, -100\]. If they previously had a waypoint it will be overrided with this new one.

``` title="waypoint-example-2.txt" linenums="1"
// Delete the player's waypoint
Waypoint [delete]

```

Delete the player's waypoint. If the player doesn't have a waypoint, this command does nothing.

## See Also

* [Marker command](/tmscript/commands/marker/)
