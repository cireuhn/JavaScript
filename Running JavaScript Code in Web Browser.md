1. Google Chrome or a web browser
- Open web browser
	- Click kebab menu -> More tools -> Developer tools -> Click on Console tab
	- Click Clear console button if there is any text
- Make the Console screen a seperate window
	- At the console tab, click the kebab menu -> Dock side, select undock into separate window

- All variables and things we define in the console will stay there and persist even if we click the clear console button

- Clear variables
	1.  Go back to web browser and refresh it
	2. In the console type  `window.location.reload()` and hit enter
	3. To delete a specific variable:
	    `delete [name of variable]`
		**Won't work for constants**
		
- This enables you to run snippets of JavaScript code by typing out an expression and hitting enter
	- When you need to type more than one line, the console should detect when a statement isn't finished and it won't execute the code until its actually complete (usually by adding all the closing brackets)

