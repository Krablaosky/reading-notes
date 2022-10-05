# Expressions & Operators

## What is an expression?

expressions are sections of code that end up outputting a value.
 There are two types of expressions, ones that assign value and ones that only evaluate.
  We covered what [operators](javascript2.md) were in the last section and now we dig into how they work in an expression.

For instance we can assign different values to things like `x = 7` which uses the `=` operator.
we can use them to do all types of mathematical arithmatic, but if we don't use that value later in a declaration then that information will dissapear. I.E. we need to assign it to something like `const z = 3 + 4'

Some important things to remember about expressions are the order of operators. `* and /` will always happen before `+ or -`.

Javascript has binary(requiring two operands) and unary operators. In the case of `3 + 4` or `x * y` these are called infix binary operators because the operator is between two operands.
![Operators](img/operators.png)

We can use these to assign to properties like in the below example

```javascript
const obj = {};

obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }.
```

If an expression does not evaluate to an object, then assignments to properties of that expression do not assign:

```javascript
const val = 0;
val.x = 3;

console.log(val.x); // Prints undefined.
console.log(val); // Prints 0.
```

When looking at putting functions inside of functions it is a slippery slope to causing pileups and miscommunications and is generally discouraged. By chaining or nesting an assignment expression, its result can itself be assigned to another variable. It can be logged, it can be put inside an array literal or function call, and so on.

```javascript
let x;
const y = (x = f()); // Or equivalently: const y = x = f();
console.log(y); // Logs the return value of the assignment x = f().

console.log(x = f()); // Logs the return value directly.

// An assignment expression can be nested in any place
// where expressions are generally allowed,
// such as array literals' elements or as function calls' arguments.
console.log([ 0, x = f(), 0 ]);
console.log(f(0, x = f(), 0));
```

## Comparison Operators

Comparison operators work pretty simply on whether the operands fit into a few conditions. IF they are `=`, `!=`, `>`, `<` etc.
[comparison](img/comparison.png)

## Assignment operators

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

There are also compound assignment operators that are shorthand for the operations listed in the following table:

![Assignment Operators](img/Assignment%20operators.png)

### Arithmatic Operators

![Arithmetic](img/arithmetic.png)

### The conditional Operator

The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition. The syntax is:

```javascript
condition ? val1 : val2
```

If the condition is true, the operator has the value of val1. Otherwise it has the value of val2. You can use the conditional operator anywhere you would use a standard operator.

For example,

```javascript
const status = age >= 18 ? 'adult' : 'minor';
```

This statement assigns the value "adult" to the variable status if age is eighteen or more. Otherwise, it assigns the value "minor" to status.

### The comma operator

This operator evaluates both operands and retirns the valie of the last operand. It is most commonly used inside a `for` loop where lots of different variables can be updated aand evaluated at a time.

### Relational Operators

The `in` operator returns the value of `true` if a specific property is inside an object or located within it.
This example shows a great use of the `in` operator.

```javascript
// Arrays
const trees = ['redwood', 'bay', 'cedar', 'oak', 'maple'];
0 in trees;        // returns true
3 in trees;        // returns true
6 in trees;        // returns false
'bay' in trees;    // returns false (you must specify the index number,
                   // not the value at that index)
'length' in trees; // returns true (length is an Array property)

// built-in objects
'PI' in Math;          // returns true
const myString = new String('coral');
'length' in myString;  // returns true

// Custom objects
const mycar = { make: 'Honda', model: 'Accord', year: 1998 };
'make' in mycar;  // returns true
'model' in mycar; // returns true
```

## Loops & Iterations

Think about a hotwheels track, you set up 2 of the speed motors in a loop so that they continue to push the car in a circle, it will never end. that is unless we end the loop via stopping it or `breaking` it.

There are quite a few types of loops and each one does something a little different. The different types of loops are as follows.

* for statement
* do...while statement
* while statement
* labeled statement
* break statement
* continue statement
* for...in statement
* for...of statement

### `For` Loop

The `for` loop repeats itself until a specific condition is false. You specify the criteria and the result and the loop runs until it is met. Sometimes infinetly. This example shows a statement that counts the number of options in a scrolling list.

```javascript
<form name="selectForm">
  <label for="musicTypes">Choose some music types, then click the button below:</label>
  <select id="musicTypes" name="musicTypes" multiple>
    <option selected>R&B</option>
    <option>Jazz</option>
    <option>Blues</option>
    <option>New Age</option>
    <option>Classical</option>
    <option>Opera</option>
  </select>
  <button id="btn" type="button">How many are selected?</button>
</form>
```
### `do while` loop

This loop also repeats until a conditon is false, but it does so in a much simpler way.

```javascript
let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);
```
This will run adding 1 to the value `i` until `i` hits the value 4 then it will stop and break the loop. 

### The `while` loop

This loop runs while a specific condition remains true. As soon as the condition is false the loop will cease.

For this one while `n` is less than 3 the loop will keep running

```javascript
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```

### Labeled Statements

A `label` provides the statement with an identifier that lets you refer to it in other places. You can have the label be any identifier that is not one of the reserved words for JavaScript

```javascript
markLoop:
while (theMark) {
  doSomething();
}
```

in this instace the label `markLoop`  identifies a while loop

### The Break Statement

The break statement ends a loop when it gets hit or comes up in the loop sequence.

This example goes through the elements of an array until if finds the specific value of an element whose value is equal to `theValue`

```javascript
for (let i = 0; i < a.length; i++) {
  if (a[i] === theValue) {
    break;
  }
}
```

You can also do something with the break like breaking to a Label

```javascript
let x = 0;
let z = 0;
labelCancelLoops: while (true) {
  console.log('Outer loops: ', x);
  x += 1;
  z = 1;
  while (true) {
    console.log('Inner loops: ', z);
    z += 1;
    if (z === 10 && x === 10) {
      break labelCancelLoops;
    } else if (z === 10) {
      break;
    }
  }
}
```

### The Continue Statement

The continue statement can be used to restart any of the `while`, `do-while`, `for`, or `label` statements.

* When you use continue without a label, it ends the current run of the loop and continues execution of the loop with the next iteration. As opposed to the break statement, continue does not end the execution of the loop entirely. In a while loop, it jumps back to the condition. In a for loop, it jumps to the increment-expression.
* When you use continue with a label, it applies to the looping statement identified with that label.

This example shows a `while` loop with a `continue` statment that executes when the value of `i` is `3`.

```javascript
let i = 0;
let n = 0;
while (i < 5) {
  i++;
  if (i === 3) {
    continue;
  }
  n += i;
  console.log(n);
}
//1,3,7,12
```

### `for in` Statememnts

The `for...in` statement iterates a specified variable over all the enumerable properties of an object. For each distinct property, JavaScript executes the specified statements. A for...in statement looks as follows:

```javascript
function dumpProps(obj, objName) {
  let result = '';
  for (const i in obj) {
    result += `${objName}.${i} = ${obj[i]}<br>`;
  }
  result += '<hr>';
  return result;
}
```

### `for of` Statements

The `for...of` statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property.

The following example shows the difference between a for...of loop and a for...in loop. While for...in iterates over property names, for...of iterates over property values:

```javascript
const arr = [3, 5, 7];
arr.foo = 'hello';

for (const i in arr) {
  console.log(i); // logs "0", "1", "2", "foo"
}

for (const i of arr) {
  console.log(i); // logs 3, 5, 7
}
```