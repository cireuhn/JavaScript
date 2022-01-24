`typeof true;`
`typeof flase;`
-->
"boolean"

Can be assigned directly or obtained as the result of some sort of check/comparison in the program

`let shaunLikesHamburgers = true;`
`let shaunLikesAsparagus = false;`
or
`let result = 5 > 4;`
->
true

One of the main uses for Boolean values is to control the flow of the program with things like if statements, while loops, or ternary operators

Other types (strings, numbers, objects, etc.) can be converted to boolean values...but it is not always obvious which they'll convert to

`let emptyString = "";`

`if (emptyString) {
	// this won't be executed
}`
- This if statement body won't be executed because it is considered <b>false</b>

<u>Falsey Values</u> ---> <b>Employers like to ask about these!</b>

1. "" (empty string)
2. 0
3. NaN (Not a Number)
4. 0n
5. null
6. undefined
7. false

