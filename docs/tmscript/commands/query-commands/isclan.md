---
tags:
  - TMScript
---

# IsClan

> Queries if the player is a member of a clan.

**IsClan \[name\] \[true|false\]**

_____

**\[name\]** - The name of the clan to query if the player is in or not.

**\[true|false\]** - If true, the command will return true if the player is in the specified clan.

_____

## Examples

``` title="isclan-example.txt" linenums="1"
If
    // Is the player on the clan named Team1
    IsClan [Team1] [true]
Then
    // Add player to Team2
    Clan [Team2]
Else
    // Add player to Team1
    Clan [Team1]
Endif
```

If the player who activated this script is on Team1, it puts them on Team2. Otherwise, it puts them on Team1.

## See Also

* [Clan command](/tmscript/commands/clan)
* [Clan Banners](/documentation/clan-banners/)
