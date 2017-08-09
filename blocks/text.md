# Text Blocks

* [string](#string)
* [join](#join)
* [length](#length)
* [is empty?](#isempty)
* [compare texts](#compare)
* [trim](#trim)
* [upcase](#upcase)
* [downcase](#downcase)
* [starts at](#startsat)
* [contains](#contains)
* [split at first](#splitatfirst)
* [split at first of any](#splitatfirstofany)
* [split](#split)
* [split at any](#splitatany)
* [split at spaces](#splitatspaces)
* [segment](#segment)
* [replace all](#replaceall)

---

### " " {#string}

![](/assets/text/string.png)

Contains a text string.

This string can contain any characters \(letters, numbers, or other special characters\). On Makeroid, it will be considered a Text object.

---

### join {#join}

![](/assets/text/join.png)

Appends all of the inputs to make a single string. If no inputs, returns an empty string.

---

### length {#length}

![](/assets/text/length.png)

Returns the number of characters including spaces in the string. This is the length of the given text string.

---

### is empty {#isempty}

![](/assets/text/isempty.png)

Returns whether or not the string contains any characters \(including spaces\). When the string length is 0, returns true otherwise it returns false.

---

### compare texts &lt;&gt; = {#compare}

![](/assets/text/compare.gif)

Returns whether or not the first string is lexicographically &lt;, &gt;, or = the second string depending on which dropdown is selected.

A string a considered lexicographically greater than another if it is alphabetically greater than the other string. Essentially, it would come after it in the dictionary. All uppercase letters are considered smaller or to occur before lowercase letters. _cat would be &gt; Cat_.

---

### trim {#trim}

![](/assets/text/trim.png)

Removes any spaces leading or trailing the input string and returns the result.

---

### upcase {#upcase}

![](/assets/text/upcase.png)

Returns a copy of its text string argument converted to all upper case

---

### downcase {#downcase}

![](/assets/text/downcase.png)

Returns a copy of its text string argument converted to all lower case

---

### starts at {#startsat}

![](/assets/text/startsat.png)

Returns the character position where the first character of piece first appears in text, or 0 if not present. For example, the location of ana in havana banana is 4.

---

### contains {#contains}

![](/assets/text/contains.png)

Returns true if _piece appears in text_; otherwise, returns false.

---

### split at first {#splitatfirst}

![](/assets/text/splitatfirst.png)

Divides the given text into two pieces using the location of the first occurrence of at as the dividing point, and returns a two-item list consisting of the piece before the dividing point and the piece after the dividing point. Splitting _apple,banana,cherry,dogfood with a comma as the splitting point returns a list of two items: the first is the text apple and the second is the text banana,cherry,dogfood_. Notice that the comma after apple doesn't appear in the result, because that is the dividing point.

---

### split at first of any {#splitatfirstofany}

![](/assets/text/splitAtFirstOfAny.png)

Divides the given text into a two-item list, using the first location of any item in the list at as the dividing point.

Splitting _i love apples bananas apples grapes by the list \[ba_,_ap_\] would result in a list of two items the first being _i love and the second ples bananas apples grapes_.

---

### split {#split}

![](/assets/text/split.png)

Divides text into pieces using at as the dividing points and produces a list of the results. Splitting _one,two,three,four at _,_\(comma\) returns the list one two three four_. Splitting _one-potato,two-potato,three-potato,four at_-potato_, returns the list one two three four_.

---

### split at any {#splitatany}

![](/assets/text/splitAtAny.png)

Divides the given text into a list, using any of the items in at as the dividing point, and returns a list of the results.

Splitting _appleberry,banana,cherry,dogfood with at as the two-element list whose first item is a comma and whose second item is rry returns a list of four items: \[applebe, banana, che, dogfood,_\]

---

### split at spaces {#splitatspaces}

![](/assets/text/splitatspaces.png)

Divides the given text at any occurrence of a space, producing a list of the pieces.

---

### segment {#segment}

![](/assets/text/segment.png)

Extracts part of the text starting at start position and continuing for length characters.

---

### replace all {#replaceall}

![](/assets/text/replaceall.png)

Returns a new text string obtained by replacing all occurrences of the substring with the replacement.

Replace all with _She loves eating. She loves writing. She loves coding as the text, She as the segment, and Hannah as the replacement would result in Hannah loves eating. Hannah loves writing. Hannah loves coding_.

