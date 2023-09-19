---
tags:
  - TMScript
---

# IsDayTime

> Queries if it is currently day time.

**IsDayTime \[true|false\]**

_____

**\[true|false\]** - If true, the command will return true if it is currently day time.

It is considered day time between 6.75 to 17.25 in clock time.

_____

## Examples

``` title="isdaytime-example.txt" linenums="1"
If
    // Is it night time
    IsDayTime [false]
Then
    // Give a bed
    Inventory [actor] [add] [Bed] [1]
Endif
```

If it is currently night time then give the player who activated this script a bed, otherwise this script does nothing.

## See Also

* [IsClock command](/tmscript/commands/query-commands/isclock/)
* [Clock Time](/documentation/clock-time/)
