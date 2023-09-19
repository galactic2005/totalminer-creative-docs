# History vs Var

It can be confusing for newcomers to determine when to use each command, as functionally, they are similar. However, there are some key differences between the two that should help players determine where each one is more effective.

## Differences between Historical Records and Variables

### Calculation Depth

The var command contains a number of built-in values and supports 5 different operators. This allows for a number of different expressions to calculate the value of a variable.

Historical records are confined to what the History command offers, which isn't much. You can work with setting historical records to specific values, addition, and subtraction.

Another note worth considering is that variables support fractional numbers, whereas hisotrical records only support whole numbers.

### Script Persistency

Variables only exist during the execution of a script. Once execution finishes of the script the value of the variables are reset back to 0.

Historical records are persistent in that they do not reset upon script execution finishing. As such, they can be used in seperate scripts at seperate times without the worry of resetting back to 0.

### Script Scope

Variables can only be used in the script they are defined in. You can use variables in other scripts using the Script command with the \[vars:\] parameter, however this is still quite limiting in scope.

Historical records, on the other hand, are globally reachable in scope for all scripts, making historical records much more flexible in this regard.

### Numeric Universality

Variables can be used anywhere a numeric literal can be used, for example:

``` title="cake-amount.txt" linenums="1"
var [cakeAmount] = [3]

// Give the actor cake
Inventory [actor] [add] [Cake] [cakeAmount]
```

This script, when executed, will give cake to an actor based on the variable _cakeAmount_. Here, we've set it to 3, so the actor will recieve 3 cake. Remaking this with History is not possible without variables.

## When to Use

In general, variables should be used when:

* The variable is needed only in the script it is defined in, or other scripts defined with the Script command.
* The variable is needed to calculate a value.
* The variable is needed in place of a numeric literal.
* The variable is needed to hold a fractional value.

Historical records should be used when:

* The record is needed in a variety of scripts, which are not connected.
* The record is needed to hold a value of some kind, such as a currency.
* The record is needed to count up or down.
* The record is needed to ever only hold a whole number.

Ultimately, it's your call when to use one over the other. However, learning about the limitations of each value type should give you a good idea as to when to use each one in the most effective way for your worlds.
