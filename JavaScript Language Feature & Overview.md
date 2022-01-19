JavaScript is an interpreted language:
- Executed w/o compiling first
- The JavaScript runtime reads actual JavaScript code, not bytecode
- The exception to this is JIT compilation
	- It compiles JavaScript to bytecode before running it for performance reasons not out of necessity

JavaScript is dynamically and weaky typed language

Dynamic vs. Static Typing
- Dynamic Typing
	- Variable types are determined at runtime instead of compile time because JavaScript isn't a compiled language
	- Opposite is "**static typing**"
	- If variables are defined by generic words such as **let, var, or without any special word**
		- `let x = 5;` 
- Static Typing
	- Check types and then run the program for compiled languages like Java and C++
	- Usually define variables by  **type** such as **int or string** 
		- `int x = 5;`

Weakly vs. Strongly Typing
- Refers to how strictly does a language enforce its types

**Note:** In this example, lets say x = 5
`"The answer is " + x`
- In Python or Ruby, concatinating a **string and int** type would result in an error
- In JavaScript, it is weakly typed and so in most situations like this it would allow it
	- Although in practice, it is not good to rely on weak typing shortcuts because it can lead to unexpected behavior

JavaScript is single-threaded where it can only run one operation at a time
- Processing large amounts of data isn't one of JavaScripts strong suits
- In contrast, multi-threaded can run multiple operations in parallel

Summary:
JavaScript is <u>dynamically</u> and <u>weakly</u> typed - variables' types are determined at runtime and not enforced very strongly
- Interpreted (not compiled)
- Dynaically and weakly typed
- "Mostly" Object-Oriented
- Single-threaded

This is important to know because it will give you a feel of how JavaScript works and why certain things are done in a certain way

