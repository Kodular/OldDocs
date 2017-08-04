# Control Blocks

* [if & if else](#if)
* [for each from to](#forrange)
* [for each in list](#foreach)
* [while](#while)
* [if then else](#choose)
* [do](#doreturn)
* [evaluate but ignore result](#evaluate)
* [open another screen](#openscreen)
* [open another screen with start value](#openscreenwithvalue)
* [get start value](#getstartvalue)
* [close screen](#closescreen)
* [close screen with value](#closescreenwithvalue)
* [close application](#closeapp)
* [get plain start text](#getplainstarttext)
* [close screen with plain text](#closescreenwithplaintext)

---

### if & if else {#if}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/if.png)

Tests a given condition. If the condition is true, performs the actions in a given sequence of blocks; otherwise, the blocks are ignored.

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/ifelse.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/ifelseif.png)

Tests a given condition. If the result is true, performs the actions in the -do sequence of blocks; otherwise tests the statement in the -else if section. If the result is true, performs the actions in the -do sequence of blocks; otherwise, performs the actions in the -else sequence of blocks.

The gif below shows how to use the if else mutator block.  
![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/if.gif)

---

### for each from to {#forrange}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/forrange.png)

Runs the blocks in the do section for each numeric value in the range starting at_from\_and ending at\_to_, incrementing\_number\_by the value of\_by\_each time. Use the given variable name,\_number\_to refer to the current value. You can change the name\_number\_to something else if you wish.

---

### for each in list {#foreach}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/foreach.png)

Runs the blocks in the do section for each item in the list. Use the given variable name,_item_, to refer to the current list item. You can change the name\_item\_to something else if you wish.

---

### while {#while}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/while.png)

Tests the -test condition. If true, performs the action given in -do , then tests again. When test is false, the block ends and the action given in -do is no longer performed.

---

### if then else {#choose}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/choose.png)

Tests a given condition. If the statement is true, performs the actions in the then-return sequence of blocks and returns the then-return value; otherwise, performs the actions in the else-return sequence of blocks and returns the else-return value.

---

### do {#doreturn}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/doreturn.png)

Sometimes in a procedure or another block of code, you may need to do something and return something, but for various reasons you may choose to use this block instead of creating a new procedure.

---

### evaluate but ignore result {#evaluate}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/evaluate.png)

Provides a "dummy socket" for fitting a block that has a plug on its left into a place where there is no socket, such as one of the sequence of blocks in the do part of a procedure or an if block. The block you fit in will be run, but its returned result will be ignored. This can be useful if you define a procedure that returns a result, but want to call it in a context that does not accept a result.

---

### open another screen {#openscreen}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/openscreen.png)

Opens the screen with the provided name.

---

### open another screen with start value {#openscreenwithvalue}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/openscreenwithvalue.png)

Opens another screen and passes a value to it.

---

### get start value {#getstartvalue}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/getstartvalue.png)

Returns the start value given to the current screen.

This value is given from usingopen another screen with start valueorclose screen with value.

---

### close screen {#closescreen}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/closescreen.png)

Closes the current screen.

---

### close screen with value {#closescreenwithvalue}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/closescreenwithvalue.png)

Closes the current screen and returns a value to the screen that opened this one

---

### close application {#closeapp}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/closeapp.png)

Closes the application.

---

### get plain start text {#getplainstarttext}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/getplainstarttext.png)

Returns the plain text that was passed to this screen when it was started by another app. If no value was passed, it returns the empty text. For multiple screen apps, use get start value rather than get plain start text

---

### close screen with plain text {#closescreenwithplaintext}

![](http://appinventor.mit.edu/explore/sites/all/files/UserGuide/blocks/control/closescreenwithplaintext.png)

Closes the current screen and passes text to the app that opened this one. This command is for returning text to non-App Inventor activities, not to App Inventor screens. For App Inventor Screens, as in multiple screen apps, use Close Screen with Value, not Close Screen with Plain Text.

