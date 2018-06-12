# Math

> **Note**: _any Math blocks that have unplugged sockets will read the unplugged spot as a 0._

* [0 \(basic number block\)](math.md#number)
* [=](math.md#=)
* [≠](math.md#≠)
* [&gt;](math.md#gt)
* [≥](math.md#gte)
* [&lt;](math.md#lt)
* [≤](math.md#lte)
* [+](math.md#add)
* [-](math.md#subtract)
* [x](math.md#multiply)
* [/](math.md#divide)
* \(\#exponent\)
* [random integer](math.md#randomint)
* [random fraction](math.md#randomfrac)
* [random set seed to](math.md#randomseed)
* [min](math.md#min)
* [max](math.md#max)
* [square root](math.md#sqrt)
* [absolute](math.md#abs)
* [neg](math.md#neg)
* [log](math.md#log)
* [e^](math.md#e)
* [round](math.md#round)
* [ceiling](math.md#ceiling)
* [floor](math.md#floor)
* [modulo](math.md#modulo)
* [remainder](math.md#remainder)
* [quotient](math.md#quotient)
* [sin](math.md#sin)
* [cos](math.md#cos)
* [tan](math.md#tan)
* [asin](math.md#asin)
* [acos](math.md#acos)
* [atan](math.md#atan)
* [atan2](math.md#atan2)
* [convert radians to degrees](math.md#convertrad)
* [convert degrees to radians](math.md#convertdeg)
* [format as a decimal](https://github.com/makeroid/docs/tree/6b89ce9eb8c93762fd238491325318be0e89c35f/format%20as%20a%20decimal/README.md)
* [is a number](math.md#isnumber)
* [convert number](math.md#convertnumber)

> ### _Can't find the math block you're looking for in the built-in blocks?_
>
> Some math blocks are dropdowns which means that they can be converted into different blocks. Here's a list of what is included in each dropdown:
>
> * **=, ≠, &gt;, ≥, &lt;, ≤**
>
> ![](../.gitbook/assets/equals.gif)
>
> * **min, max**
>
> ![](../.gitbook/assets/minmax.gif)
>
> * **square root, absolute, neg, log, e^, round, ceiling, floor**
>
> ![](../.gitbook/assets/sqrt.gif)
>
> * **modulo of, remainder of, quotient of**
>
> ![](../.gitbook/assets/modulo.gif)
>
> * **sin, cos, tan, asin, acos, atan**
>
> ![](../.gitbook/assets/sin.gif)
>
> * **convert radians to degrees, convert degrees to radians**
>
> ![](../.gitbook/assets/convert.gif)

## Basic Number Block {#number}

![](../.gitbook/assets/number.png)

Can be used as any positive or negative number \(decimals included\). Double clicking on the "0" in the block will allow you to change the number.

## = {#=}

![](../.gitbook/assets/equal.png)

Tests whether two numbers are equal and returns true or false.

## ≠

![](../.gitbook/assets/notequal.png)

Tests whether two numbers are not equal and returns true or false.

## &gt; {#gt}

![](../.gitbook/assets/greater.png)

Tests whether the first number is greater than the second number and returns true or false.

## ≥ {#gte}

![](../.gitbook/assets/greaterequal.png)

Tests whether the first number is greater than or equal to the second number and returns true or false.

## &lt; {#lt}

![](../.gitbook/assets/less.png)

Tests whether the first number is less than the second number and returns true or false.

## ≤ {#lte}

![](../.gitbook/assets/lessequal.png)

Tests whether the first number is less than or equal to the second number and returns true or false.

## + {#add}

![](../.gitbook/assets/plus.png)

Returns the result of adding any amount of blocks that have a number value together. Blocks with a number value include the basic number block, length of list or text, variables with a number value, etc. This block is a[mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html)and can be expanded to allow more numbers in the sum.

![](../.gitbook/assets/plus.gif)

## - {#subtract}

![](../.gitbook/assets/minus.png)

Returns the result of subtracting the second number from the first.

## x {#multiply}

![](../.gitbook/assets/multiply.png)

Returns the result of multiplying any amount of blocks that have a number value together. It is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) block and can be expanded to allow more numbers in the product.

![](../.gitbook/assets/multiply.gif)

## / {#divide}

![](../.gitbook/assets/divide.png)

Returns the result of dividing the first number by the second.

## ^ {#exponent}

![](../.gitbook/assets/exponent.png)

Returns the result of the first number raised to the power of the second.

## random integer {#randomint}

![](../.gitbook/assets/randomint.png)

Returns a random integer value between the given values, inclusive. The order of the arguments doesn't matter.

## random fraction {#randomfrac}

![](../.gitbook/assets/randomfrac.png)

Returns a random value between 0 and 1.

## random set seed to {#randomseed}

![](../.gitbook/assets/randomseed.png)

Use this block to generate repeatable sequences of random numbers. You can generate the same sequence of random numbers by first calling random set seed with the same value. This is useful for testing programs that involve random values.

## min {#min}

![](../.gitbook/assets/min.png)

Returns the smallest value of a set of numbers. If there are unplugged sockets in the block, min will also consider 0 in its set of numbers. This block is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) and a dropdown.

## max {#max}

![](../.gitbook/assets/max.png)

Returns the largest value of a set of numbers. If there are unplugged sockets in the block, max will also consider 0 in its set of numbers. This block is a [mutator](http://appinventor.mit.edu/explore/ai2/support/concepts/mutators.html) and a dropdown.

## square root {#sqrt}

![](../.gitbook/assets/sqrt.png)

Returns the square root of the given number.

## absolute {#abs}

![](../.gitbook/assets/abs.png)

Returns the absolute value of the given number.

## neg {#neg}

![](../.gitbook/assets/neg.png)

Returns the negative of a given number.

## log {#log}

![](../.gitbook/assets/log.png)

Returns the natural logarithm of a given number, that is, the logarithm to the base e \(2.71828...\).

## e^ {#e}

![](../.gitbook/assets/e.png)

Returns e \(2.71828...\) raised to the power of the given number.

## round {#round}

![](../.gitbook/assets/round.png)

Returns the given number rounded to the closest integer. If the fractional part is &lt; .5 it will be rounded down. It it is &gt; .5 it will be rounded up. If it is exactly equal to .5, numbers with an even whole part will be rounded down, and numbers with an odd whole part will be rounded up. \(This method is called _round to even_.\)

## ceiling {#ceiling}

![](../.gitbook/assets/ceiling.png)

Returns the smallest integer that's greater than or equal to the given number.

## floor {#floor}

![](../.gitbook/assets/floor.png)

Returns the greatest integer that's less than or equal to the given number.

## modulo {#modulo}

![](../.gitbook/assets/modulo.png)

Modulo\(a,b\) is the same as remainder\(a,b\) when a and b are positive. More generally, modulo\(a,b\) is defined for any a and b so that \(floor\(a/b\)× b\) + modulo\(a,b\) = a. For example, modulo\(11, 5\) = 1, modulo\(-11, 5\) = 4, modulo\(11, -5\) = -4, modulo\(-11, -5\) = -1. Modulo\(a,b\) always has the same sign as b, while remainder\(a,b\) always has the same sign as a.

## remainder {#remainder}

![](../.gitbook/assets/remainder.png)

Remainder\(a,b\) returns the result of dividing a by b and taking the remainder. The remainder is the fractional part of the result multiplied by b.

For example, remainder\(11,5\) = 1 because



In this case,  is the fractional part. We multiply this by b, in this case 5 and we get 1, our remainder.

Other examples are remainder\(-11, 5\) = -1, remainder\(11, -5\) = 1, and remainder\(-11, -5\) = -1.

## quotient {#quotient}

![](../.gitbook/assets/quotient.png)

Returns the result of dividing the first number by the second and discarding any fractional part of the result.

## sin {#sin}

![](../.gitbook/assets/sin.png)

Returns the sine of the given number in degrees.

## cos {#cos}

![](../.gitbook/assets/cos.png)

Returns the cosine of the given number in degrees.

## tan {#tan}

![](../.gitbook/assets/tan.png)

Returns the tangent of the given number in degrees.

## asin {#asin}

![](../.gitbook/assets/asin.png)

Returns the arcsine of the given number in degrees.

## acos {#acos}

![](../.gitbook/assets/acos.png)

Returns the arccosine of the given number in degrees.

## atan {#atan}

![](../.gitbook/assets/atan.png)

Returns the arctangent of the given number in degrees.

## atan2 {#atan2}

![](../.gitbook/assets/atan2.png)

Returns the arctangent of y/x, given y and x.

## convert radians to degrees {#convertrad}

![](../.gitbook/assets/convertrad.png)

Returns the value in degrees of the given number in radians. The result will be an angle in the range \[0, 360\)

## convert degrees to radians {#convertdeg}

![](../.gitbook/assets/convertdeg.png)

Returns the value in radians of the given number in degrees. The result will be an angle in the range \[-π , +π\)

## format as decimal {#format}

![](../.gitbook/assets/format.png)

Formats a number as a decimal with a given number of places after the decimal point. The number of places must be a non-negative integer. The result is produced by rounding the number \(if there were too many places\) or by adding zeros on the right \(if there were too few\).

## is a number {#isnumber}

![](../.gitbook/assets/isnumber.png)

Returns true if the given object is a number, and false otherwise.

## convert number {#convertnumber}

![](../.gitbook/assets/convertnumber.png)

Takes a text string that represents a positive integer in one base and returns a string that represents the same number is another base. For example, if the input string is 10, then converting from base 10 to binary will produce the string 1010; while if the input string is the same 10, then converting from binary to base 10 will produce the string 2. If the input string is the same 10, then converting from base 10 to hex will produce the string A.

