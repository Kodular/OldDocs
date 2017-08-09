# Math Blocks

> **Note**:_ any Math blocks that have unplugged sockets will read the unplugged spot as a 0._

* [0 \(basic number block\)](#number)
* [=](#=)
* [≠](#≠)
* [&gt;](#gt)
* [≥](#gte)
* [&lt;](#lt)
* [≤](#lte)
* [+](#add)
* [-](#subtract)
* [x](#multiply)
* [/](#divide)
* [^](#exponent)
* [random integer](#randomint)
* [random fraction](#randomfrac)
* [random set seed to](#randomseed)
* [min](#min)
* [max](#max)
* [square root](#sqrt)
* [absolute](#abs)
* [neg](#neg)
* [log](#log)
* [e^](#e)
* [round](#round)
* [ceiling](#ceiling)
* [floor](#floor)
* [modulo](#modulo)
* [remainder](#remainder)
* [quotient](#quotient)
* [sin](#sin)
* [cos](#cos)
* [tan](#tan)
* [asin](#asin)
* [acos](#acos)
* [atan](#atan)
* [atan2](#atan2)
* [convert radians to degrees](#convertrad)
* [convert degrees to radians](#convertdeg)
* [format as a decimal](/format as a decimal)
* [is a number](#isnumber)
* [convert number](#convertnumber)

---

> #### _Can't find the math block you're looking for in the built-in blocks?_
>
> Some math blocks are dropdowns which means that they can be converted into different blocks. Here's a list of what is included in each dropdown:
>
> * **=, ≠, &gt;, ≥, &lt;, ≤**
>
> ![](/assets/math/equals.gif)
>
> * **min, max**
>
> ![](/assets/math/minmax.gif)
>
> * **square root, absolute, neg, log, e^, round, ceiling, floor**
>
> ![](/assets/math/sqrt.gif)
>
> * **modulo of, remainder of, quotient of**
>
> ![](/assets/math/modulo.gif)
>
> * **sin, cos, tan, asin, acos, atan**
>
> ![](/assets/math/sin.gif)
>
> * **convert radians to degrees, convert degrees to radians**
>
> ![](/assets/math/convert.gif)

---

### Basic Number Block {#number}

![](/assets/math/number.png)

Can be used as any positive or negative number \(decimals included\). Double clicking on the "0" in the block will allow you to change the number.

---

### = {#=}

![](/assets/math/equal.png)

Tests whether two numbers are equal and returns true or false.

---

### ≠

![](/assets/math/notequal.png)

Tests whether two numbers are not equal and returns true or false.

---

### &gt; {#gt}

![](/assets/math/greater.png)

Tests whether the first number is greater than the second number and returns true or false.

---

### ≥ {#gte}

![](/assets/math/greaterequal.png)

Tests whether the first number is greater than or equal to the second number and returns true or false.

---

### &lt; {#lt}

![](/assets/math/less.png)

Tests whether the first number is less than the second number and returns true or false.

---

### ≤ {#lte}

![](/assets/math/lessequal.png)

Tests whether the first number is less than or equal to the second number and returns true or false.

---

### + {#add}

![](/assets/math/plus.png)

Returns the result of adding any amount of blocks that have a number value together. Blocks with a number value include the basic number block, length of list or text, variables with a number value, etc. This block is a[mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html)and can be expanded to allow more numbers in the sum.

![](/assets/math/plus.gif)

---

### - {#subtract}

![](/assets/math/minus.png)

Returns the result of subtracting the second number from the first.

---

### x {#multiply}

![](/assets/math/multiply.png)

Returns the result of multiplying any amount of blocks that have a number value together. It is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) block and can be expanded to allow more numbers in the product.

![](/assets/math/multiply.gif)

---

### / {#divide}

![](/assets/math/divide.png)

Returns the result of dividing the first number by the second.

---

### ^ {#exponent}

![](/assets/math/exponent.png)

Returns the result of the first number raised to the power of the second.

---

### random integer {#randomint}

![](/assets/math/randomint.png)

Returns a random integer value between the given values, inclusive. The order of the arguments doesn't matter.

---

### random fraction {#randomfrac}

![](/assets/math/randomfrac.png)

Returns a random value between 0 and 1.

---

### random set seed to {#randomseed}

![](/assets/math/randomseed.png)

Use this block to generate repeatable sequences of random numbers. You can generate the same sequence of random numbers by first calling random set seed with the same value. This is useful for testing programs that involve random values.

---

### min {#min}

![](/assets/math/min.png)

Returns the smallest value of a set of numbers. If there are unplugged sockets in the block, min will also consider 0 in its set of numbers. This block is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) and a dropdown.

---

### max {#max}

![](/assets/math/max.png)

Returns the largest value of a set of numbers. If there are unplugged sockets in the block, max will also consider 0 in its set of numbers. This block is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) and a dropdown.

---

### square root {#sqrt}

![](/assets/math/sqrt.png)

Returns the square root of the given number.

---

### absolute {#abs}

![](/assets/math/abs.png)

Returns the absolute value of the given number.

---

### neg {#neg}

![](/assets/math/neg.png)

Returns the negative of a given number.

---

### log {#log}

![](/assets/math/log.png)

Returns the natural logarithm of a given number, that is, the logarithm to the base e \(2.71828...\).

---

### e^ {#e}

![](/assets/math/e.png)

Returns e \(2.71828...\) raised to the power of the given number.

---

### round {#round}

![](/assets/math/round.png)

Returns the given number rounded to the closest integer. If the fractional part is &lt; .5 it will be rounded down. It it is &gt; .5 it will be rounded up. If it is exactly equal to .5, numbers with an even whole part will be rounded down, and numbers with an odd whole part will be rounded up. \(This method is called _round to even_.\)

---

### ceiling {#ceiling}

![](/assets/math/ceiling.png)

Returns the smallest integer that's greater than or equal to the given number.

---

### floor {#floor}

![](/assets/math/floor.png)

Returns the greatest integer that's less than or equal to the given number.

---

### modulo {#modulo}

![](/assets/math/modulo.png)

Modulo\(a,b\) is the same as remainder\(a,b\) when a and b are positive. More generally, modulo\(a,b\) is defined for any a and b so that \(floor\(a/b\)× b\) + modulo\(a,b\) = a. For example, modulo\(11, 5\) = 1, modulo\(-11, 5\) = 4, modulo\(11, -5\) = -4, modulo\(-11, -5\) = -1. Modulo\(a,b\) always has the same sign as b, while remainder\(a,b\) always has the same sign as a.

---

### remainder {#remainder}

![](/assets/math/remainder.png)

Remainder\(a,b\) returns the result of dividing a by b and taking the remainder. The remainder is the fractional part of the result multiplied by b.

For example, remainder\(11,5\) = 1 because

$$11/5 = 2\frac15$$

In this case, $$\frac15$$ is the fractional part. We multiply this by b, in this case 5 and we get 1, our remainder.

Other examples are remainder\(-11, 5\) = -1, remainder\(11, -5\) = 1, and remainder\(-11, -5\) = -1.

---

### quotient {#quotient}

![](/assets/math/quotient.png)

Returns the result of dividing the first number by the second and discarding any fractional part of the result.

---

### sin {#sin}

![](/assets/math/sin.png)

Returns the sine of the given number in degrees.

---

### cos {#cos}

![](/assets/math/cos.png)

Returns the cosine of the given number in degrees.

---

### tan {#tan}

![](/assets/math/tan.png)

Returns the tangent of the given number in degrees.

---

### asin {#asin}

![](/assets/math/asin.png)

Returns the arcsine of the given number in degrees.

---

### acos {#acos}

![](/assets/math/acos.png)

Returns the arccosine of the given number in degrees.

---

### atan {#atan}

![](/assets/math/atan.png)

Returns the arctangent of the given number in degrees.

---

### atan2 {#atan2}

![](/assets/math/atan2.png)

Returns the arctangent of y/x, given y and x.

---

### convert radians to degrees {#convertrad}

![](/assets/math/convertrad.png)

Returns the value in degrees of the given number in radians. The result will be an angle in the range \[0, 360\)

---

### convert degrees to radians {#convertdeg}

![](/assets/math/convertdeg.png)

Returns the value in radians of the given number in degrees. The result will be an angle in the range \[-π , +π\)

---

### format as decimal {#format}

![](/assets/math/format.png)

Formats a number as a decimal with a given number of places after the decimal point. The number of places must be a non-negative integer. The result is produced by rounding the number \(if there were too many places\) or by adding zeros on the right \(if there were too few\).

---

### is a number {#isnumber}

![](/assets/math/isnumber.png)

Returns true if the given object is a number, and false otherwise.

---

### convert number {#convertnumber}

![](/assets/math/convertnumber.png)

Takes a text string that represents a positive integer in one base and returns a string that represents the same number is another base. For example, if the input string is 10, then converting from base 10 to binary will produce the string 1010; while if the input string is the same 10, then converting from binary to base 10 will produce the string 2. If the input string is the same 10, then converting from base 10 to hex will produce the string A.

