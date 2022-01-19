1. "Number" type

<u>Decimal notation</u>
`let x = 5;
typeof x;`

output: "number"

`let pi = 3.1415l
	typeof pi;`

output: "number"

These are seen to be the same exact data type, a number

In JavaScript, there are no seperate types for integers or floating point numbers
	- Although there is a separate data type for very big numbers

`let z = -40;`

Negative numbers are allowed

Other Number Formats:
<u>Hex notation</u>

`let hex = 0x2A`
Putting 0x in the beginning of a number defines it as hex

<u>Other Number Bases</u>
`let binary = 0b101010;`
- Define binary by putting 0b before a number
`let octal = 0o52;`
- Define octabl by putting 0o before a number
`let sixyMillion = 6e7;`
- For very large numbers or small, we can use scientific notation
- e7 represents seven zeros so our example is 6 followed by 7 zeros, or it translates into six times 10 to the seventh power

<u>"NaN" and "Infinity"</u>
NaN & Infinity are both considered to be number types

`let answer = 10 * "oops";`

output: Nan

NaN = Not a number
- It means that it tried to perform some mathematical operations with values that aren't numbers
- Can happen if we didn't validate our code

`let answer = 9 / 0;`

output: Infinity

- Negative infinity is also a possible value
Several ways it can happen
- Divide by 0
- Work with numbers that are way to big for JavaScript
	-  `let answer = Math.pow(10, 999);`
	- Output: Infinity

<u>Number Operations</u>
4 + 4
55 - 12
3 * 10
24 / 6

The "Math" Object
- Contains useful JavaScript math operations such as exponentiation, the square root function, sin, cos, and many other math operation
`let x = Math.pow (10, 3);`
`let y = Math.sqrt(144);`
`Math.abs(x);`
`Math.max(x, y);
Math.min(x,);
Math.ceil(1.8);
Math.floor(1.8)
Math.round(1.8);
Math.sin(x);
...`

<u>Number Precision</u>
All number values are stored as 64-bit floating point

**Big numbers are only accurate to about 15 digits**

`let y = 12345678901234567;`

y is 1234567890123456***8***

`let x = 0.1 + 0.7;`

0.7999999999999999 -- 15 9's

Important for Two Reasons
1. It is not a good to compare two decimal numbers for equality for JavaScript because two numbers that should be equal may not be seen as such by JavaScript

`let x = 0.1 + 0.7;`

`if (x === 0.8) {
	// never executes!
}`

There are several ways around this:

`let x = 0.1 + 0.7;`

`if (Math.round(x * 10) === Math.round (0.8*10)) {
	// this works!
}`

One way is to multiple our decimal numbers by some power of 10 and then use the math.round to get rid of the rest of the digits


