---
tags:
  - TMScript
---

# History

> Manipulates historical records. Historical records can be queried by the HasHistory command to determine if a record exists.

**History \[name\] \[+|-|count|delete\]**

**History \[name\] \[player|clan\] \[+|-|count|delete\]**
_____

**\[name\]** - The name of the historical record. History names support folders which allows you to match your history names with script names, where appropiate. Variable substitution is supported for History names.

**\[+|-|count|delete\]** - Specify either an absolute value to set the history to, or specify a relative value to add to or subtract from. If delete is specified, then this command will instead delete the historical record.

**\[player|clan]** - Optional parameter that saves the historical record on the player or the player's clan instead of the world (system).

_____

Historical records are counters. So if the History command adds a record for the same name more than once, than the counter for the initial record is increased. For example:

``` title="history-counter.txt" linenums="1"
History [counter]
```

When executing this command the first time, it'll create the historial record "counter" with the value of 1. However, subsequent executions of this command will increment this record instead of creating new records.

This allows scripts to query how many times a record has occured.

_____

## Examples

``` title="history-example-1.txt" linenums="1"
// Create historical record
History [ActionX]
```

Creates a new system historical record called ActionX with the value of 1. If the record already exists, it's incremented by 1 instead.

``` title="history-example-2.txt" linenums="1"
// Deincrement record
History [ActionX] [-1]
```

Subtracts 1 from a system historical record called ActionX.

``` title="history-example-3.txt" linenums="1"
// Create historical record for player
History [PlayerHistory] [player]
```

Creates a new historical record called PlayerHistory, which will be stored with the player. If this script isn't ran by a player, this command does nothing.

``` title="history-example-4.txt" linenums="1"
// Create historical record for clan
History [ClanHistory] [clan]
```

Creates a new historical record called ClanHistory, which will be stored with the player's clan. If the player isn't in a clan, or if the script wasn't ran by a player, this command does nothing.
