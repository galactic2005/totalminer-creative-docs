---
tags:
  - TMScript
---

# Clan

> Assigns the player to a clan or removes them from a clan.

**Clan \[name\]**

**Clan \[name\] \[bannerID\]**

**Clan \[remove\]**

_____

**\[name\]** - The name of the clan to assign the player to.

**\[bannerID\]** - The clan banner ID. If omitted, the clan banner will be blank.

**\[remove\]** - Removes the player from the clan they are assigned to.

_____

## Examples

``` title="clan-example-1.txt" linenums="1"
// Assign the player to the clan Team1 with clan banner ID 33
Clan [Team1] [33]
```

Assigns the player who activated this script to a clan named Team1, using the clan banner ID 33 ![Banner 33](/images/clanbanners/33.png).

``` title="clan-example-2.txt" linenums="1"
// Removes the player from the clan they are in.
Clan [remove]
```

Removes the player who activated this script from the clan they are in. If the player isn't in a clan, this command does nothing.

## See Also

* [IsClan command](/tmscript/commands/query-commands/isclan/)
* [Clan Banners](/documentation/clan-banners/)
