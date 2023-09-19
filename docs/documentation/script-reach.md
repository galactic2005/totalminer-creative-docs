# Player Specification

When using commands or functions, you may notice some will include parameters to specify what players are affected by said command/function. For example:

``` title="player-specification.txt" linenums="1"
// Local specification
Notify [Hello, Player.] [local]

// Global specification
Notify [Hello, World.] [global]

// Admin specification
Notify [Hello, Admins.] [admin]
```

These parameters can be helpful in ensuring only certain players are affected, instead of affecting everyone in the game in what could be considered unnecessary (such as notifying everyone that they're level 5, even if only one player has reached level 5).

## Local

Using the \[local\] parameter will only 

local
remote
global
admin
clan

## Clock Time Usage in Scripting

Clock time is used in the following commands/functions:

=== "TMScript"

    * [IsClock](/tmscript/commands/query-commands/isclock/)
    * [IsDayTime](/tmscript/commands/query-commands/isdaytime/)
    * [var](/tmscript/commands/var/)

=== "LUA"
