## The "string" Type
`let singleQuoteString = 'Hello!';`

`let doubleQuoteString = "Hello!";`

``let backtickString = `Hello!`;``

- Provide same functionality for string

``let backtickString = `Hello ${name}`;
- Backtick enables easy string interpolation which is allowing us to insert variables into our strings

`let myString = "Hello!";`
`myString.length;` -> 6
`myString.charAt(0);` -> "H"
`myString.toUpperCase();` -> "HELLO!"
`myString.toLowerCase();` -> "hello!"
- String have properties that we can access to get information about the string itself..for example:
	- Length outputs the length of string
	- CharAt gives us the character in the string at a given position
	- toUpperCase() and toLowerCase() capitalizes and lowercase the string respectively

## The Escape Character

`let question =
	""How do I use quotes?" she asked";`

- Since we are using double quotes, in the first instance, JavaScript will see "" as an empty string, and second, see " she asked"

To resolve this use the escape character (\) to tell JavaScript I want to ignore the normal syntactic function of a character and just display it as is in the string

`let question =
	"\"How do I use quotes?\" she asked";

- Use escape character for other scenarios such as single quotes as well
- One way to work around this is to use both double and single qoutes

`let question =
	'"How do I use quotes?" she asked';`

Escape character (\) also enable another function called special functions such as newlines and tabs inside of strings

`let poetry = "One fish\nTwo fish";`
-->
One fish
Two fish

- \n (backslash n) is the escape sequence for a newline

If you want to put the backslash character inside a string, do it twice to cancel the escape function

`let windowsFilePath =
	"C:\\Documents\\some-file.js";`
	--->
	C:\Documents\some-files.js

## Concatenating Strings
`let firstName = "John";`
`let lastName = "Doe";`

`let fullName = firstName + " " + lastName;`
or
`let fullName = firstName.concat(" ")`
						`.concat(lastName);`
-->
"John Doe"

- Can use both empty quotes or concat method

<u>Adding Strings and Numbers together (or other data types)</u>
`let x = 5;`
`let myString = "x is " + x`
-->
"x is 5"


`let x = 5;
let y = 8;`

`let myString = "x plus y is " + x + y`
---> Breakdown
"x plus y is " + x + y
->
"x plus y is 5" + 8
-> append 8 to the end
"x plus y is 58"

To resolve this and get it to behave properly

- Wrap  (x + y) in parenthese so it gets executed first
`let myString = "x plus y " + (x + y)`
-->
"x plus y is " + 13
->
"x plus y is 13"

or

`x + y + " is the answer"`

- Move x + y to the left so it executes first