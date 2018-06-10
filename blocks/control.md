# Control

## if & if else

![](../.gitbook/assets/if.png)

Tests a given condition. If the condition is true, performs the actions in a given sequence of blocks; otherwise, the blocks are ignored.

![](../.gitbook/assets/ifelse.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

![](../.gitbook/assets/ifelseif.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise tests the statement in the -else if section. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

The gif below shows how to use the if else mutator block.

![](../.gitbook/assets/if.gif)

## for each from to

![](../.gitbook/assets/forrange.png)

Runs the blocks in the do section for each numeric value in the range starting at _from_ and __ending at _to_, incrementing _number_ by the value of _by_ each time. Use the given variable name, _number_ to refer to the current value. You can change the name _number_ to something else if you wish.

## for each in list {#foreach}

![](../.gitbook/assets/foreach.png)

Runs the blocks in the do section for each item in the list. Use the given variable name, _item_, to refer to the current list item. You can change the name _item_ to something else if you wish.

## while {#while}

![](../.gitbook/assets/while.png)

Tests the _test_ condition. If true, performs the action given in _do_, then tests again. When test is false, the block ends and the action given in _do_ is no longer performed.

## if then else {#choose}

![](../.gitbook/assets/choose.png)

Tests a given condition. If the statement is true, performs the actions in the then _return_ sequence of blocks and returns the then _return_ value; otherwise, performs the actions in the else-return sequence of blocks and returns the else-return value.

## do {#doreturn}

![](../.gitbook/assets/doreturn.png)

Sometimes in a procedure or another block of code, you may need to do something and return something, but for various reasons you may choose to use this block instead of creating a new procedure.

## evaluate but ignore result {#evaluate}

![](../.gitbook/assets/evaluate.png)

Provides a "dummy socket" for fitting a block that has a plug on its left into a place where there is no socket, such as one of the sequence of blocks in the do part of a procedure or an if block. The block you fit in will be run, but its returned result will be ignored. This can be useful if you define a procedure that returns a result, but want to call it in a context that does not accept a result.

## open another screen {#openscreen}

![](../.gitbook/assets/openscreen.png)

Opens the screen with the provided name.

## open another screen with start value {#openscreenwithvalue}

![](../.gitbook/assets/openscreenwithvalue.png)

Opens another screen and passes a value to it.

## get start value {#getstartvalue}

![](../.gitbook/assets/getstartvalue.png)

Returns the start value given to the current screen.

This value is given from using open another screen with start value or close screen with value.

## close screen {#closescreen}

![](../.gitbook/assets/closescreen.png)

Closes the current screen.

## close screen with value {#closescreenwithvalue}

![](../.gitbook/assets/closescreenwithvalue.png)

Closes the current screen and returns a value to the screen that opened this one

## close application {#closeapp}

![](../.gitbook/assets/closeapp.png)

Closes the application.

## get plain start text {#getplainstarttext}

![](../.gitbook/assets/getplainstarttext.png)

Returns the plain text that was passed to this screen when it was started by another app. If no value was passed, it returns the empty text. For multiple screen apps, use get start value rather than get plain start text.

## close screen with plain text {#closescreenwithplaintext}

![](../.gitbook/assets/closescreenwithplaintext.png)

Closes the current screen and passes text to the app that opened this one. This command is for returning text to non-App Inventor activities, not to App Inventor screens. For App Inventor Screens, as in multiple screen apps, use Close Screen with Value, not Close Screen with Plain Text.

