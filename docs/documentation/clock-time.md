# Clock Time

Clock time is a mechanic in Total Miner that is an important part of various aspects of the world, such as when monsters start spawning or when it is considered day time through scripting. As such, it is important to understand what it is and how it can be used. This documentation is created to achieve this goal.

## What is Clock Time

Clock time is the value given when one of the following methods is used:

=== "TMScript"
    Clock time is given when the \[Clock:\] built-in value type is used within the var command as shown:

    ``` title="clock-time.txt" linenums="1"
    // Get clock time
    var [clockTime] = [Clock:]
    ```

=== "LUA"
    Clock time is given with the get_hour() function as shown:

    ``` title="clock-time.lua" linenums="1"
    -- Get clock time
    local clock_time = get_hour()
    ```

When getting the current clock time, it will output a number between 0 to 24, indicating the time in a fashion similar to hours in a day.

## Clock Time Modification

There are currently two ways clock time is modified, which is by the Day/Night Cycle and Time Forwarding/Reversing.

### Day/Night Cycle

When the *Day/Night Cycle* option is enabled, clock time increments roughly by 0.019 per second, meaning a full in-game day is roughly 1,641.6 seconds, or 27.36 minutes.

In non-creative worlds, there is no option to disable the Day/Night Cycle.

### Time Forwarding/Rewinding

In creative worlds, players with the Admin permission gain the ability to change clock-time by either going forward or backwards in clock time, referred to by the Game Help menu as *Time Forwarding/Reversing*.

When Time Forwarding/Reversing, the clock time changes by roughly 2.33 per second. Forwarding time increments clock time by 2.33, while reversing time deincrements clock time by 2.33.

## Clock Time Usage in Scripting

Clock time is used in the following commands/functions:

=== "TMScript"

    * [IsClock](/tmscript/commands/query-commands/isclock/)
    * [IsDayTime](/tmscript/commands/query-commands/isdaytime/)
    * [var](/tmscript/commands/var/)

=== "LUA"
