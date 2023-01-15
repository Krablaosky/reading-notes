# Passing Functions as Props

## [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?

.map() returns a newly populated array with the results of a function that you call that iterates over every element in the calling array

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

if we want to loop through an array and display each value in JSX,we can do that using curly braces{ }. we would use our map functionon our arrayand we can use our curly braces within that loop to use the name of the array to collect all the elements and enter them


3. Each list item needs a unique ____.

each list item needs a unique key. if you don't have an explicit key to list items then react is gonna default to using indexes as keys

4. What is the purpose of a key?

the purpose of a key is to help react identify where these items are,it gives them a very unique identifying code that allows them to be accessed added or removed depending on if they have that access code.Keys should be given to the elements inside of arrays and give them and give them a stable identity.

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?

the spread operator is a parenthesis (...) of three dots. this helps expand an iterable objects into a list of arguments that can be read.

2. List 4 things that the spread operator can do.

One thing that the spread operator does is that it will literally spread an array into separate arguments so that way it can be read independently. it can also be useful for a lot of different tasks that are used in javascript like copying an array over, concatenating or combining arrays, using math functions, using an array's arguments, adding in an item to a list, adding it to state in react, combining objects, converting node list to an array.

3. Give an example of using the spread operator to combine two arrays.

if we had two different array, let's call them array A and array B. and we use the spread operator on both of those arrays. we would declare a new array using ...A, ...B. once we've done that we have combined both of those arrays. Here's an example of how it might look.

```
const A = ['1','2','3','4'];
const B = ['4','3','2','1'];

const AB = [...A, ...B];

console.log(AB); // Will result in ['1','2','3','4','4','3','2','1']
```


4. Give an example of using the spread operator to add a new item to an array.

Code Sample from Medium.com
```
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```


5. Give an example of using the spread operator to combine two objects into one.

Code Sample from Medium.com
```
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```

## [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step that the developer does to pass functions between components?

The first step the developer does to pass the function between components is to pass arguments to the child component so that it can be accessed on the lower level, This is where you would add your function so that it could be passed down using this.function

1. In your own words, what does the increment function do?

The increment function searches through the array of people's names tries to match it up to the original array And if it does match it will increase the count in that person's name. After that the name of the person in the count will be replaced with the updated name and count.

3. How can you pass a method from a parent component into a child component?

You can pass a method from a parent component into a child component, by passing the function down from the parent level as an argument. 

4. How does the child component invoke a method that was passed to it from a parent component?

Then inside the child component you would you would incorporate it as a prop inside of another function that is activated in the child function. So that way as it's called it also calls the parent function. We would then pass in the prop of the component we want like a name or title and it would update the state at the parent level.