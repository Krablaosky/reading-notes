# Javascript Objects and DOM

## Javascript Objects

1. How would you describe an object to a non-technical friend you grew up with?

An Object to me is a box of stuff you have organized a little bit, and sometimes not at all.
An Object is a box of toys that all have a few key details about them that are important. Each item in the box has some cool details like name, date you bought it, what it does etc.

2. What are some advantages to creating object literals?

Some benefits of creating Object Literals is for when you want to utilize or transfer very specific information. It's useful for when you want to create some structured and related data, that way you can reference the items in that object using the same keywords and know what it should contain. It is a much faster process than sending objects over one at a time.

3. How do objects differ from arrays?

Object differ from Arrays because Arrays are ordered lists of items, while objects are collections of data and key values that store more information. An Array is really useful for looking up a single value at an index, meanwhile an object is useful for scanning an entire piece to find the necessary information using dot notation.

4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

You would want to use bracket notation over dot notation in a few instances. In the case that you are looking for a property name held inside a variable you cant use dot notation to find that item, you can be more specific when you use bracket notation to locate a specific set of values.

5. Evaluate the code below. What does the term `this` refer to and what is the advantage to using `this`?

```javascript
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```
In this code the term `this` refers to the current object that the code is being written inside. So whatever code that is being worked on, in this instance `dog` is referred to when pulling the name out of it as well as the age. This is really useful when we start working with constructors.

## DOM

1. What is the DOM?

Stands for document Object Model and is a representation of the data that makes up the content and structure of a website. It is a programming interface for web documents that allows us to manipulate the HTML output while using JavaScript. Dom kinda takes the html information and makes it a visible document that can be altered and manipulated

2. Briefly describe the relationship between the DOM and JavaScript.

DOM and JS go hand in hand. DOM isn't a programming language and can't do a lot, just like Javascript would have no clue what an HTML is without DOM letting JS know what the components of HTML were. Once DOM and JS are working together they can be used in tandem to manipulate websites and add items to HTML. Think about it like JS can change the element information using powerful algorithms while DOM translates that information into HTML with ease.