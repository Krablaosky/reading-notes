# HTML, CSS, & JS continued

## HTML

HTML is a crucial part of what we are learning because it is the backbone of what we are building, a website powered by imagination and lots of funky code. It is integral to us being able to build a large scale website that has a lot of user functionality behind it.

1. Why is it important to use semantic elements in our HTML?

It is important to use semantic elements in our HTML because it helps us to clearly understand the code that we are using. If we had a bit of code called `getNumber()` that really gave out favorite flavors of ice cream then it wouldn't really be helpful would it. A function called `iceCreamFlavor()` would be more appropriately named. We can also use some semantic elements in our HTML to easily use preset parts for building our HTML. Take the `<h1>` element, this is a predefined header element that clearly explains what we want.

2. How many levels of headings are there in HTML?

There are six heading elements that we can use to change the size of our headings. `<h1>` through `<h6>` actually get smaller as the numbers get bigger. Imagine `h1` is the #1 heading and `h6` is the 6th place heading.

3. What are some uses for the `<sup>` and `<sub>` elements?

 `<sup>` and `<sub>` stand for Superscript and Subscript accordingly. We would want to use these for things like math equations or dates or basically anything that needs text to be above or below the main text line. The Superscript `<sup></sup>` will put the text above the main line while the Subscript `<sub></sub>` will put the text below. 

 For example: My birthday is on the 25<sup>th</sup> of some<sub>random</sub> month.

 actually looks like `My birthday is on the 25<sup>th</sup> of some<sub>random</sub> month.`

4. When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

When using the `<abbr>` element we would want to use the `title` attribute to show the full expansion of the text.

If we had the line `<p> Don't talk to <abbr title = "Reverend"> Rev.</abbr>  about this stuff.</p>`

it would look like

<p> Don't talk to <abbr title = "Reverend"> Rev.</abbr>  about this stuff.</p>

## CSS

CSS is super useful to us in terms of styling our website the way we need. It makes a super easy way to adjust and finagle certain pieces of styling without having to hunt through the stack of code to change it. It is an extremely efficient and functional way to make our website beautiful.

1. What are ways we can apply CSS to our HTML?

We can apply CSS to our HTML in 2 ways. Inline or an independent style sheet will get you similar results. The choice of preference is really dependent on what you need to do and how specific you want to get.

2. Why should we avoid using inline styles?

Inline styles are great if you want to only target one specific element. They should usually be avoided because building a style sheet is the most efficient way to make changes to sections of HTML. It also will crowd your HTML code and make it that much more difficult to read.

3. Review the block of code below and answer the following questions:
   
   1. What is representing the selector?
   
   The selector in the shown coding is the `h2` designation, which tells you that you are customizing the `h2` tag.

   2. Which components are the CSS declarations?

The declaration for this CSS code is the whole of the `color: black;` and the `padding:5px` which encompasses the whole of these sections. Each piece is broken up into the first part which is a property and the second part is the value.
   
   3. Which components are considered properties?
   
The properties for this CSS code is the `color` and the `padding`. The `color` sets the text color for `h2` and the `padding` sets the amount of space around the `h2` section.

Super helpful CSS Link
https://overapi.com/css 
## JS

Javascript is the part I am the most excited to delve into. This is the real power behind a website. This is what makes all the parts move and gets all the information. It's incredibly important for how we get our website to process data and utilize it.

1. What data type is a sequence of text enclosed in single quote marks?
   1. The data type that is enclosed in `' '` would be the `string` data type. It can also be figured out through the use of the `typeof()` function and putting the value inside of that function.
2. List 4 types of JavaScript operators.
   1. The types of JavaScript operators that we have are Arithmetic, Comparison, Logical, Assignment, and conditional.
      1. Arithmetic- These are your basic math functions like `+`, `-`, `*`, and `\`. There are more than this but this is the baseline.
      2. Comparison- These do exactly what you think, compare at least 2 variables to each other and determine the output. Most commonly we will see `==`, `===`, `!=`(not equal), `>`, `<`, `>=`,`<=`
      3. Logical- Our logical operators cover the gambit of whether multiple conditions can exist. Basically does `a` and `b` satisfy our code? or will we take `a` or `b`. We use `&&` for our `and`, `||` for our `or`, and `!` for our `not`
      4. Assignment- These reassign a value to our variable, most commonly in the form of `=`, but also with a few special cases of `+=`, `-=`, `*=`, `/=`, `%=`, `**=`
      5. Conditional- these operators take 3 operands to function. The operator can only have one of the 2 values based on a condition given. it often looks like `condition ? val1 : val2`
3. Describe a real world Problem you could solve with a Function.

A real world problem that you could solve with a function would be figuring out your weekly take home from your salary. Thats an extremely simple one that could work pretty easily by assigning your salary a value, and using arithmetic operators to break it down into weeks and takeaway your taxes. You could expand it further by using logical operators to figure out how vacation time would play into that or special holiday pay.
## JS Conditionals

1. An if statement checks a __ and if it evaluates to ___, then the code block will execute.
   1. An if statement checks a condition and if it evaluates to true then the code block will execute
2. What is the use of an `else if`?
   1. the use of an `else if` statement is to check multiple conditions and provide specific output based on those different scenarios.
3. List 3 different types of comparison operators.
   1. Most commonly we will see `==`, `===`, `!=`(not equal), `>`, `<`, `>=`,`<=`
4. What is the difference between the logical operator `&&` and `||`?
   1. the difference between these two logical operators is that the `&&` is the `and` operator while the `||` is the `or` operator. The `&&` operator needs all conditions to be met in order for the code block to execute, whether all is `true` or all is `false` all conditions need to meet the criteria. This is different from the `||` operator where if any of the conditions are met then the code block will run. You could have a hundred `||` operators and if only one of them is true then the code block will run.