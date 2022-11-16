# Debugging in JS

Debugging is extremely important with coding and is a crucial part of what we do to make everything work. It can be something as simple as checking why something isnt working with a very specific error message to a more ambiguous testing different results to see how the function reacts with every kind of answer.

1. Name some key differences between a Syntax Error and a Logic Error.

Some key features of a syntax error is that they are usually spelling errors that prevent the code from working either at all or at some part. There is usually a very clear message as to what is wrong and will help guide you to the issue.

On the other hand logic errors are where the syntax is correct but the code doesn't do what you are looking for. It might be that you are asking for two numbers to add together and you type in fish and sticks. The syntax will be right but the logic is wrong.

2. List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.

In past labs I have encountered both types of errors. I have run into more than my fair share of syntax issues. A lot of the time it's that I was missing a `;` or a `:` and it prevented the rest of the code from running. I used the console and VS Code to check where those issues were and go back to inspect them. For my logic codes it's been everything from forgetting to properly link my CSS sheet to nesting the wrong for loop. I tried to work section by section to make sure that everything worked the way it should. I isolated each section to figure out what went right and what went wrong and console logged the instances as they progressed so that I could track it.


3. How will this topic continue to influence your long term goals?

This topic will be a part of what we do all the time going forward. There will always be bugs with code and unexpected errors and it will be crucial to inspect each piece to get it working. This will always be a core part of the coding process.

## JS Debugger

1. How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

The Javascript debugging tool will help you find the moments that things break. The tool shows you the exact spot and location where it broke and will try to let you know what it thinks is wrong.

2. Define what a breakpoint is.

A breakpoint is the part in the code where it stops running and cannot continue. It is something you can set to basically try out code up to a certain point without having to run the whole thing.

3. What is the call stack?

The call stack shows the code that was executed and all instances where it is not working. It is something you can click on to have it take you directly to the line of code that isn't working and see where it is going wrong.