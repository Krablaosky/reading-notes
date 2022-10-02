# What is Javascript?

Javascript is a lightweight  compiled programming language with first class functions. It is the most well known scripting language for web pages as well as non browser environments like Adobe Acrobat. Javascript works inside the browser on the client side rather than on the web server side. Javascript is entirely different than Java so don’t get them confused.

When referring to JS we usually break it into 3 parts

* the language itself
* the DOM API or how the language interactsw ith other parts of the browser
* API or server API

JS You can use any text editor for working JS . to embed some JS code in our HTML files we use the `<script> code goes here </script>`4

See this example below

```javascript
First line
<script>

document.write("<h1>Hello World</h1>");

</script>
Last line
```

In this example we have a normal first line of code them some JS code that uses the function `document.write` to edit the content of the page

Now that we know what it looks like what can we do with it.
We can use it for prompts inside a webpage

```javascript
<script>

var name = prompt("Your name:", "");
document.write("Hello ", name);

</script>
```

Check this out, this will prompt a user inside this section for their name and take that information.

We can use this to ask questions and get answers and use that to enact different actions. The below code asks the user if they should print hello world and uses their input to determine the response.

```javascript
<script>

if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
} else {
    document.write("OK, I won't print it.");
}

</script>
```

JavaScript Variables

What are variables?

JS variables are containers for storing data. We want to keep responses and information in labeled boxes. Imagine you had a room full of boxes and wanted to quickly find saved information. It would be easiest to label the outside of the box that information goes into so you know which one to grab when someone asks about their email address.

We have a few ways to declare variables
Using

* `var`
* `let`
* `const`
* using nothing

For example, we can use this for something simple like a math equation

```javascript
var x = 5;
var y = 6;
var z = x + y;
```

For example, we establish constants and use that information to determine total price. We have defined what these variables are with this information and how they relate.

```javascript
const price1 = 5;
const price2 = 6;
let total = price1 + price2;
```

Identifiers in JS

All JS variables must have unique names to work. It can be something simple like a single letter ‘a’ or can be a full word ‘total-variable’
Some naming rules
Names can contain letters, digits, underscores, and dollar signs.
Names must begin with a letter.
Names can also begin with $ and _ (but we will not use it in this tutorial).
Names are case sensitive (y and Y are different variables).
Reserved words (like JavaScript keywords) cannot be used as names.

For example a more complex statement might look like

```javascript
let person = "John Doe",
carName = "Volvo",
price = 200;
```

You can even leave some undefined so that the information can be filled in later.

## How do computers work?

### What makes a computer a computer?

Computers take input, store it, process it and then provide output. That's what makes a computer a computer. The original ones were mechanical and wood and now we have advanced to have them be so small they are in your wrist.

Computers take input from a few ways.'

* Keyboard
* Mouse
* Sensors 
* Audio 
* Visual

All of this gets stored in the memory then it gets processed and restored in memory then it outputs it for you to see the results.

Computers work on Binary coding.

Binary works in positions by doubling up. We calculate binary by starting at the largest number and seeing how many of them fit in and mark it with a `1`, any gaps we fill in with a `0`. Thats how we give ID's to numbers and pretty much everything.

This works to calculate out text by assigning numbers to build text, since each letter has a number it gets translated out.

Circuits work by turning on of off binary signals to translate them into different outputs

Keyboard converts letter into number, then the cpu calculates how to draw the image and then stores this pixes information and then outputs the image you see on the screen.

Now we are using software which helps process all of the binary information in millions of ways to allow us to customize our computers and turn inputs into outputs.
