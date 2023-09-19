---
tags:
  - TMScript
---

# Input

> Prompts the player to enter a number.

**Input \[var\]**

_____

**\[var\]** - The name of the variable to store the number entered.

_____

The player will be prompted to input any number from -9999999999 to 9999999999 when this command is ran.

_____

## Examples

``` title="input-example.txt" linenums="1"
// Declare the variable password
var [password]

// Get the player's input and put the prompt into the password variable
Input [password]
```

Prompts the player who activated this script to enter a number. Once entered, the variable _password_ contains the input.

## See Also

* [Var command](var.md)
