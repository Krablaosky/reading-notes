# Memory Storage

## [Understanding the Javascript Callstack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’?

a call is when we invoke a function to pull in a bunch of data, that uses the last and first out principle of temporary storage

2. How many ‘calls’ can happen at once?

javascript only has a single call stack which means they can only have one call happen at a time

3. What does LIFO mean?

LIFO means last in first out,that means the last data receives is the first one to be pushed out. in the instance of using cached storage it would be the last received data that we would push out first before receiving new data

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.


This example code from freecodecamp.org is a great example of call stack functions
```
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```


5. What causes a Stack Overflow?

stack overflow happens when there is a recursive function AKA function that never actually ends.It runs itself so many times without exit that at a certain point it can't accommodate any more information.It breaks the cycle and throws a stack error

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘reference error’?

a reference there is an error that pops up when you try to use a variable that is not yet declared. it's trying to reference something that does not exist.

2. What is a ‘syntax error’?

A syntax error is sometimes just utilizing the wrong quotation marks or trailing commas which can cause the code to read entirely different from its intended purpose.This sometimes makes the code unusable or violates a pre established rule that needs to exist.

3. What is a ‘range error’?

Arrange error happens in instances where you try to manipulate an object with an invalid length. Think about if you had an array length that was negative you wouldn't be able to access anything in it and would receive a range error.

4. What is a ‘type error’?

This error happens when trying to use an incompatible type in a function or in code.A good example is trying to access the property in an undefined type of variable.

5. What is a breakpoint?

a break point is a point in the code that you choose to not move beyond. It's something that is used frequently in debugging and allows you to test out the code in chunks and segments. you can see if your code can make it from point A to Z and if it gets caught up at G you'll know that that's exactly the spot where it's breaking.

6. What does the word ‘debugger’ do in your code?

adding the word debugger to your code it's important to put it below the code you want to run.This will show you the history before reaching that particular break point.It'll show you lots of useful information in terms of function calls and variables.
