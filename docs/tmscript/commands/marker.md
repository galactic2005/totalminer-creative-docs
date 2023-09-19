---
tags:
  - TMScript
---

# Marker

> Manipulates map markers.

**Marker \[name\] \[x,z\]**

**Marker \[name\] \[x,z\] \[admin\]**

**Marker \[name\] \[delete\]**

_____

**\[name\]** - The name of the map marker.

**\[xz\]** - The surface position of the map marker to create at.

**\[admin\]** - If omitted, the map marker is visible to everyone. If used, the map marker will only be visible to those with admin permissions.

**\[delete\]** - Deletes a map marker based on name.

_____

## Examples

``` title="marker-example-1.txt" linenums="1"
// Create a marker
Marker [center] [0, 0]

// Create a admin marker
Marker [admin-base] [100, 100] [admin]

```

Creates a map marker at the center of the world titled "center" and another map marker only visible to admins titled "admin-base" at \[100, 100\].

``` title="marker-example-2.txt" linenums="1"
// Delete a marker
Marker [secret] [delete]

```

Deletes the map marker titled "secret" in the world. If no such map marker exists, this command does nothing.

## See Also

* [HasMarker command](/tmscript/commands/query-commands/hasmarker/)
* [Waypoint command](/tmscript/commands/waypoint/)
