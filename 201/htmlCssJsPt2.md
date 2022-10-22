# HTML CSS & JS Continued

## HTML Lists

Let's start off with why Ordered Lists vs Unordered Lists would be important. An unordered list is a list of items where the order doesn't matter and it will render as bullet points or other images like a shopping list. While ordered lists are intended to be followed in a specific order like a recipe.

1. When should you use an `unordered list` in your HTML document?

As stated above Unordered Lists or `<ul>` are for unordered-list items and can be shows as bullet points which can take many different shapes.

2. How do you change the `bullet style` of unordered list items?

You can change the `bullet style` of an Unordered List to look like a cirle, disc, square and triangle. There are even options to add your own custom images and you can do this using the `type` attribute in your CSS Sheet. It might look like

```css
li {
    list-style-type: circle;
}

li li {
    list-style-type: square;
}
```

3. When should you use an `ordered list` vs an `unorder list` in your HTML document?

Why would you want to use an unorderd list vs an ordered list? Well if you are following a recipe and your steps are all out of order then you are going to end up with a very strange bit of food. Those steps need to be followed in sequential order and the code will read them as such. An unordered list could be a collection of things you like, or a shopping list where the order doesn't matter as much.

4. Describe two ways you can change the numbers on `list items` provided by an `ordered list`?

There are a lot of really cool things you can do with ordered lists to make them look different. You can use the attribute `reversed` to change the numbers from high to low. You can use different types like the following.

* `a` for lowercase
* `A` for Uppercase
* `i` for lowercase Roman Numerals
* `I` for uppercase Roman Numerals
* `1` for numbers, which is usually the default.

## The Box Model

The box model is extremely important to the work we are doing with HTML because most everything ends up in a box. Whether it's long paragraphs of text or buttons to be clicked, boxes make up most of the way we can shape our HTML.

1. Describe the CSS properties of `margin` and `padding` as characters in a story. What is their role in a story titled: “The Box Model”?

If I had to describe `margin` and `padding` as characters in a story. Then `marge` the `marign` would be the character who is always on the outside of what is going on. She keeps her home(`box`) safe from the outside world by providing a barrier between them and the other boxes, she builds a fence on the outside of her property to get some space. `paddy` the `padding` lives inside the house and keeps all of the furniture away from the walls when it rains so that it doesn't get soaked.

2. List and describe the four parts of an HTML elements box as referred to by the box model.

The four parts of an HTML Element box are the margin, border, padding, and content. The margin is the part that keeps the box from nestling up against the sides of our website and gives them a little room. The border helps define the edges of the box and what is contained within it and outside of it. The padding keeps the content from crashing into the sides of the border and the content is the information we want to show inside our box.

## JS

Learning these JS operators is incredibly important to making all of the functionality in our website more robust and helps us to build cleaner code. We can use these arrays to store vast quantities of data and our loops to scan through that data to give us what we need.

1. What `data types` can you store inside of an `Array`?

We can store lots of data types inside of an `Array`. We can store lists of Strings, Numbers, Objects, and even other Arrays.

2. Is the `people` array a valid JavaScript array? If so, how can I access the values stored? If not, why?

```javascript
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
 ```

The `people` array will run, I was initially concerned about `null` being an item inside the array but it can in fact run. We can use a variety of methods to access the data. We can use `people[0]` to grab a singular value at a specific position. We can use something like `people[2][2][3]` to grab a value out of each array list living inside this array.

3. List five shorthand operators for assignment in javascript and describe what they do.

some of our shorthand operators for JS are as follows.

* `=` this assigns a value to a variable
* `+=` This is our addition assignment that adds the value on the right to the variable value on the left, then returns the new variable value
* `-=` This is our subtraction assignment that subtracts the value on the right from the variable value on the left, and returns the new variable value
* `*=` This is our multiplication assignment that multiplies the variable value on the left by the value on the right, and returns the new variable value
* `/=` This is our division assignment that divides the variable value on the left by the value on the right, and returns the new variable value

4. Read the code below and evaluate the last `expression` and explain what the result would be and why.

```javascript
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
 ```

this expression would give us `10dog`. This is because type coercion combines all of this together, since `a` is a number and `c` is a boolean it converts to a number, since `null` is not a number we get `10`. Then it adds it to the string of `b` and converts it all to a string, leaving us `10dog`

5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

So a conditional statement in the real world would be like cooking and following a recipe. It is something that says if you meet this condition let's execute what we want. So our recipe says "hey, do you have these ingredients?" if you say, "sure I got em" then you would proceed to cook with the ingredients.

6. Give an example of when a `Loop` is useful in JavaScript.

A `loop` is useful in JavaScript because it helps us to simplify our code. We can run a singular piece of code over and over a million times until our conditions are met. Think about if you had to write the same line over and over again on a word document. Then you figure out you can just copy+paste that line over and over. It makes it a lot easier and saves a lot of time. So for wanting to find an item inside of an array we would use a loop to "scan" through the array which could have a million items in it,  until we find the item we want. 