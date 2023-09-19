---
tags:
  - TMScript
---

# Wait

> Pauses the script execution for a period of time.

**Wait \[millisecs\]**

_____

**\[millisecs\]** - The time in milliseconds to wait before script execution continues.
_____

1000 milliseconds is equal to 1 second.

_____

## Examples

``` title="wait-example.txt" linenums="1"
Wait [1000]
Notify ["A second has passed."] [global] [0,0,0]
```

Script execution waits for 1000 milliseconds (or 1 second) before a notification message is created displaying a second has passed.

## See Also

* [Loop command](loop.md)
