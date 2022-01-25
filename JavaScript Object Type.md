`typeof { name: "Shaun" };`
->
"object"

JavaScript objects are a bit different than in other languages

`let person = {
	name: "Jane Doe",
	age: 35,
	eyeColor: "brown",
};`

- When we say object in the context of JavaScript, we are usually referring to what other languages refer to as hashes or key value maps
	- Basically a number of keys, which maps to some value
		- Person object, with name, age, and eye color keys

JavaScript objects allow us to group related pieces of data very easily
- JSON (JavaScript Object Notation) Format

 In the example above,

 name, age, eyecolor are <b>keys</b>
- Usually denoted by a string or symbol
- Each of these keys can be assign a value which can be <b> any of the eight JavaScript data types</b> (can even be another object so we can have nested objects)

Jane Doe, 35, brown are <b>values</b>

Object is defined inside the brackets  <b>{ }</b>

<u><b>Accessing Object Properties</b></u>

Two syntaxes to access object properties:

1. Using a dot followed by the property name
	- So if we defined a person object above, we can access by using object.key
`person.name` ---> "Jane Doe"
`person.age` ---> 35
`person.eyeColor` ---> "brown"

2. Square brackets [] with the name of the property we are trying to access
`person["name"]` ---> "Jane Doe"
`person["age"]`---> 35
`person["eyeColor"]`---> "brown"

- Property names here, unlike dot notation, are actual strings defined in between quotation marks

<b>Use Case for Accessing Object with Square Bracket</b>

- This syntax is very useful when needing to access property names dynamically such as when we define a variable containing the name of some property and use that to get the corresponding value

`let propertyName = "eyeColor";`

`person[propertyName];`
							---> "brown"

<b><u>Setting Object Properties</b></u>

We can change the age of the person by doing:

`person.age = 36;`
`person["age"] = 36;`
person.age -> 36

Doing either the dot or square bracket notation will set it to 36

<b><u> References vs. Copying</b></u>

JavaScript objects are assigned by reference

- The object is defined in memory and then the variable simply contains a reference to it
- This is usually handled by itself, but there are scenarios where it comes into play

On such scenario:
`let myObject = {
	a: 1,
	b: 2,
};`

`let myOtherObject = myObject;`

`myObject.a` --> 1
`myOtherObject.a` --> 1

`myOtherObject.a = 100`
`myObject.a` --> 100

If we have assign an object to a variable and then define another variable equal to the first variable, <u>both variables will be pointing to the same object in memory</u> instead of two different objects

As a result, if we make changes to one of the vairables, those changes will be reflected on the other one as well

`function myFunction(obj) {
	obj.name = "Changed!";
}`
`myFunction(myObject);`

`myObject.name` --> "Changed!"

- Objects are passed by reference in JavaScript, meaning if a function makes changes to an object inside the function body, those changes will be reflected on the actual object we passed
- Also true for arrays

<b><u>Setting Variables as Properties</b></u>

`let name = "Dana";`
`let age = 22;`

It happens quite a bit where we have some variables in our program where we want to put those variables into an object under a property with the same name as each of the variables. For instance:

`let person = {
	name: name,
	age: age,
}`

Where:

name: name
age: age

If we wanted to insert a name and age variable into an object. <u> In situations like this, instead of repeating the variable name, when it is the same as the property we want, we can just put the variable right inside the object</u>

`let person = {
	name,
	age,
}`
- JavaScript will take that to mean the same thing as name:name or age:age

<u><b>Keys with Special Characters</b></u>

- A thing to keep in mind when defining objects is that while property names are keys of our objects that can contain any character that a normal string can contain. <u>There are cases when we explicitly need to wrap our property names in quotation marks.</u>

`let person = {
	// ...
	"job-title": "developer",
}`

In this case the "job-title" variable needs to be wrapped in quotation marks (or single quotes and back ticks) because this key contains a - (dash)

Other cases:

`let operations = {
	// ...
	"+": "plus",
	"-": "minus",
	"*": "times",
	"/": "divided by",
}`

When defining our keys like this, we have to use square brackets to access the values of these properties

`operations["+"]`
`operations["-"]`

`operations.+`  --> Does not work

<u><b>The "null" Object</b></u>

In JavaScript, the <b>null value is used to signify the absence of data</b>

`let person = null;`
`typeof person;` --> "object"

We can let person = null to show that we don't have the person's data yet
- Null value is considered to be an object by JavaScript





