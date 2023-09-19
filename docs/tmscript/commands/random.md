---
tags:
  - TMScript
---

# Random

> Change the seed for the random number generator.

**Random \[seed\]**

_____

**\[seed\]** - The value of the seed.

_____

## Examples

``` title="random-example.txt" linenums="1"
// Set seed
Random [0]

// Get random value
var [value] = [rand:100]

// Notify seed value
Notify [[value]] [local] [0,0,0]
```

Creates a notification message of a random value between 0 to 100. However, since the random seed is set earlier in the script, the value notified will always be the same.
