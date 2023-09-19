---
tags:
  - TMScript
---

# Kick

> Kicks the player who activated the script from the multiplayer session.

**kick**

_____

Kicked players will not be able to rejoin the world until the multiplayer session has ended.

This command does nothing in single-player and to players who are a developer of Total Miner.

_____

## Examples

``` title="kick-example-1.txt" linenums="1"
Kick
```

Kicks the player who activated this script out of the multiplayer session.

``` title="kick-example-2.txt" linenums="1"
If
    HasHistory [Banned] [player] [true]
Then
    // Kick player if banned
    Kick
Endif
```

Setting this as one of the first scripts to execute when a player joins will automatically kick them from the world should they have the historical record _Banned_.
