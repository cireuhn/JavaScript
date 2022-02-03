In JavaScript arrays are ordered collection of values, usually defined in square brackets

`[1,2,3,4,5,6,7]`

`let myArray = [
	1,
	2,
	"Three",
	{ message: "Hello" },
	[1,2,3]
]`

The values in an array can be any of the basic data types and the values in the array don't all have to be the same data type

Arrays are considered "objects"

`typeof [1, 2, 3];` -> "object"

You can call the elements in an array by using square brackets and an index

`let myArray = [
	"zero",
	"one",
	"two",
	"three",
];`

`myArray[0]` -> "zero"
`myArray[1]` -> "one"

In JavaScript as in most other programming languages, <u>the indices of an array starts at 0 and go up to the length of the array minus one.</u>


You can also set the value of any of the array indices by using square brackets like this:

`myArray[1] = "uno";`
`myArray[1]` -> "uno"

`var myArray = [
	"zero",
	"one",
	"two",
	"three",
];`

Arrays in have a built in length property which allows us to get the number of elements in an array. This number is one greater than the last index in the array (because arrays start at 0)

`myArray.length;` -->4

JavaScript arrays have quite a few built-in array methods. 

For example:
- The <b>push</b> method, adds an element onto the array

`myArray.push("four");`

`myArray`
->
`["zero", "one", "two", "three", "four"]`

- The <b>pop</b> method which returns the last element of the array and removes it

`myArray.pop();` -> "three"

`myArray`
->
`["zero", "one", "two"]`

- The <b>indexof</b> method which returns the index of a given value in the array

`myArray.indexOf("two");` --> 2

- Or outputs -1 if the value is not found in the array

`myArray.indexOf("one million");` -> -1

- Many other examples to be discussed later
`myArray.map(x => x.toUpperCase());`
`myArray.filter(x => x.length <4);`
`myArray.sort();`

<u>Trailing Comma</u>

`let myArray = [
	"zero",
	"one",
	"two",
];`

`let person = {
	name: 'Jane Doe',
	age: 35,
	eyeColor: 'brown',
};`

You don't need the last comma, but it is good practice because you may forget to add one in the preceeding line when you add more to the code. Ending up getting a syntax error when you run the code.

For example:

`let person = {
	name: 'Jane Doe',
	age: 35,
	eyeColor: 'brown'` (missing comma)
	`jobTitle: "developer",
};`
