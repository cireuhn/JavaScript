1. The basic syntax for JavaScript statements

<u>Example 1 Seicolon usage:</u>
`let x = 5;`
vs
`let x = 5`

- Don't neccessarily need to end it with a semicolon, but it is good to use it
**Exception:** When using if statements in functions, most developers leave it off since there is already a closing bracket

<u>Example 2 Statements in JavaScript:</u>
`let myVeryLongString
	"This statement is too long for one line";`

- Shorter JavaScript statements are usually written all in one line, but affects readability of code
- Longer ones can be broken into multiple lines so it doesn't go over the edge of our IDE or increase readability -- We can split statements into multple lines
	`let myObject = {a: 1, b: 2, c: 3};`
	vs
	`let myObject = {
	        a: 1,
			b: 2,
			c: 3,
		};`
2. How to write comments

`let x = 5; // This is a single line comment`
vs
`// This is a 
// multi-line comment`
vs
`/*
      This is a BETTER
	multi-line comment
*/`

- These are three ways to do comments and the last one would be the best multi-line comment method

4. How to print things to the console

`let someVariable = 100;

console.log(someVariable);`

output:
Prints "100" to the console

- Useful way to debug code in JavaScript is using a **console.log function** 
- When using the console.log function with JavaScript, the console is based on what we are running (IE. Front-end, Back-end, mobile, and so on)
	- If we are running our code on the front-end and our code contains a console.log, it will be printed inside the browser's console
		- This is what happens when we run a JavaScript file from inside our browser too
	- If we are running the code on the back-end, it will be printed inside whatever terminal we are running our code from