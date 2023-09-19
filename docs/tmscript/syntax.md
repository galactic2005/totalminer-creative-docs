# Syntax

## Commands and Parameters

TMScript, like other programming languages, contains functions. Functions are called commands in TMScript. The following is the syntax of a command:

**Command \[parameter\] \[parameter\]...\[parameter\]**

The first word is that of the command. The defined command allows for different functions to be executed. For example, the Inventory command can modify actor and block inventories, whilst the Notify command can display notification messages on the top-left side of the screen.

Following this, most commands offer parameters. Parameters provide data for the command. For example, the Clan command offers \[name\] and \[bannerID\] as parameters, which are used to define what clan the player joins and what banner ID is used for that clan.

## Case sensitivity

TMScript is a case-insensitive language. This means that "value" and "VALUE" mean the same thing in this language. Here's a demonstration:

``` title="case-insensitive.txt" linenums="1"
var [value] = [10]

// This will work
Notify [[value]] [local] [0,0,0]

// But also this
notify [[value]] [local] [0,0,0]

// And this
NOTIFY [[VALUE]] [LOCAL] [0,0,0]

// And even mixing up the capalitized letters
notIFY [[VALue]] [LoCal] [0,0,0]
```

Running this script will create four notification messages, outputting "10" each time despite the casing being different in both the commands and parameters.

## Comments

Comments are created by using double slashes. There is no comment ending indicator, so the rest of the line is considered a comment.

``` title="comments.txt" linenums="1"
// Comments can be used to document your scripts
// This can help make scripts more readable to yourself or other scripters

// Comments are indicated by // at the beginning of a script
// Whilst they are generally built to leave text, you can comment commands
// This is because they are technically considered a comment, such as:

// Notify [Hello, World!] [global] [0,0,0]
// Since this is considered a comment, the command will not run.

// Additionally, you you could aso put the // after commands
// Such as in the following example:
Notify [Test notification] [global] [0,0,0] // Test

// Though they are less readable and not recommended
```
