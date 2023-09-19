---
tags:
  - TMScript
---

# IsClock

> Queries the current game hour.

**IsClock \[hour\] \[true|false\]**

**IsClock \[compare\] \[hour|history\]**

_____

**\[hour\]** - The hour to query.

**\[hour|history\]** - The hour or history to query.

**\[true|false\]** - If true, the command will return true if the clock time is the hour queried.

**\[compare\]** - Comparision based on the current hour. Will return true if the comparision is met.

_____

## Examples

``` title="isclock-example-1.txt" linenums="1"
If
    // Is it noon hour
    IsClock [12] [true]
Then
    // It's high noon
    Notify [It's high noon.] [global] [0,0,0]
Endif
```

If it is noon hour (12 PM) a notification message is created displaying that "it's high noon", otherwise this script does nothing.

``` title="isclock-example-2.txt" linenums="1"
If
    // Is it the afternoon
    IsClock [>] [12]
Then
    // It's sadly no longer high noon
    Notify [It's not high noon.] [global] [0,0,0]
Endif
```

If it is the afternoon a notification message is created displaying that "it's not high noon", otherwise this script does nothing.

## See Also

* [IsDayTime command](/tmscript/commands/query-commands/isdaytime/)
* [Clock Time](/documentation/clock-time/)
