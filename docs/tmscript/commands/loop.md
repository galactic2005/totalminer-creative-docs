---
tags:
  - TMScript
---

# Loop

> Restarts the script from the top.

**Loop**

**Loop \[millisecs\]**

_____

**\[millisecs\]** - The time in milliseconds to wait before the script restarts from the top. This value cannot be less than 2. If omitted the default value of 16 is used.

Because of how scripts are queued for execution, these timings are not exact and shouldn't be relied upon.

_____

1000 milliseconds is equal to 1 second.

Variables keep their value when the command is ran. See the second example for more information.

_____

## Examples

``` title="loop-example-1.txt" linenums="1"
Notify [I'm stuck in a loop!] [global] [0, 0, 0]
Loop [500]
```

Creates a notification message approximately every 500 milliseconds (or 0.5 seconds) forever until the script is cancelled.

``` title="loop-example-2.txt" linenums="1"
// Define the variable counter
var [counter]

// Set the block ColorRed at [0, 100, counter]
SetBlock [0, 100, counter] [ColorRed]

// Increment counter
var [counter] = [counter] + [1]
If
    IsVar [counter] [<] [101]
Then
    // Loop if counter is below 101
    Loop
Endif
```

When the loop command is ran, variables keep their value when the script restarts. This is used to create a line of 100 red blocks from \[0, 100, 0\] to \[0, 100, 100\].

## See Also

* [Wait command](wait.md)
