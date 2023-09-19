---
tags:
  - TMScript
---

# IsFiniteResources

> Queries if Finite Resources is enabled.

**IsFiniteResources \[true|false\]**

_____

**\[true|false\]** - If true, the command will return true if Finite Resources is enabled.

_____

## Examples

``` title="isfiniteresources-example.txt" linenums="1"
If
    // Is Finite Resources enabled
    IsFiniteResources [true]
Then
    Notify [Finite Resources is enabled.] [global] [0,0,0]
Else
    Notify [Finite Resources is disabled.] [global] [0,0,0]
Endif
```

If Finite Resources is enabled, a notification message is created displaying that Finite Resources is enabled. Otherwise, a notification message is created displaying that Finite Resources is disabled.
